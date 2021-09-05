<template>
  <section class="menu">
    <nav>
      <ul class="menu__links">
        <li>
          <span>MedicalRecover</span>
        </li>
        <li>
          <router-link to="/#">Home</router-link>
        </li>
        <li>
          <router-link to="/#">Product</router-link>
        </li>
        <li>
          <router-link to="/#">Pricing</router-link>
        </li>
        <li>
          <router-link to="/#">Content</router-link>
        </li>
      </ul>
      <router-view />
    </nav>
    <section class="menu__btn">
      <input class="menu__login" type="button" value="Login" />
      <input class="menu__join-us" type="button" value="Join us" />
    </section>
  </section>
</template>

<style lang="scss" scoped>
.menu {
  display: flex;
  justify-content: space-around;
  background: #fafafa;

  &__links {
    display: flex;
    list-style: none;
    margin-top: 13px;

    &:first-child {
      color: #000;
      font-size: 20px;
      font-weight: bold;
    }

    a {
      text-decoration: none;
      color: #000;
      font-size: 14px;
      font-weight: normal;
      margin: 33px 34px;
    }
  }

  &__btn {
    margin-top: 7px;
  }

  &__login {
    margin-right: 45px;
    color: #FF685B;
    border: none;
    background: none;
  }

  &__join-us {
    color: #fff;
    background: #FF685B;
    width: 137px;
    height: 52px;
    border-radius: 5px;
    padding: 15px 25px;
    border: none;
    text-transform: uppercase;
  }
}
</style>
