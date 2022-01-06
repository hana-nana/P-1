<!--

###네비게이션바를 가져온다.
const nav = document.querySelector("#main");

###상대적으로 가장 가까운 부모 엘레먼트의 상단에서부터의 픽셀값을 구한다.
let topOfNav = nav.offsetTop;

###네비게이션바을 움직이는 함수를 만든다.
function fixNav() {
        
###만약 스크롤을 topOfNav 보다 많이 내리면 즉, 네비게이션바 윗부분에 화면 끝이 닿으면 아래 내용이 발동된다.
if (window.scrollY >= topOfNav) {
    document.body.style.paddingTop = nav.offsetHeight + "px";
    document.body.classList.add("fixed-nav");
} else {
          
###그렇지 않으면 아래 내용이 발동된다.
document.body.classList.remove("fixed-nav");
document.body.style.paddingTop = 0;
    }
}

###scroll이 움직이면 fixNav 함수가 작동된다.
window.addEventListener("scroll", fixNav); 

###HTML에 JS 링크 걸어서 연결하는 코드
<script src="side page.js"></script>

-->