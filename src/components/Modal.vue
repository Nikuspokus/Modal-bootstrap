<template>
  <div>

    <b-button @click="showModal">Open Modal</b-button>

    <b-modal id="modal-1">
      <div class="d-block">Hello From My Modal!</div>
      <b-button @click="hideModal">Close Me</b-button>
      <b-button @click="toggleModal">Toggle Me</b-button>
    </b-modal>

  </div>
</template>

<script>
export default {
  name: "Modal",
  data() {
    return {
      modalShow: true,
    };
  },
};
</script>

<style></style>
