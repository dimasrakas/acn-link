<template>
  <div class="p-4 mx-auto max-w-6xl">
    <button
      onclick="location.href='https://app.asiacommerce.net/product/product/163027'"
      href=""
    >
      Web
    </button>
    <button
      onclick="location.href='AsiaCommerce://app.asiacommerce.net/product/product/163027'"
    >
      iOS
    </button>
    <button
      onclick="location.href='https://app.asiacommerce.net/product/product/163027'"
    >
      Android
    </button>
  </div>
</template>

<script>
export default {
  beforeCreate() {
    console.log(this.$device.isMobileOrTablet)

    if (this.$device.isMobileOrTablet) {
      // eslint-disable-next-line nuxt/no-globals-in-created
      window.location.href =
        'AsiaCommerce://app.asiacommerce.net/product/product/163027'
    } else {
      // eslint-disable-next-line nuxt/no-globals-in-created
      window.location.href =
        'https://app.asiacommerce.net/product/product/163027'
    }
  },
}
</script>

<style lang="scss" scoped></style>
