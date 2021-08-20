<template>
  <div class="main">
    <Header />

    <div class="mt-4 wrapper">

    </div>

    <modalLogin
      v-model="flag_modal_login"
    />

    <div @click="toggleModalLogin">OpenLogin</div>
  </div>
</template>

<script>
import Header from '@/components/header.vue';
import modalLogin from '@/components/Login.vue';

export default {
  name: 'Main',
  data() {
    return {
      flag_modal_login: false
    }
  },
  components: {
    Header,

    modalLogin,
  },
  methods: {
    toggleModalLogin() {
      this.flag_modal_login = !this.flag_modal_login;
    }
  }
}
</script>