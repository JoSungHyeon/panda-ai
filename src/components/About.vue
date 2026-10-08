<template>
  <section class="about">
    <div class="aboutInner">

      <div class="aboutTitle">
        <span class="label en">ABOUT PANDA-AI</span>

        <h2 class="kr">
          복잡한 제작 과정을<br />
          <span>대화 하나로</span> 간단하게.
        </h2>

        <p class="description kr">
          판다 AI는 기획부터 디자인, 콘텐츠 제작까지<br />
          제품 페이지 제작에 필요한 과정을 쉽고 빠르게 도와줍니다.
        </p>
      </div>


      <div class="aboutCards">

        <div class="aboutCard cardPurple">
          <div class="cardNumber en">STEP 1</div>

          <div class="cardContent">
            <h3 class="kr">제품 설정</h3>
            <p class="kr">
              제품 설정 및 제품 상세 설명과 컬러 설정
            </p>
          </div>

          <div class="circle"></div>
        </div>


        <div class="aboutCard cardBlue">
          <div class="cardNumber en">STEP 2</div>

          <div class="cardContent">
            <h3 class="kr">제품 판매 매니저</h3>
            <p class="kr">
              AI를 통한 제품 성격 및 판매 핵심 키워드 생성, 마케팅 포인트 가이드
            </p>
          </div>

          <div class="circle"></div>
        </div>


        <div class="aboutCard cardOrange">
          <div class="cardNumber en">STEP 3</div>

          <div class="cardContent">
            <h3 class="kr">콘텐츠 생성</h3>
            <p class="kr">
              페이지 생성 및 플랫폼 가이드 생성 콘텐츠 이미지, 영상 제공
            </p>
          </div>

          <div class="circle"></div>
        </div>

      </div>

    </div>
  </section>
</template>

<script>
export default {
  name: 'About'
}
</script>

<style scoped>
.about {
  position: relative;
  margin-top: -1px;
  background: #fff;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.about::before {
  content: '';
  position: absolute;
  top: -25px;
  left: 0;
  width: 100%;
  height: 50px;
  background: #fff;
  clip-path: ellipse(55% 100% at 50% 100%);
}

.aboutInner {
  width: min(1400px, 90%);
  margin: 0 auto;
}

/* =========================
   TITLE
========================= */

.aboutTitle {
  text-align: center;
}

.label {
  display: inline-block;
  margin-bottom: 30px;
  font-size: 15px;
  font-weight: 800;
  letter-spacing: 2px;
  color: #999;
}

.aboutTitle h2 {
  margin: 0;
  font-size: 64px;
  font-weight: 800;
  line-height: 1.2;
  letter-spacing: -3px;
  color: #111;
}

.aboutTitle h2 span {
  color: #B7CFFF;
}

.description {
  margin: 30px 0 0;
  font-size: 20px;
  font-weight: 500;
  line-height: 1.7;
  color: #777;
}


/* =========================
   CARDS
========================= */

.aboutCards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
  margin-top: 100px;
}

.aboutCard {
  position: relative;
  height: 380px;
  padding: 40px;
  border-radius: 30px;
  overflow: hidden;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  gap: 120px;
}

.cardPurple {
  background: #F4EAFF;
}

.cardBlue {
  background: #EAF2FF;
}

.cardOrange {
  background: #FFF0E6;
}

.cardNumber {
  position: relative;
  z-index: 2;
  font-size: 30px;
  font-weight: 600;
  color: #000;
}

.cardContent h3 {
  margin: 0;
  font-size: 30px;
  font-weight: 600;
  color: #111;
}

.cardContent p {
  margin: 30px 0 0;
  font-size: 20px;
  font-weight: 500;
  line-height: 1.6;
  color: #666;
  word-break: keep-all;
}


/* =========================
   DECORATION
========================= */

.circle {
  position: absolute;
  width: 220px;
  height: 220px;
  right: -60px;
  top: -60px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.55);
}
</style>