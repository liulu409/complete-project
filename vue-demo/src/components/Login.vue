<template>
  <el-row class="content">
    <el-col :xs="24" :sm="{span: 6,offset: 9}">
      <span class="title">
       欢迎登录
      </span>
      <el-row>
        <el-input class="input-login"
                  v-model="account"
                  placeholder="账号"
                  type="text">
        </el-input>
        <el-input class="input-login"
                  v-model="password"
                  placeholder="密码"
                  type="password">
        </el-input>
        <el-button type="primary" class="btn-login">登录</el-button>
      </el-row>
    </el-col>
  </el-row>
</template>

<script>
  export default {
    data() {
      return {
        account: '',
        password: ''
      };
    }
  };
</script>

<style scoped>
  .title {
    font-size: 28px;
  }

  .input-login {
    margin: 12px 0;
  }

  .btn-login {
    width: 100%;
    margin-top: 12px;
  }
</style>
