<template>
  <div class="main">
    <Header />
    <Description />
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
import Description from '@/components/Description.vue';

export default {
  name: 'Main',
  data() {
    return {
      flag_modal_login: false
    }
  },
  components: {
    Header,
    Description,
    modalLogin,
  },
  methods: {
    toggleModalLogin() {
      this.flag_modal_login = !this.flag_modal_login;
    }
  }
}
</script>