<template>
  <div class="main">
    <Header />
    <div class="mt-4 wrapper">

    </div>

    <modalLogin
      v-model="flag_modal_login"
    />

    <modalRegistery
      v-model="flag_modal_registery"
    />
  </div>
</template>

<script>
import Header from '@/components/header.vue';
import modalLogin from '@/components/Login.vue';
import modalRegistery from '@/components/Registery.vue';

export default {
  name: 'Main',
  data() {
    return {
      flag_modal_login: false,
      flag_modal_registery: false,
    }
  },
  components: {
    Header,

    modalLogin,
    modalRegistery
  },
  methods: {
    toggleModalLogin() {
      this.flag_modal_login = !this.flag_modal_login;
    },
    toggleModalRegistery() {
      this.flag_modal_registery = !this.flag_modal_registery;
    },
  }
}
</script>