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
      <flexbox :gutter="0">
          <flexbox-item>
            <router-link to="/"> 
              <p>首页</p>
            </router-link>
          </flexbox-item>
          <flexbox-item>
            <router-link to="/join"> 
              <p>彩票游戏</p>
            </router-link>
          </flexbox-item>
          <flexbox-item>
            <router-link to="/lotteryRes"> 
              <p>手机下注</p>
            </router-link>
          </flexbox-item>
          <flexbox-item>
            <router-link to="/user"> 
              <p>在线客服</p>
            </router-link>
          </flexbox-item>
        </flexbox>
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
      disabledPrev: false,
      disabledNext: false
    };
   }
   //,
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
  // methods: {
  //   turnPage(v) {
  //     let startRow;
  //     if (v == 'prev') {
  //       startRow = this.startRow - this.pageSize;
  //     }
  //     if (v == 'next') {
  //       startRow = this.startRow + this.pageSize;
  //     }
  //     if (startRow <= 0) {
  //       startRow = 0;
  //     }
  //     this.$emit('change', startRow);
  //   }
  // }
};
</script>
<style lang="less" scoped>
@import url('./Top.less');
</style>
