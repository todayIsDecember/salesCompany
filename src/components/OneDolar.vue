<template>
  <div class="dolar__section">
    <div class="dolar__text">
      <div class="title">SMM для початківців</div>
      <div class="article">Курс створений для людей, які хочуть змін!</div>
      <button class="btn">Купити всього за долар</button>
    </div>
    <div class="dolar__photo">
      <div class="dolar__bg">
        <img class="img" src="../../public/photo1.webp" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OneDolar",
};
</script>

<style lang="scss" scoped>
.dolar__section {
  margin: 0;
  padding: 30px 0px;
  display: flex;
  align-items: center;
  max-height: 950px;
  .dolar__text {
    width: 50%;
    .title {
      font-size: 1.9rem;
      font-weight: bold;
      margin-bottom: 10px px;
      font-family: "Montserrat", sans-serif;
    }
    .article {
      margin-top: 0;
      margin-bottom: 1rem;
    }
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
  .dolar__photo {
    .dolar__bg {
      background-color: #f3e68e;
      border-radius: 15px;
      padding: 10% 0;
      .img {
        width: 100%;
        border-radius: 20px;
        margin-left: -50px;
        box-shadow: 2px 2px 10px #ff57229c;
      }
    }
  }
}
</style>
