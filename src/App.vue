<template>
  <div class="container">
    <div class="row">
      <ms_header></ms_header>
    </div>
    <hr>
    <div class="row">
      <ms_server></ms_server>
      <ms_statusUpdate></ms_statusUpdate>
    </div>
    <hr>
    <div class="row">
      <ms_footer></ms_footer>
    </div>
  </div>
</template>

<script>
  import Footer from './components/Shared/Footer.vue'
  import Header from './components/Shared/Header.vue'
  import Server from './components/Server/Servers.vue'
  import StatusUpdate from './components/Server/StatusUpdate.vue';

  export default {
    components: {
      'ms_header': Header,
      'ms_server': Server,
      'ms_statusUpdate': StatusUpdate,
      'ms_footer': Footer
    }
  }
</script>

<style>

</style>
