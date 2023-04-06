<template>
  <div id="app">
    <Header />
    <OneDolar />
    <Profits />
    <Products />
    <Contacts />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import OneDolar from "./components/OneDolar.vue";
import Profits from "./components/Profits.vue";
import Products from "./components/Products.vue";
import Contacts from "./components/Contacts.vue";

export default {
  name: "App",
  components: {
    Header,
    OneDolar,
    Profits,
    Products,
    Contacts,
  },
};
</script>

<style lang="scss">
/* Указываем box sizing */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* Убираем внутренние отступы */
ul[class],
ol[class] {
  padding: 0;
}

/* Убираем внешние отступы */
body,
h1,
h2,
h3,
h4,
p,
ul[class],
ol[class],
li,
figure,
figcaption,
blockquote,
dl,
dd {
  margin: 0;
}

/* Выставляем основные настройки по-умолчанию для body */
body {
  min-height: 100vh;
  scroll-behavior: smooth;
  text-rendering: optimizeSpeed;
  line-height: 1.5;
  font-family: "Montserrat", sans-serif;
}

/* Удаляем стандартную стилизацию для всех ul и il, у которых есть атрибут class*/
ul[class],
ol[class] {
  list-style: none;
}

/* Элементы a, у которых нет класса, сбрасываем до дефолтных стилей */
a {
  text-decoration-skip-ink: auto;
  text-decoration: none;
  color: black;
}

/* Упрощаем работу с изображениями */
img {
  max-width: 100%;
  display: block;
}

/* Указываем понятную периодичность в потоке данных у article*/
article > * + * {
  margin-top: 1em;
}

/* Наследуем шрифты для инпутов и кнопок */
input,
button,
textarea,
select {
  font: inherit;
}

/* Удаляем все анимации и переходы для людей, которые предпочитай их не использовать */
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}
//Імпорт Шрифта
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@300;700&display=swap");
#app {
  max-width: 1170px;
  padding: 0px 15px;
  margin: 0 auto;
}
</style>
