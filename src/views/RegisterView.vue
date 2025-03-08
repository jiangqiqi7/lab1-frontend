<script setup>
import { RouterLink } from 'vue-router'
</script>


<template>
  <div class="reg-box">
    <h1>注册</h1>
    <form>
      <div class="textbox">
        <input type="text" placeholder="用户名" name="username" />
      </div>
      <div class="textbox">
        <input type="password" placeholder="密码" name="password" />
      </div>
      <div class="verify">
        <input type="text" placeholder="验证码" name="verify" />
        <img src="https://picsum.photos/200/100" width="60px" height="40px" alt="验证码" />
      </div>
      <input type="submit" class="btn" value="注册" />
    </form>

    <div>
      已有账号？<RouterLink to="/">登录</RouterLink>
    </div>
  </div>
</template>


<style scoped>

.reg-box {
    width: 300px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: var(--color-text);

    background: #ebeff1;
    border: 4px;
    padding: 40px;
    border-radius: 12px;

    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
  }

  .reg-box h1 {
    float: left;
    font-size: 40px;
    border-bottom: 6px solid #4caf50;
    margin-bottom: 20px;
    padding: 13px 0;
  }

  .textbox {
    width: 100%;
    overflow: hidden;
    font-size: 20px;
    padding: 8px 0;
    margin: 8px 0;
    border-bottom: 1px solid #4caf50;
  }

  .textbox i {
    width: 26px;
    float: left;
    text-align: center;
  }

  .textbox input {
    border: none;
    outline: none;
    background: none;
    color: var(--color-text);
    font-size: 18px;
    width: 80%;
    float: left;
    margin: 0 10px;
  }

  .btn {
    width: 60%;
    background: #799ccb;
    box-shadow: rgba(0, 0, 0, 0.15) 1.95px 1.95px 2.6px;
    border: 0px;
    border-radius: 8px;
    color: var(--color-text);
    padding: 5px;
    font-size: 18px;
    cursor: pointer;
    margin: 12px 0;
    margin-left: 20%;
  }

  .verify {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .verify input {
    overflow: hidden;
    padding: 8px 0;
    border: none;
    border-bottom: 1px solid #4caf50;
    outline: none;
    background: none;
    color: var(--color-text);
    font-size: 18px;
    width: 80%;
    float: left;
    margin: 0 10px;
  }
</style>
