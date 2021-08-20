<template>
  <div class="home">

  </div>
</template>

<script>
import { user } from '@/plugins/helper.js';

import Vue from 'vue';
import VueToast from 'vue-toast-notification';
import 'vue-toast-notification/dist/theme-sugar.css';

Vue.use(VueToast);

export default {
  name: 'Login',
  data() {
    return {
      email: null,
      first_name: null,
      last_name: null,
      phone: null,
      password: null
    }
  },
  components: {
  },
  mounted() {
    this.email = 'test@test.ru';
    this.password = 'test';

    Vue.$toast.success('Тест', {
        position: 'bottom'
    })

    this.login();
  },
  methods: {
    async login() {
      const data = {
        email: this.email,
        password: this.password
      };

      const res = await user.login(data);

      console.log(res);
    }
  }
}
</script>