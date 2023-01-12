<template>
  <div class="col-lg-2 mt-3 d-flex justify-content-around">
    <svg
      class="rounded-circle"
      margin="30"
      width="140"
      height="140"
      focusable="false"
    >
      <rect width="100%" height="100%" :fill="getColor()" />
      <text
        text-anchor="middle"
        x="50%"
        y="50%"
        fill="white"
        dy=".3em"
        font-size="60"
      >
        {{ num }}
      </text>
    </svg>
  </div>
</template>

<script>
export default {
  name: 'LottoBall',
  props: {
    num: Number
  },
  created() {},
  methods: {
    getColor() {
      let color = 'black'
      //   if (this.num > 0 && this.num <= 0) {
      //     color = 'gold'
      //   } else if (this.num > 10 && this.num <= 20) {
      //     color = 'green'
      //   } else if (this.num > 20 && this.num <= 30) {
      //     color = 'gray'
      //   } else if (this.num > 30 && this.num <= 40) {
      //     color = 'black'
      //   } else color = 'black'
      //   console.log(color)
      return color
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
