<template>
  <div class="home">
    <div class="page-wrapper">
      <section-header />
      <nuxt />
      <section-footer />
    </div>
  </div>
</template>

<script>
import SectionFooter from '~/components/SectionFooter.vue'
import SectionHeader from '~/components/SectionHeader.vue'
export default {
  components: { SectionHeader, SectionFooter },
}
</script>
