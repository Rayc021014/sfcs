<template>
  <div class="credentials">
    <span id="email-label">電郵地址或用戶名稱</span>
    <label for="email">
      <input type="text" id="email" placeholder="電郵地址或用戶名稱">
    </label>

    <span id="password-label">密碼</span>
    <label>
      <input type="password" id="password" placeholder="密碼">
    </label>

    <a href="https://accounts.spotify.com/en/password-reset?flow_id=e7a22513-1961-43f7-b049-b507394d9aa5%3A1682456236" id="forgot">忘記密碼?</a>

    <label for="remember-label">
      <input type="checkbox" id="remember-label" checked="checked"><span class="checkmark">記住我</span>
    </label>

    <button id="log-in">登入</button>
  </div>
</template>

<script>
export default {
  name: "Credential"
}
</script>

<style scoped>

</style>