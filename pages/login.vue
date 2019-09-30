<template>
</template>

<script>
export default {
  created () {
    this.$auth.loginWith('auth0')
  }
}
</script>
