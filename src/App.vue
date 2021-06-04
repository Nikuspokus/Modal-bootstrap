<template>
  <div id="app">
    <HelloWorld msg="Test Modal" />

    <div>
      <b-button id="show-btn" @click="$bvModal.show('bv-modal-example')"
        >Open Modal</b-button
      >

      <b-modal
        id="bv-modal-example"
        hide-footer
        hide-header
        class="modal-xl "
        size="lg"
      >
        <div class="">
        
          <div>
            <h3>Hello From This Modal!</h3>
          </div>
          <div class="d-block text-center ">
            Using <code>$bvModal</code> Methods
          </div>
          <div class="row ">
            <div class="col  p-0">
              <div class="row m-2 border border-primary rounded bg-white">
                <div class="row text-muted m-1">
                  Description
                  <span>
                    <h1>Ceci est un titre</h1>
                    <p>
                      Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                      Neque inventore a eaque atque vitae eius odio, recusandae
                      harum voluptate! Quos quis totam dolorem culpa
                      exercitationem ipsa amet quas pariatur autem.
                    </p>
                  </span>
                </div>
                <div class="row text-muted m-1">Sujets de la réunion</div>
              </div>
              <div class="row m-2 border border-primary rounded bg-white text-muted m-1">
                <div class="row text-muted m-1">
                blabla 
                </div>
              </div>
              
            </div>
            <div class="col m-2 border border-primary bg-white rounded text-muted m-1">
              Participants
              Voir pour faire un collapse pour la liste des Participants
            </div>

          </div>
          <div class="bg-secondary"></div>
          <hr>
          <b-button
            class="mt-3"
            style="float: right;"
            @click="$bvModal.hide('bv-modal-example')"
            >Retour</b-button
          >
          <b-button
            class="mt-3"
            style="float: left;"
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

  border: 5px solid rgba(0, 0, 0, 0.8);
}
</style>
