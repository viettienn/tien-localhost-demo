<template>
  <header :class="$style.header">
    <div :class="$style.appHeaderOld">
      <div :class="$style.headerContent">
        <img :class="$style.logoIcon" loading="lazy" alt="" src="/logo.svg" />
        <div :class="$style.navLinks">
          <div :class="$style.home">Home</div>
          <div :class="$style.stays">Stays</div>
          <div :class="$style.becomeAHost">Become a host</div>
        </div>
      </div>
    </div>
  </header>
</template>
<script lang="ts">
  import { defineComponent } from "vue";

  export default defineComponent({
    name: "Component",
  });
</script>
<style module>
  .logoIcon {
    height: 40.5px;
    width: 156.8px;
    position: relative;
  }
  .home {
    position: relative;
  }
  .stays {
    position: relative;
  }
  .becomeAHost {
    position: relative;
    white-space: nowrap;
  }
  .navLinks {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: flex-start;
    gap: 0px 30px;
  }
  .headerContent {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    max-width: 1280px;
    gap: var(--gap-xl);
  }
  .appHeaderOld {
    align-self: stretch;
    background-color: var(--primary-contrast);
    border-bottom: 1px solid var(--light-grey-border);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: var(--padding-sm) var(--padding-xl);
  }
  .header {
    align-self: stretch;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    text-align: left;
    font-size: var(--font-size-sm);
    color: var(--color-black);
    font-family: var(--font-archivo);
  }

  @media screen and (max-width: 1275px) {
    .headerContent {
      max-width: 100%;
    }
  }
</style>
