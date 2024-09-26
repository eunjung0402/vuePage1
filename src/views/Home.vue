<template>
  <div class="home">
    <v-img
      lazy-src="../assets/bg-main-01.jpg"
      max-width="100%"
      min-height="900px"
      src="../assets/bg-main-01.jpg"
    ></v-img>
    <div class="main-text">
      <h2>우리동네 등기사건은 내가 접수한다!</h2>
      <p>마켓에서 사건을 수임하고, 오피스로 업무를 처리해보세요.</p>
      <p>여기는 프리로스 입니다.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>
<style scoped>
h2 {
  font-size: 4rem;
}
p {
  font-size: 1.5rem;
}
.home {
  position: relative;
}
.main-text {
  position: absolute;
  top: 300px;
  width: 100%;
  margin: auto;
  color: #fff;
  text-align: center;
}
</style>
