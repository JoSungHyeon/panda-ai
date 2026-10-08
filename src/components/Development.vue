<template>
  <div class="mainPage">
    <div class="development">
      <div class="icon">🚧</div>
      <h1>개발중입니다</h1>
      <p>더 나은 서비스를 위해 열심히 준비하고 있어요.</p>
    </div>
  </div>
</template>

<style scoped>
.mainPage {
  width: 100vw;
  height: 100vh;
  background-color: #F2F2F2;

  display: flex;
  align-items: center;
  justify-content: center;
}

.development {
  text-align: center;
  padding: 50px 70px;
  background-color: #FFFFFF;
  border-radius: 24px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.06);
}

.icon {
  font-size: 48px;
  margin-bottom: 20px;
}

h1 {
  margin: 0;
  font-size: 32px;
  font-weight: 700;
  color: #222;
}

p {
  margin: 12px 0 0;
  font-size: 16px;
  color: #888;
}
</style>