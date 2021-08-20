<template>
  <div class="home">
    <Menu />
  </div>
</template>

<script>
import axios from '@/service/axios';
import Menu from '@/components/menu.vue';

export default {
  name: 'Login',
  components: {
    Menu
  },
  methods: {
    login() {
      axios.get('https://yandex.ru/')
      .then((res) => {
        console.log(res);
      })
    }
  }
}
</script>