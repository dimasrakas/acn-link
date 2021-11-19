<template>
  <div class="p-4 mx-auto max-w-6xl">
    isMobile : {{ $device.isMobileOrTablet }}
  </div>
</template>

<script>
export default {
  beforeCreate() {
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
