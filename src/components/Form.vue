<template>
  <div class="form__card">
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
        <option value="value1" selected>Выберите направление стажировки</option>
        <option value="value2">Значение 2</option>
        <option value="value3">Значение 3</option>
      </select>
      <button>Отправить заявку на участие</button>
    </form>
  </div>
</template>
<script>
export default {
  name: "RegiS",
};
</script>
<style>
.form__card {
  widows: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 7vw;
}
.form__card form {
  width: 68vw;
  height: max-content;
  background: var(--card-color);
  box-shadow: 4.27751px 8.55502px 0px 0px #fff;
  display: flex;
  align-items: center;
  flex-direction: column;
  row-gap: 2.4vw;
  padding: 3vw 0;
}
.form__card form input {
  width: 28vw;
  padding: 20px 25px;
  background-color: var(--input-color);
  border: none;
  outline: none;
  font-size: 1.4vw;
  color: var(--primary-color);
}
.form__card form input::placeholder {
  font-size: 1.4vw;
  color: var(--primary-color);
}
.form__card form input:first-child {
  margin-right: 2.7vw;
}

.form__card form select {
  width: 59vw;
  height: 60px;
  padding-left: 20px;
  font-size: 1.4vw;
  background-color: var(--input-color);
  border: none;
  color: var(--primary-color);
  outline: none;
}

.form__card form select option {
  border: none;
  outline: none;
  background-color: var(--primary-color);
  color: var(--input-color);
}
.form__card form button {
  width: 59vw;
  height: 60px;
  border: none;
  outline: none;
  background-color: var(--btn-color);
  color: var(--main-bg-color);
  font-size: 1.3vw;
  font-weight: 700;
  letter-spacing: 0.4px;
  box-shadow: 5px 10px 0px 0px #000;
}
</style>
