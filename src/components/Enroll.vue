<template>
  <div class="footer">
    <hr id="footer-hr">
    <span id="account">未註冊帳戶?</span>
    <button id="sign-up" @click="sign_up()">註冊 SPOTIFY</button>
  </div>
</template>

<script>
export default {
  name: "Enroll",
  methods: {
    sign_up () {
      window.location.assign("https://www.spotify.com/tw/signup?flow_id=a4ed0182-7296-43f2-8af0-2e2efbfbabd6%3A1682459394&forward_url=https%3A%2F%2Fopen.spotify.com%2F%3Fflow_id%3Da4ed0182-7296-43f2-8af0-2e2efbfbabd6%253A1682459394");
    }
  }
}
</script>

<style scoped>

</style>