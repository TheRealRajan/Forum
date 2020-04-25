<template>
  <div class="wrapper">
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512">
      <path
        d="M328 0h-16a16 16 0 0 0-16 16v480a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16V16a16 16 0 0 0-16-16zm-96 96h-16a16 16 0 0 0-16 16v288a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16V112a16 16 0 0 0-16-16zm192 32h-16a16 16 0 0 0-16 16v224a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16V144a16 16 0 0 0-16-16zm96-64h-16a16 16 0 0 0-16 16v352a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16V80a16 16 0 0 0-16-16zM136 192h-16a16 16 0 0 0-16 16v96a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16v-96a16 16 0 0 0-16-16zm-96 32H24a16 16 0 0 0-16 16v32a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16v-32a16 16 0 0 0-16-16zm576 0h-16a16 16 0 0 0-16 16v32a16 16 0 0 0 16 16h16a16 16 0 0 0 16-16v-32a16 16 0 0 0-16-16z"
      />
    </svg>

    <div class="forgot-password">
      <span class="header">Forgot Password</span>
      <p class="reset-info">
        Uh oh ! We know that feeling. Just enter the
        <span class="text-emphasis">Email Address</span> you registered with and
        we will send you a
        <span class="text-emphasis">link</span> to reset your
        password right away.
      </p>
      <form action="post">
        <input type="text" placeholder="Your Email" />
        <button type="submit">Send Password Reset Link</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "ForgotPassword"
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin: auto auto;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background: $almostWhite;
  svg {
    height: 3rem;
    width: 3rem;
    fill: $primaryBlue;
    margin-bottom: 2rem;
  }
}
.forgot-password {
  width: 22vw;
  border-radius: 5px;
  background: $white;
  box-shadow: 1px 8px 10px 2px $kindaWhite;
  //   margin: auto auto;
  padding: 3em 2em;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.header {
  font-size: 1.3rem;
  color: $kindaWhite;
  font-weight: 600;
  text-align: center;
}
.reset-info {
  font-size: 0.8rem;
  color: $lightText;
  margin-top: 2em;
}
.text-emphasis {
  font-weight: 600;
}
form {
  display: flex;
  flex-direction: column;
  width: 100%;
  margin: 1em 0;
  //   justify-content: space-around;

  input {
    padding: 0.5em 0.8em;
    font-family: "Manrope";
    margin-bottom: 2.5em;
    border-radius: 5px;
    border: 1px solid $kindaWhite;
    &::placeholder {
      font-size: 0.75rem;
      color: $lightText2;
    }
  }

  button {
    background: $purple;
    font-size: 0.75rem;
    color: #fff;
    border: none;
    border-radius: 5px;
    padding: 0.75em 0;
    cursor: pointer;
    text-align: center;
    box-shadow: 0px 1px 10px 2px $cardShadow;
    &:hover {
      box-shadow: 1px 1px 5px $purple;
      transition: linear 0.2s;
    }
  }
}
</style>
