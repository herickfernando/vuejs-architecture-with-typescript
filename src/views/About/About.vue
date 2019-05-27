<template lang="pug">
  .about
    h1 This is an about page
    input-text(placeholder="Name")
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import InputText from '@/support/commons/components/inputs/input-text.vue';

@Component({
  components: {
    InputText,
  },
})
export default class About extends Vue {}
</script>
