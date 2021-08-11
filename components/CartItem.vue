<template>
  <div class="row">
    <div class="col-md-2">
      <img src="/images/product/1.jpg" class="product-img" />
    </div>
    <div class="col-md-8">
      <p class="product-name">
        {{ item.product_name }}
      </p>
      <p class="in-stock">{{ item.stock_status }}</p>
      <p class="sold-by">
        Sold By <a href="">{{ item.sold_by }}</a>
      </p>
      <p class="gift">Gift options not available. <a href="">Learn more</a></p>
      <select
        class="quantity"
        @change="updateQuantities(item.product_id)"
        v-model="quantity"
      >
        <option
          v-for="qt in item.quantity"
          :key="qt"
          :value="qt"
          :selected="qt == item.quantity"
        >
          Qty:{{ qt }}
        </option>
      </select>
      <button class="cart-btn" @click="deleteItemFromCart(item.product_id)">
        Delete</button
      ><button class="cart-btn" @click="saveForLater(item.product_id)">
        Save For Later</button
      ><button class="cart-btn">See More Like This</button>
    </div>
    <div class="col-md-2">
      <p class="price">&#8377; {{ item.product_price }}</p>
    </div>
    <div class="col-md-12"><hr /></div>
  </div>
</template>

<script>
export default {
  props: ['item'],
  data(props) {
    return {
      quantity: props.item.quantity,
    }
  },
  methods: {
    async deleteItemFromCart(productId) {
      const res = await this.$axios.delete('/api/shoppingcart/' + productId)
      console.log(res)
      alert(res.data.MESSAGE)
    },
    saveForLater(productId) {
      alert('will save for later')
    },
    async updateQuantities(productId) {
      const res = await this.$axios.put('/api/shoppingcart/' + productId, {
        quantity: this.item.quantity,
      })
      alert(res.data.MESSAGE)
    },
  },
}
</script>

<style></style>
