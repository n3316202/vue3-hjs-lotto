<template>
  <div class="container">
    <div class="row mt-sm-5">
      <lotto-ball v-for="num in lottoSet" :key="num" :num="num"></lotto-ball>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import LottoBall from '@/components/LottoBall.vue'

export default {
  name: 'LottoView',
  components: {
    LottoBall
  },
  data() {
    return { lottoSet: new Set() }
  },
  created() {
    console.log(typeof this.lottoSet)
    while (this.lottoSet.size != 6) {
      const lottoNum = Math.ceil(Math.random() * 45 + 1)
      this.lottoSet.add(lottoNum)
    }

    for (let temp of this.lottoSet) {
      console.log(temp)
    }
  },
  methods: {}
}
</script>
