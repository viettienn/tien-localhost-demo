<template>
  <div :class="$style.form">
    <h2 :class="$style.createAccount">Create Account</h2>
    <form :class="$style.formFieldsParent">
      <div :class="$style.formFields">
        <div :class="$style.email">
          <input
            :class="$style.emailAddress"
            placeholder="Email address"
            type="text"
          />
          <img :class="$style.iconaccount" alt="" src="/iconaccount.svg" />
        </div>
        <div :class="$style.password">
          <input :class="$style.password1" placeholder="Password" type="text" />
          <img :class="$style.iconpassword" alt="" src="/iconpassword.svg" />
        </div>
        <div :class="$style.confirmPassword">
          <input
            :class="$style.confirmPassword1"
            placeholder="Confirm password"
            type="text"
          />
          <img :class="$style.iconpassword1" alt="" src="/iconpassword.svg" />
        </div>
      </div>
      <button :class="$style.searchFlightsButton">
        <div :class="$style.button">Sign up</div>
      </button>
    </form>
    <div :class="$style.formInner">
      <div :class="$style.frameChild" />
    </div>
    <div :class="$style.orSignUpWithParent">
      <div :class="$style.orSignUp">Or sign up with</div>
      <div :class="$style.facebookbuttonframe">
        <div :class="$style.socialLogindefaultCopy">
          <div :class="$style.facebook">
            <img
              :class="$style.socialIcongm"
              loading="lazy"
              alt=""
              src="/socialicongm.svg"
            />
          </div>
          <div :class="$style.facebook1">Google</div>
        </div>
        <div :class="$style.socialLogindefaultCopy1">
          <img
            :class="$style.facebookIcon"
            loading="lazy"
            alt=""
            src="/facebook.svg"
          />
          <div :class="$style.facebook2">Facebook</div>
        </div>
        <div :class="$style.socialLogindefaultCopy2">
          <img :class="$style.facebookIcon1" alt="" src="/facebook-1.svg" />
          <div :class="$style.facebook3">Apple</div>
        </div>
      </div>
    </div>
    <div :class="$style.iAlreadyHaveContainer">
      <span>I already have an account. </span>
      <span :class="$style.login">Login</span>
    </div>
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "Form",
  });
</script>
<style module>
  .createAccount {
    margin: 0;
    width: 493px;
    position: relative;
    font-size: var(--font-size-7xl);
    letter-spacing: 0.02em;
    font-weight: 700;
    font-family: inherit;
    display: inline-block;
    max-width: 100%;
  }
  .emailAddress {
    width: 104px;
    border: none;
    outline: none;
    font-family: var(--font-archivo);
    font-size: var(--font-size-base);
    background-color: transparent;
    height: 17px;
    position: relative;
    letter-spacing: 0.24px;
    color: var(--light-text);
    text-align: left;
    display: flex;
    align-items: center;
  }
  .iconaccount {
    height: 20px;
    width: 20px;
    position: relative;
    min-height: 20px;
  }
  .email {
    align-self: stretch;
    border-radius: var(--br-9xs);
    background-color: var(--primary-contrast);
    border: 1px solid var(--color-gainsboro);
    overflow: hidden;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    padding: var(--padding-base) var(--padding-xl) var(--padding-mini)
      var(--padding-lg);
    gap: var(--gap-xl);
  }
  .password1 {
    width: 73px;
    border: none;
    outline: none;
    font-family: var(--font-archivo);
    font-size: var(--font-size-base);
    background-color: transparent;
    height: 17px;
    position: relative;
    letter-spacing: 0.24px;
    color: var(--light-text);
    text-align: left;
    display: flex;
    align-items: center;
  }
  .iconpassword {
    height: 20px;
    width: 20px;
    position: relative;
    min-height: 20px;
  }
  .password {
    align-self: stretch;
    border-radius: var(--br-9xs);
    background-color: var(--primary-contrast);
    border: 1px solid var(--color-gainsboro);
    overflow: hidden;
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    justify-content: space-between;
    padding: var(--padding-mini) var(--padding-xl) var(--padding-base)
      var(--padding-lg);
    gap: var(--gap-xl);
  }
  .confirmPassword1 {
    width: 133px;
    border: none;
    outline: none;
    font-family: var(--font-archivo);
    font-size: var(--font-size-base);
    background-color: transparent;
    height: 17px;
    position: relative;
    letter-spacing: 0.24px;
    color: var(--light-text);
    text-align: left;
    display: flex;
    align-items: center;
  }
  .iconpassword1 {
    height: 20px;
    width: 20px;
    position: relative;
    min-height: 20px;
  }
  .confirmPassword {
    align-self: stretch;
    border-radius: var(--br-9xs);
    background-color: var(--primary-contrast);
    border: 1px solid var(--color-gainsboro);
    overflow: hidden;
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    justify-content: space-between;
    padding: var(--padding-mini) var(--padding-xl) var(--padding-base)
      var(--padding-lg);
    gap: var(--gap-xl);
  }
  .formFields {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px 0px 0px;
    gap: 16px 0px;
  }
  .button {
    position: relative;
    font-size: var(--font-size-base);
    letter-spacing: 0.46px;
    line-height: 26px;
    font-weight: 600;
    font-family: var(--font-archivo);
    color: var(--primary-contrast);
    text-align: center;
  }
  .searchFlightsButton {
    cursor: pointer;
    border: none;
    padding: var(--padding-smi) var(--padding-27xl) var(--padding-smi)
      var(--padding-31xl);
    background-color: var(--accent);
    border-radius: var(--br-7xs);
    overflow: hidden;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    white-space: nowrap;
  }
  .searchFlightsButton:hover {
    background-color: var(--color-lightseagreen);
  }
  .formFieldsParent {
    margin: 0;
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-3xs) var(--padding-sm) var(--padding-5xs);
    gap: 27px 0px;
  }
  .frameChild {
    height: 2px;
    flex: 1;
    position: relative;
    border-top: 1.6px solid var(--color-whitesmoke-200);
    box-sizing: border-box;
    max-width: 100%;
  }
  .formInner {
    align-self: stretch;
    height: 14px;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-3xs) var(--padding-sm) var(--padding-5xs);
    box-sizing: border-box;
    max-width: 100%;
  }
  .orSignUp {
    align-self: stretch;
    position: relative;
    letter-spacing: 0.02em;
    line-height: 160%;
  }
  .socialIcongm {
    position: absolute;
    height: 100%;
    width: 100%;
    top: 0%;
    right: 0%;
    bottom: 0%;
    left: 0%;
    max-width: 100%;
    overflow: hidden;
    max-height: 100%;
  }
  .facebook {
    width: 40px;
    height: 40px;
    position: relative;
    border-radius: var(--br-xl);
    overflow: hidden;
    flex-shrink: 0;
  }
  .facebook1 {
    align-self: stretch;
    position: relative;
    letter-spacing: 0.24px;
  }
  .socialLogindefaultCopy {
    flex: 1;
    border-radius: var(--br-5xs);
    background-color: var(--color-whitesmoke-100);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-6xl) var(--padding-smi) var(--padding-7xl);
    box-sizing: border-box;
    gap: 19px 0px;
    min-width: 116px;
  }
  .facebookIcon {
    width: 40px;
    height: 40px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .facebook2 {
    position: relative;
    letter-spacing: 0.24px;
  }
  .socialLogindefaultCopy1 {
    flex: 0.5736;
    border-radius: var(--br-5xs);
    background-color: var(--color-whitesmoke-100);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-6xl) var(--padding-21xl) var(--padding-7xl)
      var(--padding-22xl);
    box-sizing: border-box;
    gap: 19px 0px;
    min-width: 116px;
  }
  .facebookIcon1 {
    width: 40px;
    height: 40px;
    position: relative;
    overflow: hidden;
    flex-shrink: 0;
  }
  .facebook3 {
    align-self: stretch;
    position: relative;
    letter-spacing: 0.24px;
  }
  .socialLogindefaultCopy2 {
    flex: 1;
    border-radius: var(--br-5xs);
    background-color: var(--color-whitesmoke-100);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-6xl) var(--padding-smi) var(--padding-7xl);
    box-sizing: border-box;
    gap: 19px 0px;
    min-width: 116px;
  }
  .facebookbuttonframe {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-11xs) 0px 0px;
    gap: 0px 13px;
    text-align: center;
    color: var(--light-text);
  }
  .orSignUpWithParent {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    padding: 0px var(--padding-5xs) var(--padding-sm);
    gap: 10px 0px;
  }
  .login {
    color: var(--accent);
  }
  .iAlreadyHaveContainer {
    width: 493px;
    position: relative;
    letter-spacing: 0.02em;
    line-height: 160%;
    text-align: center;
    display: inline-block;
    max-width: 100%;
  }
  .form {
    flex: 1;
    background-color: var(--primary-contrast);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-21xl) var(--padding-20xl) var(--padding-20xl);
    box-sizing: border-box;
    gap: 24px 0px;
    max-width: 100%;
    text-align: left;
    font-size: var(--font-size-base);
    color: var(--dark);
    font-family: var(--font-archivo);
  }

  @media screen and (max-width: 750px) {
    .facebookbuttonframe {
      flex-wrap: wrap;
    }

    .form {
      padding-top: var(--padding-7xl);
      padding-bottom: var(--padding-6xl);
      box-sizing: border-box;
    }
  }
  @media screen and (max-width: 450px) {
    .createAccount {
      font-size: var(--font-size-2xl);
    }

    .socialLogindefaultCopy1 {
      flex: 1;
    }
  }
</style>
