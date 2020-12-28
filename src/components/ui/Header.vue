<template>
  <div>
    <v-app-bar dense>
      <v-toolbar-title>GitHub Search</v-toolbar-title>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>
.theme--light.v-app-bar.v-toolbar.v-sheet {
  @include headerProps;
}

.v-toolbar__title {
  @include hov(font-weight, normal, bold);
  @include hov(font-size, 1rem, 1.5rem);
}
</style>
