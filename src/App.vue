<template>
  <div id="app">
    <HelloWorld msg="Test Modal" />

    <div>
      <div class="mx-auto center" style="width: 150px;">
        <b-button id="show-btn" @click="$bvModal.show('bv-modal-example-1')"
          >Open Modal 1
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
                  <b-button
                    class="size"
                    style="background-color:rgb(0, 119, 255); border:none; "
                  >
                    <div class="row  ">
                      <a
                        href="https://www.google.fr"
                        target="_blank"
                        class="mx-auto m-2 d-block"
                        style="color: white; text-decoration:none"
                      >
                        Rejoindre la réunion
                      </a>
                    </div>
                  </b-button>
                  
                  
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
                class="col-4 m-2 border border-primary-50 bg-white rounded text-muted m-1"
                id="droite"
              >
                <div class="m-2">
                  Participants
                </div>
                <div>
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
            <hr />
            <b-button
              class="mt-3"
              style="float: right;"
              @click="$bvModal.hide('bv-modal-example-1')"
              >Retour</b-button
            >
          </div>
        </div>
      </b-modal>
      <!-- //////////////////////////////////////////////////// -->
      <!-- <b-modal
        id="bv-modal-example-2"
        hide-footer
        hide-header
        class="modal-xl m-1 border border-primary-50 rounded"
        size="lg"
      >
        <div id="global">
          <h3 class="text-center">YPO</h3>
          <div
            id="gauche"
            class="border border-primary-50 bg-white p-2"
            style="border-radius: 10px;"
          >
            <div class="col ">
              <div
                class="border border-primary-50 row text-muted m-2 mb-10"
                style="height: 300px; border-radius: 10px;"
              >
                <p>
                  Description de la réunion
                </p>
                <h6>Ceci est un titre</h6>
                <br />
                <p>
                  Une petite réunion Agile pour partir en vacances d'été
                  l'esprit tranquille
                </p>
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

              <div class="container">
                <b-button
                  class="size"
                  style="background-color:rgb(0, 119, 255); border:none; "
                >
                  <div class="row  ">
                    <a
                      href="https://www.google.fr"
                      target="_blank"
                      class="mx-auto m-2 d-block"
                      style="color: white; text-decoration:none"
                    >
                      Rejoindre la réunion
                    </a>
                  </div>
                </b-button>
                <div>
                  <b-badge style="background-color:pink" class="mx-1"
                    >Speak'up</b-badge
                  >
                  <b-badge style="background-color:green" class="mx-1"
                    >PHP</b-badge
                  >
                  <b-badge class="test-3 mx-1">SII lille</b-badge>
                </div>
              </div>
            </div>
          </div>

          <div
            id="droite"
            class="border border-primary-50 bg-white p-2"
            style="border-radius: 10px;"
          >
            <div>
              liste des participants
            </div>
            <div>
              <div>
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
          <hr />
          <b-button
            class="mt-3"
            style="float: right;"
            @click="$bvModal.hide('bv-modal-example-2')"
            >Retour
          </b-button>
        </div>
      </b-modal> -->
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

.test-1 {
  background-color: rgb(0, 119, 255);
}
.test-2 {
  background-color: rgb(0, 119, 255);
}
.test-3 {
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
}
a {
  color: aqua;
}
.container {
  justify-content: flex-start;
  align-self: flex-end;
}
</style>
