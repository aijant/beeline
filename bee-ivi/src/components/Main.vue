<template>
  <section class="main">
    <div class="main__content">
      <span>Join Us</span>
      <h1>
        A Great Place to <br />
        Receive Care
      </h1>
      <p>
        Medical Recover is most focused in helping you <br />
        discover your most beauiful smile
      </p>
      <div class="main__btn">
        <input class="main__first" type="button" value="Get Quote Now" />
        <input class="main__second" type="button" value="Learn More" />
      </div>
    </div>
    <div class="main__img">
      <img
        src="../assets/hero-8-bg-shape-cover.png"
        alt="hero-8-bg-shape-cover"
      />
    </div>
    <div class="main__items">
      <section class="main__item">
        <img src="../assets/circle sec-1.svg" alt="hero" />
        <h4>Online Appoinment</h4>
        <p>
          The gradual accumulation of information about atomic and small-scale
          behaviour...
        </p>
      </section>
      <section class="main__item">
        <img src="../assets/circle sec-2.svg" alt="hero" />
        <h4>Emergency Case</h4>
        <p>
          The gradual accumulation of information about atomic and small-scale
          behaviour...
        </p>
      </section>
      <section class="main__item">
        <img src="../assets/circle sec-3.svg" alt="hero" />
        <h4>Cancer Care</h4>
        <p>
          The gradual accumulation of information about atomic and small-scale
          behaviour...
        </p>
      </section>
    </div>
  </section>
</template>

<script>
export default {
  name: "Main",
};
</script>

<style scoped lang="scss">
.main {
  position: relative;
  background: #fafafa;

  &__content {
    position: absolute;
    margin: auto 11%;
    margin-top: 5rem;

    span {
      color: #ff685b;
      font-size: 12px;
    }

    h1 {
      font-size: 58px;
      letter-spacing: 0.2px;
      font-weight: bold;
      color: #252b42;
      text-align: left;
      margin: 8rem 0 3rem;
    }

    p {
      color: #737373;
      font-size: 20px;
      font-weight: normal;
      letter-spacing: 0.2px;
    }
  }

  &__btn {
    margin-top: 4rem;
  }

  &__first {
    width: 193px;
    height: 52px;
    background: #ff685b;
    color: #fff;
    border: none;
    border-radius: 5px;
    margin-right: 10px;
  }

  &__second {
    width: 193px;
    height: 52px;
    color: #ff685b;
    background: none;
    border: 1px solid #ff685b;
    border-radius: 5px;
  }

  &__items {
    display: flex;
    justify-content: center;
    transform: translate(0px, -40%);
  }

  &__item {
    box-shadow: 2px 2px 2px 2px rgba(225, 225, 233, 0.034);
    border-radius: 5px;
    background: #fff;
    width: 328px;
    padding: 25px;
    height: auto;
    margin-right: 4%;

    h4 {
      border-bottom: 2px solid #ff685b;
      height: 2rem;
    }

    p {
      margin-top: 2rem;
    }
  }
}
</style>
