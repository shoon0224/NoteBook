<template>
    <div>
        <nav>
          <ul class="nav-container">
            <router-link class="nav-item" to="/"> <h2> NoteBook</h2> </router-link>
            <router-link class="nav-item" to=""> <a> 종류  </a></router-link>
            <router-link class="nav-item" to=""> <a> 노트북 검색</a></router-link>
            <router-link class="nav-item" to="SignIn"> <a> 로그인 </a></router-link>
          </ul>
        </nav>
    </div>
</template>

<script>
    export default {
        name: "Nav"
    }
</script>

<style scoped>
body {
  margin: 0; 
}
/* 바디의 바깥 여백을 없앰으로서 내비게이션 바가 페이지에 바짝 붙게 함*/


.nav-container{
  display: flex; /*아이템을 가로로 나열*/
  flex-direction: row; /* 이거 뭐지*/
  width: 100%; /*차지 범위를 100%로 한다.*/

  background-color: black; 
  list-style-type: none/*아이템 앞에 점 제거*/
}

.nav-item {
  margin: 0px 15px ; /*아이템들 글자 간격 띄우기*/
  cursor: pointer;/*마우스를 올렸을 때 포인터모양을 바꾸는 것*/
  text-align: center;
  color: white;
  text-decoration:none;/*밑줄 없앰*/

}
.nav-item a{
text-align: center;
float: right;
}

.nav-container {
  position: fixed;
  top: 0; /*상단 위치를 0으로 함으로서 위에 붙음*/
}
.nav-item a:hover {
  background-color: #0F1A31;
}
</style>