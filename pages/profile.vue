<template>
  <div class="container">
    <p>
      <img :src="avatar" hight="120" width="120">
    </p>
    <p>
      名前 : {{ this.$auth.$state.user.name }}
    </p>
    <p>
      メールアドレス : {{ this.$auth.$state.user.email }}
    </p>
    <button @click="logoutNow">
      ログアウト
    </button>
  </div>
</template>

<script>
export default {
  middleware: 'auth',
  data: function() {
    return {
      avatar: this.$auth.$state.user.picture 
    }
  },
  methods: {
    logoutNow: function() {
      this.$router.push("/logout")
    }
  }
}
</script>
