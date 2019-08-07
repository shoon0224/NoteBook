<template>
    <div>
        <!--회원가입-->
        <div style=" width: 20%; margin:0 auto; ">
            <h2>회원가입</h2>
            <div class="form-group">
                <label for="exampleInputId">아이디</label>
                <input type="id" v-model="id" class="form-control" id="exampleInputId" aria-describedby="idHelp" placeholder="id">
            </div>
            <div class="form-group">
                <label for="exampleInputPassword">비밀번호</label>
                <input type="password" v-model="password" class="form-control" id="exampleInputPassword" placeholder="Password">
            </div>
            <div class="form-group">
                <label for="exampleInputUsername">유저이름</label>
                <input type="text" v-model="username" class="form-control" id="exampleInputUsername" placeholder="Username">
            </div>
            <button class="btn btn-outline-dark" v-on:click="reqSignUp">확인</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: "SignUp",
    
    }
</script>

<style scoped>
button {
        float: right;
    }
    
    h2 {
        font-size: 45px;
        padding: 20% 0;
    }
</style>