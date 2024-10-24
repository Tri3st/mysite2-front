<template>
  <div class="three-column-layout">
    <header>
      <AppLogo />
      <AppNavigation />
    </header>

    <main>
      <slot />
    </main>

    <aside>
      <slot name="aside" />
      <AppFooter />
    </aside>
  </div>
</template>

<script>
export default {
  name: "ThreeColumnLayout",
}
</script>

<style scoped lang="scss">
.three-column-layout {
  display: grid;
  grid-template-areas:
    "header"
    "main"
    "aside";
}
</style>