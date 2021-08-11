<template>
  <main class="main">
    <div class="container">
      <div class="cart">
        <div class="row">
          <!-- cart left -->
          <div class="col-md-9 mb-4">
            <div class="bg-white cart-panel">
              <h2>Shopping Cart <span>Price</span></h2>

              <!-- item start -->
              <div v-for="item in cartItems" :key="item.product_id">
                <cart-item :item="item" />
              </div>
              <!-- item end -->

              <div class="row">
                <div class="col-md-12">
                  <p class="sub-total">
                    Sub Total (4 Items):
                    <span class="price">&#8377; 5333.00</span>
                  </p>
                </div>
              </div>
            </div>
          </div>

          <!-- cart right -->
          <div class="col-md-3">
            <div class="row">
              <div class="col-md-12 col-xs-6 mb-4">
                <div class="bg-white cart-panel-right-protection">
                  100% Purchase Protection
                  <span>Original Products | Secure Payment</span>
                </div>
              </div>
              <div class="col-md-12 col-xs-6 mb-4">
                <div class="bg-white cart-panel-right-detail">
                  <p class="detail">
                    <img src="/images/check.png" />Part of your order qualifies
                    for FREE Delivery. Select this option at checkout.
                    <span>Details</span>
                  </p>
                  <p class="sub-total">
                    Sub Total ( 4 Items ) :
                    <span class="price">&#8377; 5333.00</span>
                  </p>
                  <input type="checkbox" name="" /> This order contains a gift
                  <button type="submit" name="">Proceed To Buy</button>
                  <select name="">
                    <option value="" selected>EMI Available</option>
                  </select>
                </div>
              </div>
              <div class="col-md-12 col-xs-6 mb-4">
                <div class="bg-white cart-panel-right-sponsored">
                  <h2>Sponsored Products related to items in your cart</h2>
                  <!-- item -->
                  <div class="row mb-4">
                    <div class="col-md-4">
                      <img src="/images/product/5.jpg" class="product-img" />
                    </div>
                    <div class="col-md-8">
                      <p class="product-name">Fast&Up 100%…</p>
                      <p class="rating">
                        <i class="fa fa-star yellow"></i
                        ><i class="fa fa-star yellow"></i
                        ><i class="fa fa-star yellow"></i
                        ><i class="fa fa-star yellow"></i
                        ><i class="fa fa-star gray"></i>
                      </p>
                      <p class="price">&#8377; 1999.00</p>
                      <a href="" class="buying">See all buying options</a>
                    </div>
                  </div>
                  <!-- item end -->

                  <!-- item -->
                  <div class="row mb-4">
                    <div class="col-md-4">
                      <img src="/images/product/6.jpg" class="product-img" />
                    </div>
                    <div class="col-md-8">
                      <p class="product-name">Horlicks Health &…</p>
                      <p class="rating">
                        <i class="fa fa-star yellow"></i
                        ><i class="fa fa-star yellow"></i
                        ><i class="fa fa-star yellow"></i
                        ><i class="fa fa-star yellow"></i
                        ><i class="fa fa-star gray"></i>
                      </p>
                      <p class="price">&#8377; 412.00</p>
                      <a href="" class="buying">See all buying options</a>
                    </div>
                  </div>
                  <!-- item end -->

                  <!-- item -->
                  <div class="row">
                    <div class="col-md-4">
                      <img src="/images/product/7.jpg" class="product-img" />
                    </div>
                    <div class="col-md-8">
                      <p class="product-name">MuscleBlaze Biozyme…</p>
                      <p class="rating">
                        <i class="fa fa-star yellow"></i
                        ><i class="fa fa-star yellow"></i
                        ><i class="fa fa-star yellow"></i
                        ><i class="fa fa-star yellow"></i
                        ><i class="fa fa-star gray"></i>
                      </p>
                      <p class="price">&#8377; 4499.00</p>
                      <a href="" class="buying">See all buying options</a>
                    </div>
                  </div>
                  <!-- item end -->
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
import CartItem from '~/components/CartItem.vue'
export default {
  components: { CartItem },

  props: ['cartItems'],
}
</script>

<style></style>
