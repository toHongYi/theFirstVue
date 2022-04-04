<template>
  <div style="text-align:center">
    <h2>欢迎你 {{ username }}登录成功！</h2>
    <img src="">
    <router-link to='/'>
      <span>返回登录界面</span>
    </router-link>
  </div>
</template>

<script>
import Cookies from 'js-cookie';
export default{
  computed:{
    username(){
      return Cookies.get('userName');
    }
  }
}


</script>
<!-- 添加“scoped”属性以将CSS仅限于此组件 -->
<style scoped>




</style>
