<template>
  <div class="card">
    <img class="card__preview" :src="preview" alt="">
    <h2 class="card__name">{{ title }}</h2>
    <p class="card__description">{{ description }}</p>
    <ButtonCard />
    <!-- <button class="card__button">Купить</button> -->
  </div>
</template>
<script>

import ButtonCard from '@/components/ui/Button.vue'

export default {
  name: 'CardElement',
  components: {
    ButtonCard
  },
  props: {
    preview: {
      type: String,
      default: ''
    },
    title: {
      type: String,
      default: ''
    },
    description: {
      type: String,
      default: ''
    }
  },
  setup () {
  }
}
</script>
<style lang="scss" scoped>
.card {
  position: static;
  width: 330px;
  height: 490px;
  display: flex;
  flex-direction: column;
  align-items: center;
  border-radius: 10px;
  box-shadow: 1px 1px 4px 0px rgba(0, 0, 0, 0.3);
  background: rgb(255, 255, 255);
  padding-bottom: 24px;
  margin: 0px 26px;
}
.card__preview {
  /* image 1 */
  padding: 17px;
}
.card__name {
  /* Skyrim. История создания великой игры */
  position: static;
  width: 293px;
  height: 56px;
  /* Автолейаут */
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  // padding: 0px;
  /* Inside Auto Layout */
  flex: none;
  order: 0;
  flex-grow: 0;
  margin: 14px 0px;
  text-align: center;
  color: rgb(0, 0, 0);
  font-family: Roboto;
  font-size: 24px;
  font-weight: 400;
  line-height: 28px;
  letter-spacing: 0%;
  text-align: center;
}

.card__description {
  /* Сергей Анисимов */
  color: rgb(0, 0, 0);
  font-family: Roboto;
  font-size: 20px;
  font-weight: 400;
  line-height: 23px;
  letter-spacing: 0%;
  text-align: left;
}
</style>
