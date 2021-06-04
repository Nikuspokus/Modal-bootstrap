<template>
  <div id="app">
    <HelloWorld msg="Test Modal" />

    <div>
      <div class="mx-auto center" style="width: 150px;">
        <b-button id="show-btn" @click="$bvModal.show('bv-modal-example')"
          >Open Modal
        </b-button>
      </div>
      <template>
 
</template>

      <b-modal
        id="bv-modal-example"
        hide-footer
        hide-header
        class="modal-xl m-2 border border-primary-50 rounded"
        size="lg"
      >
        <template #modal-title> Using <code>$bvModal</code> Methods </template>
        <div>
          <div>
            <h3 style="display: inline">YPO next Gen #5</h3>
            <b-button-close
              type="button"
              class="border-radius: 20px bg-transparent"
              aria-label="close"
              style="border-color: transparent; border-radius:5px; float:right"
              @click="$bvModal.hide('bv-modal-example')"
            >X
            </b-button-close>
          </div>
          <div class="row">
            <div class="col-7 p-0">
              <div class="row m-2 border border-primary-50 rounded bg-white">
                <div class="row text-muted m-1">
                  <p>
                    Description de la réunion
                  </p>
                  <h6 class="m-0 p-0">Ceci est un titre</h6>
                  <br />
                  <p class="m-0 p-0">
                    Une petite réunion Agile pour partir en vacances d'été
                    l'esprit tranquille
                  </p>
                </div>
                <div class="row text-muted m-1">
                  <div>
                    Sujets de la réunion:
                  </div>
                  <ul>
                    <li class="ml-3">dsfsdf</li>
                    <li class="pl-3">dsfsdf</li>
                    <li class="ml-3">dsfsdf</li>
                  </ul>
                </div>
              </div>
              <div
                class="row m-2 border border-primary-50 rounded  text-muted m-1"
              >
                <div class="row text-muted m-1">
                  Lien de la reunion:
                  <a href="https://www.google.fr" target="_blank"
                    ><img
                      class="mx-auto mb-2 d-block"
                      src="./assets/logo-web-2020.png"
                      width="20%"
                  /></a>
                </div>
              </div>
              <div class="row m-2 text-muted">
                <div class="row text-muted ">
                  <div>
                    <b-badge style="background-color:green" class="mx-1"
                      >New</b-badge
                    >
                    <b-badge style="background-color:orange" class="mx-1"
                      >New</b-badge
                    >
                    <b-badge style="background-color:purple" class="mx-1"
                      >New</b-badge
                    >
                    <b-badge style="background-color:pink" class="mx-1"
                      >New</b-badge
                    >
                    <b-badge style="background-color:blue" class="mx-1"
                      >New</b-badge
                    >
                    <b-badge variant="primary">Primary</b-badge>
                  </div>
                </div>
              </div>
            </div>
            <div
              class="col-4 m-2 border border-primary-50 bg-white rounded text-muted m-1"
            >
              Participants Voir pour faire un collapse pour la liste des
              Participants
            </div>
          </div>
          <hr />
          <b-button
            class="mt-3"
            style="float: right;"
            @click="$bvModal.hide('bv-modal-example')"
            >Retour</b-button
          >
        </div>
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
      this.$root.$emit("bv::show::modal", "modal-1", "#btnShow");
    },
    hideModal() {
      this.$root.$emit("bv::hide::modal", "modal-1", "#btnShow");
    },
  },
};
</script>

<style>
hr {
  border: 0;
  border-top: 1px solid rgba(0, 0, 0, 0.1);
}
</style>

