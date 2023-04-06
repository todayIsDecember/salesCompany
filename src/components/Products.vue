<template>
  <div class="products">
    <div class="products__title">Продукти</div>
    <div class="products__container">
      <div class="card">
        <div class="card__header">
          <div class="card__image">
            <img src="../../public/photo2.webp" alt="" />
          </div>
          <div class="card__title">
            Курс СММ для новачків+ СММ копірайт+ Версія ПРО
          </div>
        </div>
        <div class="card__body">
          <div class="card__description">
            -Курс СММ для новачків <br />
            -Курс по створенню тексту(копірайт)<br />
            -Курс запис правильного рісл<br />
            - Контент мейкер<br />
            - Як правильно робити фото
          </div>
          <div class="card__action">
            <button class="btn">10 USD</button>
          </div>
        </div>
      </div>
      <div class="card">
        <div class="card__header">
          <div class="card__image">
            <img src="../../public/photo3.webp" alt="" />
          </div>
          <div class="card__title">СММ для початківців</div>
        </div>
        <div class="card__body">
          <div class="card__description">
            Онлайн-курс в пдф форматі смм для початківців<br />
            В нього входить<br />
            1) Що таке смм<br />
            2) Інструменти з якими працювати<br />
            3) Створення візуалу<br />
            4) Яку роль відіграє рілс<br />
            5) додатки для обробки фото та відео<br />
            6) Створення контент плану<br />
            7) Аналіз цільової аудиторії<br />
            8)Запуск контенту
          </div>
          <div class="card__action">
            <button class="btn">1 USD</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Product",
};
</script>

<style lang="scss" scoped>
.products {
  .products__title {
    font-size: 1.9rem;
    font-weight: bold;
    margin-bottom: 10px;
    font-family: "Montserrat", sans-serif;
    text-align: center;
    margin-bottom: 20px;
  }
  .products__container {
    display: flex;
    justify-content: space-between;
    .card {
      width: 35%;
      border: none;
      font-size: 14px;
      border-radius: 15px;
      box-shadow: 0 2px 16px 0 rgb(92 92 92 / 7%);
      position: relative;
      .card__header {
        border: none;
        text-align: center;
        padding-bottom: 0;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        height: 354.469px;
        .card__image {
          img {
            border-top-left-radius: 15px;
            border-top-right-radius: 15px;
          }
        }
        .card__title {
          margin: 0;
          font-size: 20px;
          font-weight: bold;
          padding: 5px 10px;
        }
      }
      .card__body {
        padding: 10px 20px;
        border-top: 3px solid #ff57229c;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        height: 600px;
        .card__description {
          margin-top: 0;
          line-height: 50px;
          font-size: 14px;
        }
        .card__action {
          text-align: center;
          .btn {
            width: fit-content;
            padding-left: 15%;
            padding-right: 15%;
            color: #fff;
            background-color: #fe7272;
            box-shadow: 2px 2px 10px #ff57229c;
            border: none;
            margin: 15px 0px;
            cursor: pointer;
            font-size: 17px;
            display: inline-block;
            min-height: 40px;
            transition: 0.3s ease 0s;
            &:hover {
              box-shadow: 4px 4px 15px #ff57229c;
              transition: 0.3s ease 0s;
            }
          }
        }
      }
    }
  }
}
</style>
