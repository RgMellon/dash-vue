<template>
  <v-footer id="core-footer" absolute height="82">
    <div class="footer-items">
      <span v-for="link in links" :key="link.name">
        <a :href="link.Link" class="tertiary--text footer-links">{{ link.name }}</a>
      </span>
    </div>
    <v-spacer />
    <span class="font-weight-light copyright">
      &copy;
      {{ (new Date()).getFullYear() }}
      <a
        href="https://www.creative-tim.com/"
        target="_blank"
      >Powered by pucom</a>
      <v-icon color="tertiary" size="17">mdi-heart</v-icon>Economize
    </span>
  </v-footer>
</template>

<script>
export default {
  data: () => ({})
};
</script>

<style>
#core-footer {
  margin-top: 20px;
  z-index: 0;
}
</style>
