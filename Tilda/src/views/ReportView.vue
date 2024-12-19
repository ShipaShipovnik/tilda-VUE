<script setup>

</script>

<template>
  <div class="container">
    <h1>Сообщить о нарушении</h1>
    <p>Tilda Publishing — программное обеспечение, с помощью которого пользователи создают сайты и размещают на них
      контент. Администрация Tilda Publishing не несет ответственности за содержимое сайтов пользователей.
      <br>
      Если вы считаете, что пользователь Tilda Publishing нарушает ваши права, отправьте нам сообщение через форму.
    </p>
    <form>
      <label for="">Ваш e-mail</label>
      <input type="email" placeholder="Оставьте ваш email, чтобы мы могли с вами связаться  ">
      <label for="">Ваше имя</label>
      <input type="text" placeholder="Пожалуйста, напишите вашем имя и фамилию">
      <label for="">Ссылка на сайт</label>
      <input type="text" placeholder="Укажите ссылку на сайт, на который вы хотите пожаловаться">
      <label for="">Комментарий</label>
      <input type="text" placeholder="Опишите нарушение">
      <button type="submit">Отправить</button>
    </form>
  </div>
</template>

<style scoped>
.container {
  width: 530px;
}

h1 {
  margin-bottom: 30px;

  font-size: 24px;
  text-align: center;
}

p {
  margin-bottom: 30px;
  font-size: 12px;
}

form {
  width: 100%;
}

input,
label {
  display: block;
  width: 100%;
}
label{
  margin-bottom:6px
}

input {
  height: 50px;
  border: 1px solid black;
  background-color: white;
  color: #838383;
  padding: 13px 19px;
  margin-bottom: 20px;
}

button {
  padding: 20px 65px;
  background: black;
  border: none;
  color: white;
  display: flex;
  justify-self: center;
  margin-top: 30px;
  transition: transform .2s;
}

button:hover {
  cursor: pointer;
  /* IE 9 */
  -webkit-transform: scale(1.1);
  /* Safari 3-8 */
  transform: scale(1.1);
}
</style>
