<script>
export default {
  data() {
    return {
      priceList: [
        { id: 1, title: 'Бесплатный', amount: '1 сайт', descr: 'Используй свою суперсилу с нашей коллекцией ключевых блоков', price: 'Бесплатно' },
        { id: 2, title: 'Новичок', amount: '3 сайта', descr: 'Используй свою суперсилу и еще ьчето там кого то там', price: 'Платно' },
        { id: 3, title: 'Про', amount: '10 сайтов', descr: 'Для настоящих сайтовщиков бизнесменов и бизнесвуменов Для настоящих сайтовщиков бизнесменов и бизнесвуменов ', price: 'Дорого' },
      ],
      questionList: [
        {
          id: 1,
          question: 'В чем отличие тарифных планов Personal и Business?',
          answer: 'Тарифный план Business включает в себя все то, что есть в плане Personal, плюс позволяет экспортировать код сайтов и создавать до 5 сайтов внутри одного аккаунта(Personal — 1 сайт).'
        },
        {
          id: 2,
          question: 'Можно ли привязать свой домен к сайту, сделанному на Тильде?',
          answer: 'Да. Вы можете использовать свой домен и настроить его привязку к проекту, который сделан на Тильде. Прочитайте инструкцию, как это сделать.'
        },
        {
          id: 3,
          question: 'Подскажите, что понимается под «Экспорт исходного кода» в тарифе Business?',
          answer: 'Экспортируется статичный html плюс все необходимые файлы (картинки, css, js). Сайт пакуется в архиви вам дается ссылка на его скачивание. Просто разархивируйте файлы и скопируйте их к себе на сервер. Вы получите сайт, который будет открываться с вашего сервера и не будет зависим от Тильды. Прочитайте инструкцию, как это сделать.'
        },
        {
          id: 4,
          question: 'Что будет если я не продлю подписку?',
          answer: 'Сайт будет снят с публикации. Данные будут храниться на Тильде в течение 6 месяцев. В любое время вы можете продлить подписку и продолжить вносить изменения в ваш проект. Если по истечении этого срока вы не продлите подписку, данные будут удалены.'
        },
      ],
    }
  },
}

</script>

<template>
  <div class="container">
    <h1>Тарифы: план для каждого</h1>
    <div class="cards-line">
      <div class="tarif-card" v-for="tarif in priceList" :key="tarif.id">
        <img src="@/assets/media/icon1.png" alt="icon" class="tarif-card__icon">
        <h3 class="tarif-card__title">{{ tarif.title }}</h3>
        <h3 class="tarif-card__amount">{{ tarif.amount }}</h3>
        <p class="tarif-card__descr">{{ tarif.descr }}</p>
        <h2 class="tarif-card__price">{{ tarif.price }}</h2>
        <a href=""><button class="tarif-card__btn">Создать сайт</button></a>
      </div>
    </div>
    <div class="faq">
      <div class="faq__block" v-for="qst in questionList" :key="qst.id">
        <span class="faq-question">{{ qst.id }}. {{ qst.question }}</span>
        <p class="faq-answer">{{ qst.answer }}</p>
      </div>
    </div>
  </div>

</template>

<style scoped>
h1 {
  font-weight: 300px;
  font-size: 24px;
  margin-bottom: 40px;
  text-align: center;
}

.container {
  width: 700px;
}

.cards-line {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  width: 100%;
  margin-bottom: 70px;
}

.tarif-card {
  max-width: 210px;
  padding: 20px 20px;
  border: black 1px solid;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
}

.tarif-card__icon {
  height: 69px;
  width: 75px;
  margin-bottom: 15px;
}

.tarif-card__title {
  margin-bottom: 5px;
  font-weight: 300px;
  font-size: 12px;
}

.tarif-card__amount {
  margin-bottom: 17px;
  font-weight: 700;
  font-size: 12px;
}

.tarif-card__descr {
  margin-bottom: 25px;
  font-weight: 300px;
  font-size: 9px;
  flex-grow: 1;
}

.tarif-card__price {
  margin-bottom: 25px;
  font-weight: 300px;
  font-size: 12px;
  margin-top: auto;
}

.tarif-card__btn {
  padding: 5px 15px;
  font-weight: bold;
  font-size: 8px;
  background-color: #E1E1E1;
  border-radius: 28px;
  border: none;
}

a:has(.tarif-card__btn) {
  margin-top: auto;
}

/*  */

.faq {
  padding: 0 20px;
}

.faq__block {
  margin-bottom: 25px;
  font-size: 12px;
}

.faq-question {
  margin-bottom: 22px;
  font-weight: 700;
}
</style>