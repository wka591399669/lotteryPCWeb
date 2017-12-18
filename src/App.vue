<template>
  <div id="app">
     
    <transition enter-active-class="animated fadeIn" leave-active-class="animated fadeOut" mode="out-in">
      <router-view class="page"></router-view>
    </transition>
   
  </div>
</template>

<script>
  
export default {
  name: 'app', 
  data() {
    return {
      show: ['Home', 'Join', 'LotteryRes', 'User']
    };
  }
};
</script>
<style lang="less"> 

</style>


