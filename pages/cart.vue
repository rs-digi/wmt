<template>
  <div>
    <seaction-main :cartItems="cartItems" />
  </div>
</template>

<script>
import SeactionMain from '~/components/SeactionMain.vue'
export default {
  components: { SeactionMain },
  async asyncData(context) {
    const res = await context.app.$axios.$get(
      '/api/shoppingcart/6112f18ffa2baf0015d4340a'
    )
    console.log(res)

    const cartItems = res.DATA
    return { cartItems }
  },
}
</script>

<style></style>
