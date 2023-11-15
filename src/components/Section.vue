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
      <Form />
      <div class="about">
        <div class="about__title">
          <h2>Немного о нас</h2>
          <p>
            Разработка профессиональных информационных систем. Более 20 лет мы
            создаем программные продукты, которые упрощают и оптимизируют
            рабочие процессы каждого.
          </p>
        </div>
        <div class="about__card">
          <div class="card__item">
            <div class="item item_one"></div>
            <div class="item item_two">
              <h3>21+</h3>
              <p>Лет уникального опыта</p>
            </div>
            <div class="item item_three">
              <h3>200+</h3>
              <p>Специалистов</p>
            </div>
            <div class="item item_four">
              <h3>30+</h3>
              <p>Реализованых проектов</p>
            </div>
          </div>
        </div>
      </div>
      <div class="service">
        <div class="service__box">
          <div class="card item_left">
            <div class="card__title">
              <h2>
                Почему <br />
                RealSoft Academy
              </h2>

              <p>
                Мақсадимиз 1 000 000 тажрибали мутахассисларни тайёрлаш.
                Мамлакатимизнинг барча ҳудудларини қамраб олиш. Халқаро миқёсда
                тан олинган сертификатларни тақдим этиш. Чет элда энг талабчан
                IT академияси мақомига эришиш
              </p>
            </div>
            <div class="card__photo">
              <img
                :src="require('../assets/Images/section/ServiceBigImg.png')"
                alt=""
              />
            </div>
          </div>
          <div>
            <div class="card item_right">
              <div
                class="card__desc active"
                v-for="(item, index) in items"
                :key="index"
              >
                <img :src="item.src" alt="" />
                <h4>{{ item.title }}</h4>
                <p>{{ item.desc }}</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import Form from "./Form.vue";

export default {
  name: "SectioN",

  components: {
    Form,
  },
  data() {
    return {
      items: [
        {
          src: require("../../src/assets/Images/section/ServiceIconOne.svg"),
          title: "Гибкая формы обучения",
          desc: "Сиз ўзингиз учун қулай кун ва вақтни танлаш имкониятига эгасиз",
        },
        {
          src: require("../../src/assets/Images/section/ServiceIconTwo.svg"),
          title: "Трудоустройство",
          desc: "После успешного прохождения стаживровки поможем с трудоустройством на работу",
        },
        {
          src: require("../../src/assets/Images/section/ServiceIconThree.svg"),
          title: "Опытные преподователи",
          desc: "Мы предлагаем вам наставников с практическим опытом",
        },
        {
          src: require("../../src/assets/Images/section/ServiceIconFour.svg"),
          title: "Качетсвенное обучение",
          desc: "Мы предлагаем вам наставников с практическим  опытом",
        },
      ],
    };
  },
};
</script>
<style>
section {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin-top: 8vw;
}
/* Section---Title */
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
/* Section---Title */
/* Section---About */
section .about {
  margin-top: 20vw;
}
/* About--title */
section .about .about__title {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  row-gap: 2.2vw;
}
section .about .about__title h2 {
  font-size: 5.5vw;
  letter-spacing: -1.48px;
  color: var(--primary-color);
}
section .about .about__title p {
  max-width: 500px;
  color: var(--primary-color);
  text-align: center;
  font-size: 1.4vw;
}
/* About--title */
/* * */
/* About--Card */
section .about .about__card {
  margin-top: 70px;
}
section .about .about__card .card__item {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  row-gap: 20px;
  margin-bottom: 50px;
}
section .about .about__card .item {
  flex-grow: 1;
  box-shadow: 0px 4.27751px 0px 0px #fff;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  padding-left: 50px;
}
section .about .about__card .item h3 {
  font-size: 6vw;
  color: var(--primary-color);
  font-weight: 400;
  letter-spacing: -1.68px;
}
section .about .about__card .item:nth-child(2) h3 {
  color: var(--main-bg-color);
}
section .about .about__card .item:nth-child(2) p {
  color: var(--main-bg-color);
}
section .about .about__card .item p {
  font-size: 1.6vw;
  color: var(--primary-color);
  font-weight: 400;
  letter-spacing: -1.68px;
}
section .about .about__card .card__item .item:nth-child(1) {
  width: 35vw;
  height: 40vh;
  background-image: url("../assets/Images/section/ItemImgOne.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  box-shadow: 4.27751px 4.27751px 0px 0px #fff;
}
section .about .about__card .card__item .item:nth-child(2) {
  width: 45vw;
  height: 40vh;
  background-image: url("../assets/Images/section/ItemImgTwo.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  margin-left: 15px;
}
section .about .about__card .card__item .item:nth-child(3) {
  width: 45vw;
  height: 40vh;
  background-image: url("../assets/Images/section/ItemImgThree.jpg");
  background-size: cover;
  background-repeat: no-repeat;
}
section .about .about__card .card__item .item:nth-child(4) {
  width: 35vw;
  height: 40vh;
  background-image: url("../assets/Images/section/ItemImgFour.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  margin-left: 10px;
}

/* About--Card */

/* Service--Card */
section .service {
  width: 100%;
  margin-top: 15vw;
}
section .service .service__box {
  display: flex;
  justify-content: space-between;
  color: var(--primary-color);
  /* position: relative; */
}

section .service .service__box .item_left {
  position: relative;
}
section .service .service__box .item_left .card__photo {
  position: absolute;
  left: -100px;
  top: 62%;
}
section .service .service__box .item_left .card__title h2 {
  font-size: 5vw;
  font-weight: 400;
  letter-spacing: -1.48px;
}

section .service .service__box .item_left .card__title p {
  max-width: 580px;
  font-size: 1.3vw;
  font-weight: 400;
  padding-top: 30px;
}

section .service .service__box .item_right {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 20px;
}
section .service .service__box .item_right .card__desc {
  width: 42vw;
  height: 300px;
  background: #282828;
  box-shadow: 5px 5px 0px 0px #4c22c3;
  transition: 0.3s;
  padding-top: 50px;
  padding-left: 40px;
}
section .service .service__box .item_right .card__desc:hover {
  background: #4c22c3;
  box-shadow: 4.28571px 4.28571px 0px 0px #03fe33;
}

section .service .service__box .item_right .card__desc h4 {
  padding-top: 50px;
  font-size: 2vw;
  font-weight: 500;
}
section .service .service__box .item_right .card__desc p {
  max-width: 510px;
  font-size: 20px;
  padding-top: 15px;
  font-weight: 400;
  line-height: 26px;
}
</style>
