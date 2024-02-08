<template>
  <div class="">
    <Header></Header>
    <Main></Main>
 </div>
</template>

<script>
import Header from '@/components/blocks/Header'
import Main from '@/components/blocks/Main'

export default {
  name: 'HomeView',
  components: {
    Header,
    Main
  },
  props: {
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped>

</style>
