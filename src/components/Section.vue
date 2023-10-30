<template>
  <div>
    <section>
      <div class="section__title">
        <h1>
          Уникальная
          <img
            class="img1"
            src="../assets/Images/section/TextIconOne.svg"
            alt=""
          />
          IT Стажировка <br />
          <img
            class="img2"
            src="../assets/Images/section/TextIconTwo.svg"
            alt=""
          />
          в ведущей
          <img
            class="img2"
            src="../assets/Images/section/TextIconThee.svg"
            alt=""
          />
          компании
          <img
            class="img2"
            src="../assets/Images/section/TextIconFour.svg"
            alt=""
          />
        </h1>
      </div>
      <div class="section__card">
        <form action="">
          <div
            style="
              display: flex;
              align-items: center;
              justify-content: space-between;
            "
          >
            <input type="text" placeholder="Имя" />
            <input type="tel" placeholder="+998" />
          </div>
          <select name="select">
            <option value="value1" selected>
              Выберите направление стажировки
            </option>
            <option value="value2">Значение 2</option>
            <option value="value3">Значение 3</option>
          </select>
          <button>Отправить заявку на участие</button>
        </form>
      </div>
    </section>
  </div>
</template>
<script>
export default {
  name: "SectioN",
};
</script>
<style>
section {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
section .section__title h1 {
  font-size: 6vw;
  text-align: center;
  letter-spacing: -3px;
  color: var(--primary-color);
  font-weight: 400;
}
section .section__title h1 .img2 {
  height: 65px;
  width: 60px;
}
section .section__card form {
  width: 70vw;
  height: max-content;
  background: var(--card-color);
  box-shadow: 4.27751px 8.55502px 0px 0px #fff;
  display: flex;
  align-items: center;
  flex-direction: column;
}
section .section__card form input {
  width: 25vw;
  padding: 20px 25px;
  background-color: var(--input-color);
  border: none;
  outline: none;
}
</style>
