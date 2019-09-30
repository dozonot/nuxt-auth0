<template>
  <p>
    すでにログアウトしています。<nuxt-link to="/">Homeへ戻る</nuxt-link>
  </p>
</template>

<script>
export default {
  created () {
    this.$auth.logout()
  }
}
</script>
