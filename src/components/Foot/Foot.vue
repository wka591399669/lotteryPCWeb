<template>
  <div id="Top">
    <div class="topClass">
      <div><img src="../../assets/img/end_log.png" alt=""></div>
      <div>
        <div>
          <span>线上客服</span>
          <span>|</span>
          <span>加入收藏</span>
          <span>|</span>
          <span>玩法介绍</span>
        </div>
        <div>
          <div>
            <span>您好：</span><span class="red">zhangyihua</span><span>可用余额：</span><span class="red">￥8888.88</span><span><img src="../../assets/img/message.png" alt=""></span>
          </div>
          <div>
            <span>会员中心</span>
            <span>|</span>
            <span>充值</span>
            <span>|</span>
            <span>提现</span>
            <span>|</span>
            <span>交易记录</span>
            <span>|</span>
            <span>未读消息(0)</span>
            <span>|</span>
            <span>安全退出</span>
          </div>
        </div>
      </div>
    </div>
    <div>
      <el-menu :default-active="activeIndex2" class="el-menu-demo" mode="horizontal" 
        background-color="#111" text-color="#e9b02b" active-text-color="#FFFFFF" >
        <el-menu-item index="1">首页</el-menu-item>
        <div class="gameTypeClass">
          <el-submenu index="2">
            <template slot="title">彩票游戏</template>
            <div class="gameTypeListClass">
              <el-menu-item index="2-1"><span>北京幸运28</span></el-menu-item>
              <el-menu-item index="2-2"><span>北京幸运28</span></el-menu-item>
              <el-menu-item index="2-3"><span>北京幸运28</span></el-menu-item>
              <el-menu-item index="2-4"><span>北京幸运28</span></el-menu-item>
              <el-menu-item index="2-5"><span>北京幸运28</span></el-menu-item>
              <el-menu-item index="2-6"><span>北京幸运28</span></el-menu-item>
              <el-menu-item index="2-7"><span>北京幸运28</span></el-menu-item>
              <el-menu-item index="2-8"><span>北京幸运28</span></el-menu-item>
              <el-menu-item index="2-9"><span>北京幸运28</span></el-menu-item> 
            </div>
          </el-submenu>
        </div>
       
        <el-menu-item index="3">手机下注</el-menu-item>
        <el-menu-item index="4">在线客服</el-menu-item>
        <el-menu-item index="5">注册账号</el-menu-item>
      </el-menu> 
    </div>
  </div>
</template>
<script>
import { Flexbox, FlexboxItem } from 'vux';

export default {
  name: 'Pages',
  components: { 
    Flexbox,
    FlexboxItem
  }, 
  data() {
    return {
      activeIndex: '1',
      activeIndex2: '1',
      disabledPrev: false,
      disabledNext: false
    };
   },
  // computed: {
  //   totalPage() {
  //     return Math.ceil(this.totalCount / this.pageSize);
  //   },
  //   nowPage() {
  //     return Math.ceil((this.startRow + 1) / this.pageSize) || 1;
  //   }
  // },
  // created() {
  //   this.turnPage();
  // },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  }
};
</script>
<style lang="less" scoped>
@import url('./Foot.less');
</style>
