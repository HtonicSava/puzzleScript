<template>
  <div class="home">

  </div>
</template>

<script>
import { user } from '@/plugins/helper.js';

export default {
  name: 'Registery',
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
    this.first_name = 'Test';
    this.last_name = 'Test';
    this.phone = '88005553535';
    this.password = 'test';

    this.login();
  },
  methods: {
    async login() {
      const data = {
        email: this.email,
        first_name: this.first_name,
        last_name: this.last_name,
        phone: this.phone,
        password: this.password
      };

      const res = await user.registery(data);

      console.log(res);
    }
  }
}
</script>