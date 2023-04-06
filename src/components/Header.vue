<template>
  <div class="header">
    <div class="header__body">
      <div class="header__logo">
        <img src="../../public/qr.png" alt="" />
      </div>
      <nav class="header__menu" :class="addActiveClassOnMenu">
        <ul class="header__list">
          <li class="list__item"><a href="#">Переваги</a></li>
          <li class="list__item"><a href="#">Ціна</a></li>
          <li class="list__item"><a href="#">Оплата</a></li>
          <li class="list__item"><a href="#">Про нас</a></li>
          <li class="list__item"><a href="#">Контакти</a></li>
        </ul>
      </nav>
      <div
        class="header__burger"
        :class="addActiveClassOnBurger"
        @click="active = !active"
      >
        <span></span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data: () => ({
    active: false,
  }),

  computed: {
    addActiveClassOnBurger() {
      return {
        active__burger: this.active,
      };
    },
    addActiveClassOnMenu() {
      return {
        active__menu: this.active,
      };
    },
  },
};
</script>

<style lang="scss" scoped>
.header {
  margin-top: 10px;
  background-color: #fff;
  height: 80px;
  .header__body {
    height: inherit;
    display: flex;
    justify-content: space-between;
    align-items: center;
    .header__logo {
      position: relative;
      z-index: 50;
      width: 80px;
      height: 80px;
    }
    .header__menu {
      position: relative;
      z-index: 1;
      .header__list {
        display: flex;
        justify-content: flex-end;
        .list__item {
          margin: 0;
          font-size: 16px;
          padding: 0px 5px;
          @media (max-width: 766px) {
            font-size: 20px;
            margin: 0px 20px;
            line-height: 80px;
            border-bottom: 1px solid grey;
          }
          a {
            color: #000;
            &:hover {
              color: #fe7272 !important;
            }
          }
        }
        @media (max-width: 766px) {
          margin-top: 85px;
          flex-direction: column;
        }
      }
      @media (max-width: 766px) {
        position: absolute;
        top: 0px;
        left: -500px;
        height: 100vh;
        background-color: #fff;
        transition: all 300ms ease 0s;
        overflow: auto;
      }
    }
    .active__menu {
      left: 0;
      width: 100%;
    }
    .header__burger {
      display: none;
      @media (max-width: 766px) {
        margin-top: 4px;
        margin-left: 15px;
        display: block;
        position: relative;
        width: 20px;
        z-index: 50;
      }
      span {
        position: absolute;
        background-color: #000;
        left: 0;
        width: 80%;
        height: 2px;
        top: -2px;
        transition: all 0.3s ease 0s;
      }
      &:before,
      &:after {
        content: "";
        background-color: #000;
        position: absolute;
        width: 100%;
        height: 2px;
        left: 0;
        transition: all 0.3s ease 0s;
      }
      &:before {
        top: 3px;
      }
      &::after {
        bottom: 5px;
      }
    }
    .active__burger::before {
      transform: rotate(45deg);
      top: -3px;
    }
    .active__burger::after {
      transform: rotate(-45deg);
      bottom: 1px;
    }
    .active__burger span {
      transform: scale(0);
    }
  }
}
</style>
