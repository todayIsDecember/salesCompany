<template>
  <div class="contacts">
    <div class="contacts__title">Маєш питання звертайся!</div>
    <div class="contacts__article">
      за допомогою нашого бота ти можеш задати нам питання та отримати відповідь
    </div>
    <button class="contacts__btn">Контакти</button>
  </div>
</template>

<script>
export default {
  name: "Contacts",
};
</script>

<style lang="scss" scoped>
.contacts {
  margin-top: 100px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding-top: 30px;
  padding-bottom: 30px;
  background-color: #f3e68e;
  .contacts__title {
    font-size: 1.9rem;
    font-weight: bold;
    margin-bottom: 10px px;
    font-family: "Montserrat", sans-serif;
  }
  .contacts__article {
  }
  .contacts__btn {
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
</style>
