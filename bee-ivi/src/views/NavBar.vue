<template>
  <section>
    <nav>
      <ul class="navigation">
        <li>
          <router-link to="/">Помощь</router-link>
        </li>
        <li>
          <router-link to="/about">О компании</router-link>
        </li>
        <li>
          <router-link to="/about">Карта офисов</router-link>
        </li>
        <li>
          <router-link to="/about">Акции и новости</router-link>
        </li>
        <li>
          <router-link to="/about">Beeline Рахмат</router-link>
        </li>
      </ul>
      <div class="buttons">
        <a class="btn-ru" href="#">ru</a><span>/</span>
        <a class="btn-kg" href="#">kg</a>
        <a class="btn-per" href="#">Частным лицам</a><span>/</span>
        <a class="btn-bis" href="#">Бизнесу</a>
      </div>
      <router-view />
    </nav>

    <nav>
      <ul class="navigation">
        <li>
          <a href="#"><img src="@/assets/vector.png" alt="vector"/></a>
        </li>
        <li>
          <router-link to="/">Перейти в Билайн </router-link>
        </li>
        <li>
          <router-link to="/">Тарифы</router-link>
        </li>
        <li>
          <router-link to="/">Услуги</router-link>
        </li>
        <li>
          <router-link to="/">Пополнить баланс</router-link>
        </li>
        <li>
          <router-link to="/">Приложения</router-link>
        </li>
        <li>
          <router-link to="/">Еще</router-link>
        </li>
      </ul>
      <button type="button">Войти</button>
      <router-view />
    </nav>
  </section>
</template>

<style lang="scss">
section {
  padding: 0 calc(15% - 15px);
}

nav {
  margin: 30px;

  &::after {
    content: "";
    clear: both;
    display: table;
  }
}

.navigation {
  list-style: none;
  float: left;

  li {
    display: inline-block;
    margin-left: 30px;

    &:first-child {
      margin: 0;
    }
    a {
      text-decoration: none;
      color: $main-color;
    }
  }
}

.btn-ru,
.btn-kg,
.btn-per,
.btn-bis {
  text-decoration: none;
  color: $main-color;

  &:hover {
    background-color: darken($color-secondary, 10%);
  }
}

.btn-kg {
  margin-right: 12px;
}

.btn-ru {
  margin-left: 12px;
}

.btn-per {
  margin-left: 12px;
  padding-left: 8px;
}

.buttons span {
  margin: 4px;
}
</style>
