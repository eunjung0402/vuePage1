<template>
  <v-container class="footer">
    <div class="left">
      <ul>
        <li><a href="">개인정보 보호정책</a></li>
        <li><a href="">서비스이용약관</a></li>
        <li><a href="">제휴문의</a></li>
      </ul>
      <div class="footer_div_1">
        <span>㈜로앤텍</span>
        <span>대표:조성화</span>
        <span>서울시 서초구 양재천로21길 29, 202호(양재동)</span>
      </div>
      <div class="footer_div_2">
        <span>사업자등록번호:211-88-86547</span>
        <span>대표전화:<b>070-4652-7068</b></span>
        <span>이메일:priros.rp@gmail.com</span>
      </div>
      <p>COPYRIGHT Ⓒ PRIROS ALL RIGHTS RESERVED.</p>
    </div>
    <div class="right">
      <p>PRIROS</p>
    </div>
  </v-container>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
.footer {
  background-color: gray;
}
.container {
  max-width: 100%;
}
</style>
