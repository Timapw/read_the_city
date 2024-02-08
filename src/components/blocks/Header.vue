<template>
  <header class="header">
    <img class="header__logo" src="@/components/icons/Logo2.png" alt="404">
    <div class="header__phone">+7 987 654 32-10</div>
  </header>
</template>
<script>
export default {
  name: 'HeaderPage',
  components: {
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
.header {
/* Navigation */
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 60px;
background: rgb(50, 120, 255);
}
.header__logo {
    position: absolute;
    display: flex;
    justify-content: left;
    top: 16.4px;
    // bottom: 18.35px;
    left: 70px;
}
.header__phone{
    position: absolute;
width: 175px;
height: 26px;
right: 40px;
top: 0;
bottom: 18px;
display: flex;
justify-content: right;
padding-top: 16px;
padding-bottom: 18px;
padding-right: 70px;
color: rgb(255, 255, 255);
font-family: Roboto;
font-size: 22px;
font-weight: 600;
line-height: 26px;
text-align: left;
}
</style>
