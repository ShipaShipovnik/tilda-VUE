<script setup>

</script>

<template>
  <div class="container">
    <section class="banner">
      <h1 class="h1">Создайте впечатляющий <br>
        сайт на Tilda <span style="font-weight: 300;">для бизнеса и медиа</span></h1>
      <p>550+ профессиональных блоков готовы для вашего сайта и интернет-магазина</p>
      <router-link><button class="banner-btn">Тарифы</button></router-link>
    </section>
    <!--  -->
    <section class="center-infoblock" id="infoblock1">
      <h1 class="h1">Как сделать тысячи людей счастливыми?</h1>
      <p class="main-text">Мы придумали новый способ создания сайтов, где процесс похож на игру. Теперь
        каждый — дизайнер, если есть страсть к любимому делу. Неважно, что вы делаете: сайт
        для бизнеса, лендинг пейдж, интернет-магазин или редакторский спецпроект —
        с Тильдой вы сделаете это быстро и легко.</p>
    </section>
    <!--  -->
    <section class="image-infoblock" id="infoblock2">
      <div class="infoblock__img"><img src="@/assets/media/image 2.png" alt="image2"></div>
      <div class="infoblock__descr">
        <h1 class="">Интуитивный конструктор
          сайтов</h1>
        <p class="main-text">Создание сайта самостоятельно с помощью блоков
          из библиотеки Tilda.
          <br><br>
          Используйте блоки в сотнях комбинаций, просто добавляя один
          за другим, в интуитивно понятном интерфейсе. Вы сможете создать
          сайт своими руками.
        </p>
      </div>
    </section>
    <!--  -->
    <section class="image-infoblock" id="infoblock3">
      <div class="infoblock__descr">
        <h1 class="h1">Библиотека блоков</h1>
        <p class="main-text">Полноэкранные обложки, эффектная типографика,
          фотогалереи, фоновые видео, формы заявок и многое
          другое.
          <br><br>
          Вам не обязательно быть дизайнером. Создано более 550 блоков.
          Каждый из них гармоничен, и в то же время имеет настройки,
          позволяющие создать сайт с индивидуальным дизайном.
        </p>
      </div>
      <div class="infoblock__img"><img src="@/assets/media/image 3.png" alt="image3"></div>
    </section>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 300px;
  font-size: 32px;
  margin-bottom:40px;
}

.banner {
  text-align: center;
}

.banner h1 {
  font-size: 37px;
  font-weight: 600;
}

.banner-btn {
  background-color: #FF9466;
  width: 197px;
  height: 52px;
  margin: 40px 0 70px 0;
  border: none;
  color: white;
  font-size: 14px;
  font-weight: 700;
}

.image-infoblock {
  display: grid;
  height: 400px;
  align-items: center;
}

#infoblock1 {
  text-align: center;
}

#infoblock2 {
  grid-template-columns: 340px auto;
  gap: 83px;
}
#infoblock3 {
  grid-template-columns: auto 340px;
  gap: 24px;
}
</style>
