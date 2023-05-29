<template>
  <div class="buttons">
    <button id="facebook" class="app-buttons" @click="clickFacebook()">
      <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor" class="bi bi-facebook"
           viewBox="0 0 16 16">
        <path
            d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z" />
      </svg>
      <span>&emsp;使用 FACEBOOK 帳戶繼續</span>
    </button>
    <button id="apple" class="app-buttons" @click="clickApple()">
      <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor" class="bi bi-apple"
           viewBox="0 0 16 16">
        <path
            d="M11.182.008C11.148-.03 9.923.023 8.857 1.18c-1.066 1.156-.902 2.482-.878 2.516.024.034 1.52.087 2.475-1.258.955-1.345.762-2.391.728-2.43Zm3.314 11.733c-.048-.096-2.325-1.234-2.113-3.422.212-2.189 1.675-2.789 1.698-2.854.023-.065-.597-.79-1.254-1.157a3.692 3.692 0 0 0-1.563-.434c-.108-.003-.483-.095-1.254.116-.508.139-1.653.589-1.968.607-.316.018-1.256-.522-2.267-.665-.647-.125-1.333.131-1.824.328-.49.196-1.422.754-2.074 2.237-.652 1.482-.311 3.83-.067 4.56.244.729.625 1.924 1.273 2.796.576.984 1.34 1.667 1.659 1.899.319.232 1.219.386 1.843.067.502-.308 1.408-.485 1.766-.472.357.013 1.061.154 1.782.539.571.197 1.111.115 1.652-.105.541-.221 1.324-1.059 2.238-2.758.347-.79.505-1.217.473-1.282Z" />
        <path
            d="M11.182.008C11.148-.03 9.923.023 8.857 1.18c-1.066 1.156-.902 2.482-.878 2.516.024.034 1.52.087 2.475-1.258.955-1.345.762-2.391.728-2.43Zm3.314 11.733c-.048-.096-2.325-1.234-2.113-3.422.212-2.189 1.675-2.789 1.698-2.854.023-.065-.597-.79-1.254-1.157a3.692 3.692 0 0 0-1.563-.434c-.108-.003-.483-.095-1.254.116-.508.139-1.653.589-1.968.607-.316.018-1.256-.522-2.267-.665-.647-.125-1.333.131-1.824.328-.49.196-1.422.754-2.074 2.237-.652 1.482-.311 3.83-.067 4.56.244.729.625 1.924 1.273 2.796.576.984 1.34 1.667 1.659 1.899.319.232 1.219.386 1.843.067.502-.308 1.408-.485 1.766-.472.357.013 1.061.154 1.782.539.571.197 1.111.115 1.652-.105.541-.221 1.324-1.059 2.238-2.758.347-.79.505-1.217.473-1.282Z" />
      </svg>
      <span>&emsp;使用 APPLE 帳戶繼續</span>
    </button>
    <button id="google" class="app-buttons" @click="clickGoogle()">

      <img src="src/images/google.png" alt="google-icon" class="icons">
      <span>&emsp;以 GOOGLE 帳戶繼續</span>
    </button>
  </div>
</template>

<script>
export default {
  name: "OtherLogin",
  methods: {
    clickGoogle () {
      window.location.assign("https://accounts.google.com/o/oauth2/v2/auth/oauthchooseaccount?response_type=code&access_type=offline&client_id=1046568431490-ij1gi5shcp2gtorls09frkc56d4mjbe2.apps.googleusercontent.com&state=AQDCLxn143bdsDXY%2Fs8Pn68fnkhfaEpjV%2Bf5RRxbA%2F3LoRfld0ZMT0pqyXXxyDPzAtwouN1dpNzrufP7vU7HJQqaep5MoXlfCLIRzTELOqwd01SAChzQRg52M8eQUXJ5zpjT9kQ3Uxt%2Bphd8Spmk7DCeXCln6A4RfomkgvrVvW8WhXBWbtmij08%2BQpJ686mYBFRJ3Z8%2BaZaKVjuq3tx99i4S15RMH8FAjVWWdXqj5EFHOvK7u0eveQFgMcQjDiyEyHELk4%2B5Bd2bUEXGTdUEE2%2B1jK%2BpV7FhRB3VYBGl7FRovf%2FNCqc7Cjjv8r3QtQXTK8lzYvkVP59hHTtJNOnBGcBbkCX1S3B9&scope=profile%20email%20openid&redirect_uri=https%3A%2F%2Faccounts.spotify.com%2Flogin%2Fgoogle%2Fredirect&service=lso&o2v=2&flowName=GeneralOAuthFlow");
    },

    clickApple () {
      window.location.assign("https://appleid.apple.com/auth/authorize?client_id=com.spotify.accounts&response_type=code&response_mode=form_post&scope=name%20email&state=AQAO4Nv8psH8fAc0E7zFQvTJKJDlYmeYh0tl6zpmtES7Gsujx9dKGalJ38eJjzxYUroOXggQE1h0gbTAkYJycoo7tSGsOQ83BDWReBXGlAMBUUfaUSD%2B0emzD%2BwDx%2BI7gZ96s3yvlZtHEghzUyw%2FSFy%2BdHURfTcPXiRpNko2E0LN5LB8%2BSaQwmFHZ%2FoQeZ2%2FF5BPOoIhQ%2BlHdSU%2F0nFdygEp5iWbNx6OyV3Mkl%2FLr8FpM4R1N2GMfBOBUFNhcGhNd2VIkbgwZ%2BlpN1iX%2Bw%3D%3D&redirect_uri=https%3A%2F%2Faccounts.spotify.com%2Flogin%2Fapple%2Fredirect");
    },

    clickFacebook () {
      window.location.assign("https://www.facebook.com/login.php?skip_api_login=1&api_key=174829003346&kid_directed_site=0&app_id=174829003346&signed_next=1&next=https%3A%2F%2Fwww.facebook.com%2Fv7.0%2Fdialog%2Foauth%3Fclient_id%3D174829003346%26state%3DAQB5pnMdIRHjCItM8blnzq%252Fb60gu0QSmuFIK8sOXNn%252BtvCj1iCd3BqawJoVzozgNhi8RtZsgpOkjb4CABZF84afhS%252FMoz0LCHZf6fGP%252BigNZADkiYhZ7gE8gcLawvxs3NheRSShO7M9Q68iBSx0Z6opizwpWVFtszWy0yfv2jIJpZ4v6U0pU5R8%252FH%252BQUVKDpspaGN9t%252BENCNYd%252F0P3TUbqTctB6Haaiws3UnCuYyadBI5klQJ%252BsDKEIlezqg759jTHqYTgpB9%252BA0jmOZSLRnf2OQ46wEbJXC8HAl2WQvWePttNic0zSQVKDjHL2bGJSaNTspdu3%252FrdkQbxm0FBnmtqsKy5psyq%252By%26redirect_uri%3Dhttps%253A%252F%252Faccounts.spotify.com%252Flogin%252Ffacebook%252Fredirect%26ret%3Dlogin%26fbapp_pres%3D0%26logger_id%3D20d9dd51-bb1e-4bbb-84f1-4dae296cbb93%26tp%3Dunspecified&cancel_url=https%3A%2F%2Faccounts.spotify.com%2Flogin%2Ffacebook%2Fredirect%3Ferror%3Daccess_denied%26error_code%3D200%26error_description%3DPermissions%2Berror%26error_reason%3Duser_denied%26state%3DAQB5pnMdIRHjCItM8blnzq%252Fb60gu0QSmuFIK8sOXNn%252BtvCj1iCd3BqawJoVzozgNhi8RtZsgpOkjb4CABZF84afhS%252FMoz0LCHZf6fGP%252BigNZADkiYhZ7gE8gcLawvxs3NheRSShO7M9Q68iBSx0Z6opizwpWVFtszWy0yfv2jIJpZ4v6U0pU5R8%252FH%252BQUVKDpspaGN9t%252BENCNYd%252F0P3TUbqTctB6Haaiws3UnCuYyadBI5klQJ%252BsDKEIlezqg759jTHqYTgpB9%252BA0jmOZSLRnf2OQ46wEbJXC8HAl2WQvWePttNic0zSQVKDjHL2bGJSaNTspdu3%252FrdkQbxm0FBnmtqsKy5psyq%252By%23_%3D_&display=page&locale=zh_TW&pl_dbl=0");
    }
  }
}
</script>

<style scoped>

</style>