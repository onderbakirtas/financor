<div class="login">
  <h1 class="login-title">Login.</h1>
  <form class="login-form">
    <input type="text" placeholder="Email">
    <input type="password" placeholder="Password">
    <button>Proceed to login</button>
  </form>
</div>

<style lang="postcss">
  .login {
    @apply p-6 rounded-2xl bg-white w-80;
  }

  .login-title {
    @apply text-3xl text-gray-800 mb-12;
  }

  .login-form {
    @apply flex flex-col w-full;
  }

  input {
    @apply w-full border-0 bg-gray-200 rounded-md block p-3 mb-4 box-border outline-none;
  }

  button {
    @apply block border-0 bg-blue-700 text-white rounded-md text-center py-3 cursor-pointer;
  }

  input, button {
    @apply font-sans;
  }
</style>