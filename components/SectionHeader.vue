<template>
  <header class="header">
    <div class="header-middle">
      <div class="container">
        <div class="header-left mr-md-4">
          <nuxt-link
            to="/"
            class="mobile-menu-toggle w-icon-hamburger"
          ></nuxt-link>
          <nuxt-link to="/" class="logo ml-lg-0">
            <img src="/images/logo.png" alt="logo" width="145" height="45" />
          </nuxt-link>
          <a href="" class="location ml-lg-0">
            Hello <span>Select Your Address</span>
          </a>
          <form
            method="get"
            action="#"
            class="
              header-search
              hs-expanded hs-round
              d-none d-md-flex
              input-wrapper
            "
          >
            <div class="select-box">
              <select id="category" name="category">
                <option value="">Products</option>
                <option value="">Product 1</option>
                <option value="">Product 2</option>
                <option value="">Product 3</option>
                <option value="">Product 4</option>
                <option value="">Product 5</option>
              </select>
            </div>
            <input
              type="text"
              class="form-control"
              name="search"
              id="search"
              required
            />
            <button class="btn btn-search" type="submit">
              <i class="w-icon-search"></i> Search
            </button>
          </form>
        </div>
        <div class="header-right ml-4">
          <div class="header-call d-xs-show d-lg-flex align-items-center">
            <a href="" class="user-account ml-lg-0">
              Hello, Sign In <span>Account & Lists</span>
            </a>
          </div>
          <a class="wishlist label-down link d-xs-show" href="">
            <img src="images/track.png" width="20" />
            <span class="wishlist-label d-lg-show">Track Orders</span>
          </a>
          <a class="wishlist label-down link d-xs-show" href="">
            <img src="images/help.png" width="20" />
            <span class="compare-label d-lg-show">Help</span>
          </a>
          <nuxt-link class="wishlist label-down link d-xs-show" to="/cart">
            <img src="images/cart.png" width="20" />
            <span class="compare-label d-lg-show">Cart</span>
          </nuxt-link>
        </div>
      </div>
    </div>
    <!-- End of Header Middle -->
    <div
      class="header-bottom sticky-content fix-top sticky-header has-dropdown"
    >
      <div class="container">
        <div class="inner-wrap">
          <div class="header-left">
            <div
              class="dropdown category-dropdown show-dropdown"
              data-visible="true"
            >
              <a
                href="#"
                class="category-toggle"
                role="button"
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="true"
                data-display="static"
                title=""
              >
                <i class="w-icon-category"></i>
                <span>Categories</span>
              </a>
              <div class="dropdown-box" style="display: none">
                <ul class="menu vertical-menu category-menu">
                  <li>
                    <a href=""> Covid Essentials </a>
                  </li>
                  <li>
                    <a href=""> Fitness & Nutrition Supplements </a>
                  </li>
                  <li>
                    <a href=""> Personal Care </a>
                  </li>
                  <li>
                    <a href=""> Diabetic Care </a>
                  </li>
                  <li>
                    <a href=""> Skin Care </a>
                  </li>
                  <li>
                    <a href=""> Baby & Mom Care </a>
                  </li>
                  <li>
                    <a href=""> Women Care </a>
                  </li>
                  <li>
                    <a href=""> Health Care Devices </a>
                  </li>
                  <li>
                    <a href=""> Surgical Equipment </a>
                  </li>
                </ul>
              </div>
            </div>
            <span class="divider d-lg-show"></span>
            <nav class="main-nav">
              <ul class="menu active-underline">
                <li class="active">
                  <a href="">Best Offers</a>
                </li>
                <li class="active">
                  <a href="">Trade Show</a>
                </li>
                <li class="active">
                  <a href="">Personal Protective Equipment</a>
                </li>
                <li class="active">
                  <a href="">Medicine</a>
                </li>
                <li class="active">
                  <a href="">Ask Doctor</a>
                </li>
                <li class="active">
                  <a href="">Covid 19</a>
                </li>
                <li class="active">
                  <a href="">Offer Price</a>
                </li>
                <li>
                  <a href="">Sell on WMT <i class="fa fa-angle-down"></i></a>
                  <ul>
                    <li><a href="">Sell</a></li>
                  </ul>
                </li>
              </ul>
            </nav>
          </div>
          <div class="header-right">
            <span class="divider d-lg-show"></span>
            <div class="dropdown">
              <a href="#" class="currency">English - USD</a>
              <div class="dropdown-box">
                <a href="#USD">English - USD</a>
                <a href="#EUR">English - EUR</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {}
</script>

<style></style>
