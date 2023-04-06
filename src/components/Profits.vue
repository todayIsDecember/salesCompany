<template>
  <div class="profits">
    <div class="profits__title">Чому потрібно взяти курс саме у нас !</div>
    <div class="profits__container">
      <div class="profits__elem">
        <div class="title">Ціна всього 1 долар</div>
        <div class="article">
          Горнятко кави вартує 1 долар в наш час!<br />
          А зараз за ці кошти ти можеш опанувати нову професію!<br />
          Людина випиває чашку кави в розрізі 1 хвилини до 10, а за годину вже
          не буде навіть про це згадувати.<br />
          А купивши курс можна почати заробляти вдома!<br />
          Роботи стане на всіх!<br />
          Або ж ти можеш зробити свій особистий акаунт професійним, що додасть
          тобі можливості стати блогером та радувати людей
        </div>
      </div>
      <div class="profits__elem">
        <div class="title">
          Над курсом працювали кращі СММ - України та Польші!
        </div>
        <div class="article">
          Отож, одразу цей курс для початківців.<br />
          Так ви пройшовший його можете одразу починати працювати!<br />
          Це не курс якогось відомого блогера, який написав повітря для вас та
          сказав шо він ТОПовий СММ спеціаліст<br />
          Курс створили кращі спеціалісти нашої країни,які налаштовували роботу
          відомих брендів, яких ми не можемо нажаль назвати у звязку з
          конфеденційністю приватної інформації.<br />
          Курс зрозуміє навіть дитинка- тому не зволікай
        </div>
      </div>
      <div class="profits__elem">
        <div class="title">Інші курси в процесі розробки</div>
        <div class="article">
          В близькому часі будуть ще декілька курсів таких як:<br />
          - Курс молодого таргетолога<br />
          - Курс по запуску емейл маркетингу<br />
          - Курс по створенню црм-систес<br />
          - Курс від партнерів Р2Р
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Profits",
};
</script>

<style lang="scss" scoped>
.profits {
  padding: 50px 0px;
  .profits__title {
    text-align: center;
    font-size: 1.9rem;
    font-weight: bold;
    margin-bottom: 30px;
    font-family: "Montserrat", sans-serif;
  }
  .profits__container {
    margin-top: 20px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    .profits__elem {
      width: 30%;
      .title {
        font-size: 1.2rem;
        font-weight: bold;
        margin-bottom: 10px px;
        font-family: "Montserrat", sans-serif;
      }
      .article {
        font-size: 14px;
      }
    }
  }
}
</style>
