<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<style>
body { margin:0; font-family:sans-serif; background:#eee; }

/* 상단 */
.header {
  background:white;
  padding:12px;
  text-align:center;
  font-weight:bold;
  position:relative;
}
.menu {
  position:absolute;
  right:10px;
  top:12px;
  font-size:20px;
}

/* 탭 */
.tabs { display:flex; background:white; border-bottom:1px solid #ddd; }
.tab { flex:1; text-align:center; padding:10px; }
.active { border-bottom:2px solid black; font-weight:bold; }

/* 카드 */
.card { padding:20px; background:#f5f5f5; }

.photo {
  width:150px;
  display:block;
  margin:auto;
}

.nameBox {
  display:flex;
  justify-content:space-between;
  align-items:center;
  margin-top:15px;
}

.name { font-size:22px; font-weight:bold; }
.gray { font-size:12px; color:gray; }

/* QR */
.qr img { width:100px; }

/* 타이머 */
.timer { margin-top:10px; font-size:13px; }
.bar {
  height:4px;
  background:#ddd;
  margin-top:5px;
}
.fill {
  height:100%;
  width:100%;
  background:#3b5cff;
}

/* 바코드 */
.barcode {
  height:60px;
  margin-top:20px;
  background: repeating-linear-gradient(
    to right,
    black 0px,
    black 1px,
    white 1px,
    white 2px,
    black 2px,
    black 4px,
    white 4px,
    white 5px,
    black 5px,
    black 8px,
    white 8px,
    white 10px,
    black 10px,
    black 11px,
    white 11px,
    white 13px
  );
}

/* 상세정보 */
.detail {
  display:none;
  margin-top:10px;
  font-size:14px;
}

/* 버튼 */
.bottom {
  margin:20px;
  padding:15px;
  background:black;
  color:white;
  text-align:center;
  border-radius:10px;
}

/* 설정창 */
.modal {
  display:none;
  position:fixed;
  top:0;
  left:0;
  width:100%;
  height:100%;
  background:rgba(0,0,0,0.7);
}
.modalContent {
  background:white;
  margin:50px;
  padding:20px;
}

input { width:100%; margin:5px 0; }
</style>
</head>

<body>

<div class="header">
  모바일신분증
  <span class="menu" onclick="menuTap()">≡</span>
</div>

<div class="tabs">
  <div class="tab active">주민등록증</div>
  <div class="tab">운전면허증</div>
</div>

<div class="card">

  <img id="img" class="photo" src="https://via.placeholder.com/150">

  <div class="nameBox">
    <div>
      <div class="gray">주민등록증 모바일 확인서비스</div>
      <div class="name" id="name">홍길동</div>
      <div id="detail" class="detail"></div>
    </div>

    <div class="qr">
      <img src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=test">
    </div>
  </div>

  <div class="timer">
    남은시간 <span id="time">30</span>초
    <div class="bar"><div class="fill" id="bar"></div></div>
  </div>

  <div class="barcode"></div>

</div>

<div class="bottom" onclick="toggleDetail()">상세정보 표시</div>

<!-- 설정창 -->
<div class="modal" id="modal">
  <div class="modalContent">
    <input id="nameInput" placeholder="이름">
    <input id="birthInput" placeholder="생년월일">
    <input id="addrInput" placeholder="주소">
    <input id="regionInput" placeholder="지역">
    <input type="file" onchange="changeImg(event)">
    <button onclick="apply()">저장</button>
  </div>
</div>

<script>

// 메뉴 4번 터치
let tapCount = 0;
function menuTap(){
  tapCount++;
  if(tapCount >= 4){
    modal.style.display = "block";
    tapCount = 0;
  }
}

// 사진 변경
function changeImg(e){
  let reader = new FileReader();
  reader.onload = function(){
    img.src = reader.result;
    localStorage.setItem("img", reader.result);
  }
  reader.readAsDataURL(e.target.files[0]);
}

// 저장
function apply(){
  localStorage.setItem("name", nameInput.value);
  localStorage.setItem("birth", birthInput.value);
  localStorage.setItem("addr", addrInput.value);
  localStorage.setItem("region", regionInput.value);

  name.innerText = nameInput.value;
  modal.style.display = "none";
}

// 상세정보
function toggleDetail(){
  if(detail.style.display === "block"){
    detail.style.display = "none";
  } else {
    detail.innerHTML =
      (localStorage.getItem("birth")||"") + "<br>" +
      (localStorage.getItem("region")||"") + "<br>" +
      (localStorage.getItem("addr")||"");
    detail.style.display = "block";
  }
}

// 🔥 타이머 (완전 수정)
let time = 30;
let max = 30;

const timeText = document.getElementById("time");
const bar = document.getElementById("bar");

function updateTimer(){
  time--;

  if(time < 0){
    time = max;
  }

  timeText.innerText = time;
  bar.style.width = (time/max)*100 + "%";
}

setInterval(updateTimer, 1000);

// 초기 상태
timeText.innerText = time;
bar.style.width = "100%";

// 로드
window.onload = function(){
  let savedName = localStorage.getItem("name");
  let savedImg = localStorage.getItem("img");

  if(savedName) name.innerText = savedName;
  if(savedImg) img.src = savedImg;
};

</script>

</body>
</html>