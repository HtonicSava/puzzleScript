<template>
  <div class="home">

  </div>
</template>

<script>
import axios from '@/service/axios';


export default {
  name: 'Login',
  components: {

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