<template>
  <div class="base">
    <Header class="header"></Header>
      <main class="main">
      <Card
        :preview="require('@/assets/images/Skyrim.png')"
        title="Skyrim. История создания великой игры"
        description="Франк Экстанази"
      />
      <Card
        :preview="require('@/assets/images/Search.png')"
        title="Поисковое продвижение сайтов"
        description="Сергей Анисимов"
      />
      <Card
        :preview="require('@/assets/images/Design.png')"
        title="Английский для дизайнеров"
        description="Татьяна Магарина"
      />
      <Card
        :preview="require('@/assets/images/English.png')"
        title="Дизайн и цвет. Практикум"
        description="Шон Адамс"
      />

      </main>
  </div>
</template>
<script>
import Card from '@/components/elements/Card'

export default {
  name: 'MainPage',
  components: {
    Card
  },
  props: {
  },
  setup () {
  }
}
</script>
<style lang="scss" scoped>
* {
  margin: 0;
  padding: 0;
}
.base {
//    background-color: black;
}
.main {
  display: flex;
  justify-content: center;
  padding: 295px 162px 295px;
}
</style>
