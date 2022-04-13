<template>
  <div class="header">
    <div class="header__logo">
      <img src="../../assets/img/video_logo.png" alt="" />
      <h1 class="title">{{ title }}</h1>
    </div>
    <div class="header__search">
      <input
        class="input__search-video"
        placeholder="Введите название для поиска"
        type="search"
        name="input_search"
      />
    </div>
    <div class="header__controls">
      <button class="buttons">
        <img src="../../assets/img/contacts.png" title="Контакты" alt="img" />
      </button>
      <button class="buttons">
        <img src="../../assets/img/support.png" alt="img" title="Поддержка" />
      </button>
      <button class="buttons">
        <img src="../../assets/img/bell.png" alt="img" title="Уведомления" />
      </button>
      <button class="buttons">
        <img src="../../assets/img/loginOut.png" alt="img" title="Вход/Выход" />
      </button>
    </div>
  </div>
</template>
<script>
export default {
  name: "header-component",
  data() {
    return {
      title: "RUMEDIA",
    };
  },
};
</script>
<style lang="scss">
.header {
  height: 60px;
  display: flex;
  justify-content: space-between;
  flex-basis: 33.334%;

  .header__logo {
    display: flex;
    align-items: center;
    .title {
      margin-left: 5px;
      color: rgb(12, 116, 235);
    }
  }
  .header__search {
    display: flex;
    justify-content: center;
    align-items: center;
    .input__search-video {
      width: 500px;
      height: 30px;
      padding: 5px;
      border: none;
      box-shadow: 1px 1px 1px 1px grey;
      border-radius: 5px;
    }
  }
  .header__controls {
    display: flex;
    align-items: center;
    justify-content: space-between;
    .buttons {
      margin-right: 5px;
      padding: 2px;
      border: none;
      cursor: pointer;
      background-color: white;
    }
    button:last-child {
      margin-left: 20px;
    }
  }
}
</style>
