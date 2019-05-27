<template lang="pug">
  input.input(
    name="input"
    :placeholder="placeholder"
  )
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Input extends Vue {
  @Prop() private placeholder!: string;
}
</script>

<style lang="scss">
  .input {
    width: 15vh;
    height: 3vh;
    border: .2vh solid grey;
    border-radius: 1vh;
    font-family: 'Times New Roman', Times, serif;
    font-size: 15px;
    &:focus {
      border: .1vh solid grey;
      box-shadow: .2vh .2vh .3vh;
      outline: none;
    }
  }
</style>
