<template>
  <div>
    <NavBar />
    <HomeCarousel />
    <Footer />
  </div>
</template>

<script>

export default {
  async created() {
    this.sale_items = await this.$content("products")
      .where({ onSale: true })
      .fetch();
    this.products = await this.$content("products").fetch();
  },
    date() {
        return {
            products: null,
            sale_items: null,
        };
    },
  
}
</script>
