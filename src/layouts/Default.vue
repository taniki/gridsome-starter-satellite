<template>
  <div>
    <nprogress-container />
    <header>
      <b-navbar
        toggleable="lg"
        type="dark"
        variant="dark"
      >
        <b-container>
          <b-navbar-brand to="/">
            mon nouveau produit qui tue
          </b-navbar-brand>
        </b-container>
      </b-navbar>
    </header>

    <div class="mb-4">
      <slot />
    </div>
  </div>
</template>

<script>
import NprogressContainer from 'vue-nprogress/src/NprogressContainer'

export default {
  components: {
    NprogressContainer
  }
}
</script>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>
</style>
