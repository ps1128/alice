<style scoped>
  .container {
    overflow-y: scroll;
    margin-top: 60px;
  }
  .input-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    align-content: center;
    justify-content: center;
    /* width: 80%;
    height: 60%; */
  }
  .headline{
    font-size: 22px;
    text-align: center;
    padding: 20px;
}
input[type="text"],
input[type="submit"]{
  -webkit-appearance: none;
  -webkit-animation: none;
  display: block;
  margin: 0 auto;
  font-size: 15px;
  width: 240px;
}
input[type="text"]{
  height: 35px;
  border-radius: 3px;
  border:1px solid #cBcccf;
  color:#6a6f77;
  outline: 0;
}
input[type="submit"]{
  margin-top: 25px;
  height: 35px;
  background: #357eb8;
  color:#bcedff;
  font-weight: bold;
  font-size: 16px;
}
input[type="submit"]:hover{
  background:#0e62a3;
  cursor: pointer;
}
.astyle{
  margin: 5px 0 5px 70px;
  font-size: 18px;
  color: #6a6f77;
}
.bstyle{
  display: block;
  float: left;
  margin-left: 70px;
  font-size: 15px;
}
.cstyle{
  display: block;
  float: left;
  margin-left: 70px;
  font-size: 15px;
}
.cstyle a{
  text-decoration: none;
}
</style>

<template>
  <div class="container">
    <div class="input-container">
      <form action="#" method="get">
        <p class="headline">用户登录</p>
        <p class="astyle">用户名：</p>
        <input class="astyle" type="text" placeholder="请输入用户名">
        <p class="astyle">密码：</p>
        <input class="astyle" type="password" placeholder="请输入密码">
        <input type="submit" value="登陆" name="login" >
        <p class="bstyle"><input type="checkbox" name="rempas">  记住密码</p>
        <p class="cstyle">忘记密码</p>
        <p class="cstyle">没有账号？<router-link to="/register">立即注册</router-link></p>
      </form>
    </div>
  </div>
</template>
