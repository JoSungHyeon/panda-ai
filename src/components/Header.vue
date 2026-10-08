<template>
  <header>
      <div class="logo en">
          <span class="p">P</span>
          <span class="a">A</span>
          <span class="n">N</span>
          <span class="d">D</span>
          <span class="a2">A</span>
          <span class="dash">-</span>
          <span class="a3">A</span>
          <span class="i">i</span>
      </div>
      <div class="loginBtn kr">로그인</div>
  </header>
</template>

<style scoped>
header {
  background-color: #fff;
  padding: 1rem 1.5rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: fixed;
  z-index: 2;
  top: 0;
  left: 0;
  width: 100%;
  border-bottom: 1px solid #ccc;
  background-color: #F2F2F2;
}

.logo {
  display: inline-flex;
  align-items: center;
  font-size: 30px;
  font-weight: 900;
  line-height: 1;

  letter-spacing: 1.2;
}

/* P */
.logo .p {
  color: #E3B9FF;
}

/* A */
.logo .a {
  color: #B7CFFF;
}

/* N */
.logo .n {
  color: #83CFFF;
}

/* D */
.logo .d {
  color: #B4D5E8;
}

/* A */
.logo .a2 {
  color: #F3B7B7;
}

/* - */
.logo .dash {
  color: #F4B1B1;
  margin: 0 2px;
}

/* A */
.logo .a3 {
  color: #FFBE8A;
}

/* i */
.logo .i {
  color: #FFB26D;
}

.loginBtn {
  font-size: 24px;
  font-weight: 600;
}
</style>