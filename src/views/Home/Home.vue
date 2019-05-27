<template lang="pug">
  .home
    img(alt='Vue logo', src='@/assets/logo.png')
    hello-world(msg='Welcome to Your Vue.js + TypeScript App')
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import HelloWorld from '@/views/Home/components/HelloWorld.vue';

@Component({
  components: {
    HelloWorld,
  },
})
export default class Home extends Vue {}
</script>
