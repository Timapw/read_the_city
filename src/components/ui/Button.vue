<template>
  <button class="button">{{name}}</button>
</template>

<script>

export default {
  name: 'ButtonUi',
  components: {
  },
  props: {
    name: {
      type: String,
      default: 'Купить'
    }
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>

.button {
  width: 141px;
  height: 34px;
  color: #ffffff;
  border-radius: 7px;
  background: rgb(50, 120, 255);
  border-color: rgb(50, 120, 255);
  padding: 8px 15px;
  /* Btn */
  font-family: Roboto;
  font-size: 20px;
  font-weight: 500;
  line-height: 22px;
  // letter-spacing: -2%;
  // text-align: center;

}
</style>
