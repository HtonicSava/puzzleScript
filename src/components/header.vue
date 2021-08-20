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
        background-color: white;
    }

    .header__content{
      max-width: 1280px;
      margin: auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 18px 0px 26px;
    }

    .header__nav{
      display: flex;
      justify-content: space-between;
      flex-grow: 1;
      align-items: center;
      padding: 0px 50px 5px;
      
        p{
          cursor: pointer;
          transition: 0.3s;
          &:hover{
           color: #3B7A20;
          }
          
        }
      
    }

    .header__social{
      img{
        cursor: pointer;
        margin-right: 10px;
        &:last-child {
          margin-right: 0px;
        }
      }
    }
</style>
