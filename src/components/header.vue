<template>
  <div class="header">
       <div class="header__content">
         <div class="header__logo">
           <img src="../assets/img/header/session.png" alt="">
         </div>
         <div class="header__nav">
           <p>Бета-тест</p>
           <p>Принцип работы</p>
           <p>Преимущества</p>
           <p>Команда</p>
         </div>
         <div class="header__social">
           <img src="../assets/img/header/facebook.png" alt="">
           <img src="../assets/img/header/inst.png" alt="">
           <img src="../assets/img/header/twitter.png" alt="">
         </div>
       </div>
  </div>
</template>

<script>
  export default {
    name: 'header',
    data: function () {

    }
     
  }
</script>

<style lang="scss" scoped>
    .header{
        font-family: Roboto;
        font-style: normal;
        font-weight: 500;
        font-size: 24px;
        line-height: 28px;

        color: #3A3A3A;
    }
</style>
