<template>
  <div id="app">
    <HelloWorld msg="Welcome to Your Vue.js App" />


    <div>
  <b-button @click="showModal" ref="btnShow">Open Modal</b-button>

  <b-modal id="modal-1">
    <div class="d-block">Hello From My Modal!</div>
    <b-button @click="hideModal">Close Me</b-button>
    <b-button @click="toggleModal">Toggle Me</b-button>
  </b-modal>
</div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
  methods: {
    showModal() {
      this.$root.$emit('bv::show::modal', 'modal-1', '#btnShow')
    },
    hideModal() {
      this.$root.$emit('bv::hide::modal', 'modal-1', '#btnShow')
    },

  }
};
</script>

<style>
</style>
