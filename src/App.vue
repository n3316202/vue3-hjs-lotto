<template>
  <body>
    <lotto-header></lotto-header>
    <lotto-main></lotto-main>
    <lotto-footer></lotto-footer>
  </body>
</template>

<script>
import LottoMain from './components/LottoMain.vue'
import LottoHeader from './components/LottoHeader.vue'
import LottoFooter from './components/LottoFooter.vue'

export default {
  name: 'App',
  components: {
    LottoMain,
    LottoHeader,
    LottoFooter
  }
}
</script>

<style scoped>
body {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
</style>
