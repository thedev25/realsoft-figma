<template>
  <div>
    <header>
      <nav>
        <div class="nav__logo">
          <img src="../assets/Images/Header/MainLogo.svg" alt="RealSoft-Logo" />
        </div>
        <div class="nav__lang">
          <img
            src="../assets/Images/Header/langunageLogo.svg"
            alt="GlobusLogo"
          />
          <ul>
            <li>Русский</li>
          </ul>
          <img src="../assets/Images/Header/SelectIconLogo.svg" alt="arrows" />
        </div>
        <ol>
          <li>О нас</li>
          <li>Почему мы</li>
          <li>Стоимость</li>
          <li>Контакты</li>
        </ol>
        <div class="nav__phone">
          <span>+998 (99) 220 84 84 </span>
        </div>
        <div class="nav__btn">
          <button>Отправить заявку</button>
        </div>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
};
</script>

<style>
header {
  width: 100%;
  padding-top: 30px;
  padding-bottom: 20px;
  border-bottom: 1px solid #414141;
}
nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: var(--primary-color);
}
nav .nav__lang {
  display: flex;
  align-items: center;
  justify-content: center;
  column-gap: 8px;
}
nav .nav__lang li {
  font-size: 1.3vw;
  font-weight: 800;
}
nav ol {
  display: flex;
  align-items: center;
  justify-content: space-between;
  column-gap: 1.6vw;
}
nav ol li {
  font-size: 1.3vw;
  font-weight: 400;
}
nav .nav__phone span {
  font-size: 1.3vw;
  font-weight: 700;
}
nav .nav__btn button {
  padding: 1.5vw 3.5vw;
  outline: none;
  border: none;
  background-color: var(--input-color);
  color: var(--primary-color);
  font-size: 1.2vw;
  font-weight: 700;
}
</style>
