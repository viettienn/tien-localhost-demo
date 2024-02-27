<template>
  <div :class="$style.signUpPage">
    <Component />
    <main :class="$style.loginSections">
      <div :class="$style.formWrapper"><form /></div>
    </main>
    <footer :class="$style.footer">
      <div :class="$style.privacypolicyframe">
        <div :class="$style.copyrightnotice">
          <div :class="$style.localhostIncAll">
            © 2023 Localhost, Inc. All Rights Reserved
          </div>
          <div :class="$style.termsandconditionstext">
            <div :class="$style.privacyPolicy">Privacy Policy</div>
            <div :class="$style.termsConditions">Terms & Conditions</div>
            <div :class="$style.contactUs">Contact us</div>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>
<script lang="ts">
  import { defineComponent } from "vue";
  import Component from "../components/Component.vue";
  import Form from "../components/Form.vue";

  export default defineComponent({
    name: "SignUpPage",
    components: { Component, Form },
  });
</script>
<style module>
  .formWrapper {
    width: 589px;
    border-radius: var(--br-5xs);
    overflow: hidden;
    flex-shrink: 0;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    max-width: 100%;
  }
  .loginSections {
    align-self: stretch;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    padding: var(--padding-150xl) var(--padding-150xl) 170px;
    box-sizing: border-box;
    background-image: url("/public/login-sections@3x.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: top;
    max-width: 100%;
  }
  .localhostIncAll {
    position: relative;
    line-height: 120%;
    font-weight: 300;
  }
  .privacyPolicy {
    position: relative;
    line-height: 120%;
    font-weight: 300;
  }
  .termsConditions {
    position: relative;
    line-height: 120%;
    font-weight: 300;
  }
  .contactUs {
    position: relative;
    line-height: 120%;
    font-weight: 300;
  }
  .termsandconditionstext {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: 0px 20px;
  }
  .copyrightnotice {
    flex: 1;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: space-between;
    max-width: 1280px;
    gap: var(--gap-xl);
  }
  .privacypolicyframe {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    max-width: 1280px;
  }
  .footer {
    align-self: stretch;
    border-top: 1px solid var(--light-grey-border);
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: 12px 30px;
    max-width: 100%;
    text-align: left;
    font-size: var(--font-size-sm);
    color: var(--color-black);
    font-family: var(--font-archivo);
  }
  .signUpPage {
    width: 100%;
    position: relative;
    background-color: #fafafa;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    letter-spacing: normal;
  }
  .signUpPage:hover {
    background: linear-gradient(#fff, #fff), #87550a;
  }

  @media screen and (max-width: 1275px) {
    .copyrightnotice {
      max-width: 100%;
    }

    .privacypolicyframe {
      max-width: 100%;
    }
  }
  @media screen and (max-width: 1100px) {
    .loginSections {
      padding: 110px 84px;
      box-sizing: border-box;
    }
  }
  @media screen and (max-width: 750px) {
    .loginSections {
      padding-top: var(--padding-52xl);
      padding-bottom: var(--padding-52xl);
      box-sizing: border-box;
    }

    .copyrightnotice {
      flex-wrap: wrap;
    }
  }
  @media screen and (max-width: 450px) {
    .loginSections {
      gap: 56px;
      padding-left: var(--padding-23xl);
      padding-right: var(--padding-23xl);
      box-sizing: border-box;
    }
  }
</style>
