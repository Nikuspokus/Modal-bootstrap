<template>
  <div id="app">
    <!-- <HelloWorld class="ml-0 center" msg="Test Modale" /> -->

    <div>
      <div class="mx-auto center" style="width: 150px;">
        <b-button
          class="mt-5"
          id="show-btn"
          @click="$bvModal.show('bv-modal-example-1')"
          >Open Modale
        </b-button>
      </div>
      <!-- <div class="mx-auto center" style="width: 150px;">
        <b-button id="show-btn" @click="$bvModal.show('bv-modal-example-2')"
          >Open Modal 2
        </b-button>
      </div> -->

      <b-modal
        id="bv-modal-example-1"
        hide-footer
        hide-header
        class="modal-xl m-1 border border-primary-50 rounded"
        size="lg"
      >
        <div>
          <div>
            <div>
              <h3 class="text-center ">YPO next Gen #5</h3>
              <!-- <b-button-close
              type="button"
              class="border-radius: 20px"
              aria-label="close"
              style="border-color: transparent; border-radius:5px; float:right"
              @click="$bvModal.hide('bv-modal-example')"
            >
            </b-button-close> -->
            </div>
            <div class="row">
              <div class="col-6 p-0" id="gauche">
                <div class="row m-2 border border-primary-50 rounded bg-white">
                  <div class="row text-muted m-2">
                    <h5>
                      Description de la réunion
                    </h5>
                    <br />
                    <br />
                    <p class="m-0 p-0">
                      Une petite réunion Agile pour partir en vacances d'été
                      l'esprit tranquille
                    </p>
                    <br />
                  </div>
                  <div class="row text-muted m-1">
                    <h6>
                      Sujets de la réunion:
                    </h6>
                    <br />
                    <div>
                      <ul>
                        <li class="ml-3">dsfsdf</li>
                        <li class="pl-3">dsfsdf</li>
                        <li class="ml-3">dsfsdf</li>
                      </ul>
                    </div>
                  </div>
                </div>

                <div class="row m-2 text-muted">
                  <div class="row text-muted ">
                    <div>
                      <b-badge style="background-color:pink" class="mx-1"
                        >Speak'up</b-badge
                      >
                      <b-badge style="background-color:green" class="mx-1"
                        >PHP</b-badge
                      >
                      <b-badge class="test-3 mx-1">SII lille</b-badge>
                      <b-badge variant="primary">Primary</b-badge>
                    </div>
                  </div>
                </div>
              </div>
              <div
                class="col-4 m-2 border border-primary-50 bg-white rounded text-muted "
                id="droite "
              >
                <div class="m-2">
                  Participants (12)
                </div>
                  <div class="scrollbar" id="style-1">
                    <div class="force-overflow m-2">
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Nicolas Vasseur</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Justine Wannehein</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Robin Belon</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Thomas Fournet</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Nicolas Vasseur</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Justine Wannehein</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Robin Belon</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Thomas Fournet</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Julien Bisson</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Eloïse Fauquette</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Thomas Dujardin</b-button
                      >
                      <b-button
                        pill
                        disabled
                        variant="outline-primary"
                        class="m-1"
                        style="font-size: 80%;"
                        >Lea Escorza</b-button
                      >
                    </div>
                </div>
              </div>
            </div>
            <div class="row">
              <div id="global">
                <div
                  id="gauche"
                  class="col-4 m-2 border border-primary-50 bg-white rounded text-muted"
                >
                  <b-button
                    class="size "
                    style="background-color:rgb(0, 119, 255); border:none; float: left"
                  >
                    <div class="row  ">
                      <a
                        href="https://sii-group.com/fr-FR/sii-lille"
                        target="_blank"
                        class="mx-auto d-block"
                        style="color: white; text-decoration:none"
                      >
                        <span class="glyphicon" glyphicon-facetime-video
                          >Rejoindre la réunion</span
                        >
                      </a>
                    </div>
                  </b-button>
                </div>

                <div
                  id="droite"
                  class="col-4 my-2 border border-primary-50 bg-white rounded text-muted"
                >
                  <b-button
                    class="size"
                    style="background-color:rgb(143, 143, 143); border:none; float: right;"
                    @click="$bvModal.hide('bv-modal-example-1')"
                    >Retour
                  </b-button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </b-modal>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",

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

.test-1 {
  background-color: rgb(0, 119, 255);
}

.border {
  border-color: primary;
}
#global {
  width: 100%;
}
#droite,
#gauche {
  display: inline-block;
  vertical-align: top;
}
#gauche {
  width: 62%;
}

#droite {
  width: 32%;
}
.size {
  width: 100%;
  background-color: rgb(0, 119, 255);
  background-color: rgb(143, 143, 143);
}
a {
  color: aqua;
}
.container {
  justify-content: flex-start;
  align-self: flex-end;
}

/* .scroller {
  height: 400px;
  overflow-y: scroll;
  scrollbar-color: rebeccapurple green;
  scrollbar-width: thin;
} */

.scrollbar {
  margin-left: 30px;
  float: left;
  height: 300px;
  overflow-y: scroll;
  margin-bottom: 25px;
}

#style-1::-webkit-scrollbar-track {
  -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
  border-radius: 10px;
  background-color: #f5f5f5;
}

#style-1::-webkit-scrollbar {
  width: 8px;
  background-color: #f5f5f5;
}

#style-1::-webkit-scrollbar-thumb {
  border-radius: 10px;
  background-color: rgb(0, 119, 255);
}
</style>
