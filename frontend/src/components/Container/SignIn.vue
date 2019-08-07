<template>
    <div>
        <!--로그인-->
        <div style="width: 20%; margin:0 auto;">
            <h2>로그인</h2>
            <div class="container" style="padding: 10% 0%;">
                <label for="exampleInputId">아이디를 입력하세요</label>
                <input type="id" class="form-control" v-model="id" id="exampleInputId" aria-describedby="idHelp" placeholder="Enter id">
            </div>
            <div class="container" style="padding:0 0;">
                <label for="exampleInputPassword">비밀번호를 입력하세요</label>
                <input type="password" class="form-control" v-model="password" id="exampleInputPassword" placeholder="Password">
            </div>
            <b-button class="btn" to="SignUp" style="margin:10% 0%; padding:0% 10%;">회원가입</b-button>
            <button type="submit" class="btn btn-outline-dark" style="margin:10% 0; padding:0 10%;" v-on:click="Login">로그인</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: "SignIn",
       
    }
</script>

<style scoped>
button {
        float: right;
    }
    
    h2 {
        font-size: 45px;
        padding:20% 0;
    }
</style>