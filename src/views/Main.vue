<template>
  <div class="main">
    <Header />
    <Description />
    <Functional />
    <Team />
    <Connect />
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
import Header from '@/components/Header.vue';
import modalLogin from '@/components/Login.vue';
import Description from '@/components/Description.vue';
import Functional from '@/components/Functional.vue';
import Team from '@/components/Team.vue';
import Connect from '@/components/Connect.vue';

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
    Functional,
    Team,
    Connect,
  },
  methods: {
    toggleModalLogin() {
      this.flag_modal_login = !this.flag_modal_login;
    }
  }
}
</script>