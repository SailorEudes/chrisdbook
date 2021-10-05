<template>
  <div class="waxon_tm_about" id="biographie">
    <div class="container">
      <div class="about_inner">
        <div class="left" v-scroll-reveal="{ delay: 40 }">
          <img
            class="thumbnail"
            src="../../assets/img/about/2.jpg"
            alt="man with sunglass"
          />
        </div>
        <!-- End left thumbnail -->
        <div class="right">
          <div class="name" v-scroll-reveal="{ delay: 40 }">
            <h3>Qui suis-je ?<span class="bg">Résumé</span></h3>
            <span class="job"
              >"Je peux donc je suis. Mais qui suis-je ? Être et avoir, drôle de
              binôme."</span
            >
          </div>
          <div class="text">
            <p style="text-align: justify" v-scroll-reveal="{ delay: 60 }">
              Plutôt connu sous mes diminutifs "<b>Swayn</b>", ou
              "<b>Chris</b>", je suis une personne qui a décidé de changer
              physiquement, personnellement mais aussi professionnellement.
            </p>
            <p style="text-align: justify" v-scroll-reveal="{ delay: 70 }">
              Ayant traversé d'innombrables choses, les ayant vécus, et les
              ayant pour certaines, détestées, j'ai décidé de me rendre utile,
              en apportant mon savoir-faire à des personnes qui veulent changer
              dans leur vie, être une meilleure version d'eux-mêmes, pour eux
              <b>en priorité</b>, pour leurs proches, et pour leur vie de tous
              les jours !
            </p>
            <p style="text-align: justify" v-scroll-reveal="{ delay: 80 }">
              Avec maintenant 5 ans d'expérience dans ce domaine, je serais apte
              à accompagner les personnes qui le veulent, mais le vouloir ne
              suffit pas à mes yeux, il faut aussi le faire, ne pas abandonner,
              donner du sien et surtout, <b>se faire confiance</b> !
            </p>
          </div>
          <div class="waxon_tm_button" v-scroll-reveal="{ delay: 100 }">
            <button class="ib-button" @click="showModal">
              <span>Données Physiques</span>
            </button>
          </div>
        </div>
        <!-- End right content -->
      </div>
    </div>

    <!-- Start Modalbox -->
    <transition name="fade">
      <!-- Modal -->
      <div
        :class="{ 'modal-mask': isActive }"
        id="modal"
        @click="closeModal"
        v-if="isVisible"
      >
        <div
          class="
            modal-dialog
            modal-dialog-centered
            modal-dialog-scrollable
            modal-user
          "
          @click.stop
        >
          <div class="modal-content">
            <div class="waxon_tm_modalbox_about">
              <div class="close" @click="closeModal">
                <img
                  class="svg"
                  src="../../assets/img/svg/cancel.svg"
                  alt="cancel-img"
                />
              </div>
              <!-- End .close -->
              <div class="my_box">
                <div class="left">
                  <div class="about_title">
                    <h3>Composition</h3>
                  </div>
                  <!-- End .abut_title -->
                  <div class="waxon_progress">
                    <div class="progress_inner">
                      <span
                        ><span class="label">Eau</span
                        ><span class="number">54%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width: 54%"></div>
                        </div>
                      </div>
                    </div>
                    <!-- End progress_inner -->
                    <div class="progress_inner">
                      <span
                        ><span class="label">Graisse Corporelle</span
                        ><span class="number">22%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width: 22%"></div>
                        </div>
                      </div>
                    </div>
                    <!-- End progress_inner -->
                    <div class="progress_inner">
                      <span
                        ><span class="label">Protéine</span
                        ><span class="number">21%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width: 21%"></div>
                        </div>
                      </div>
                    </div>
                    <!-- End progress_inner -->
                  </div>
                  <!-- End .waxon_progress -->
                </div>
                <!-- End .left -->
                <div class="right">
                  <div class="about_title">
                    <h3>Langues</h3>
                  </div>
                  <div class="waxon_progress">
                    <div class="progress_inner">
                      <span
                        ><span class="label">Français</span
                        ><span class="number">100%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width: 100%"></div>
                        </div>
                      </div>
                    </div>
                    <div class="progress_inner">
                      <span
                        ><span class="label">Italien</span
                        ><span class="number">90%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width: 90%"></div>
                        </div>
                      </div>
                    </div>
                    <div class="progress_inner">
                      <span
                        ><span class="label">Anglais</span
                        ><span class="number">50%</span></span
                      >
                      <div class="background">
                        <div class="bar">
                          <div class="bar_in" style="width: 50%"></div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
                <!-- End .right -->
              </div>
              <div class="counter">
                <div class="about_title">
                  <h3>Physique</h3>
                </div>
                <ul>
                  <li>
                    <div class="list_inner">
                      <h3>182cm</h3>
                      <span>Hauteur</span>
                    </div>
                  </li>
                  <li>
                    <div class="list_inner">
                      <h3>78Kg</h3>
                      <span>Poids</span>
                    </div>
                  </li>
                  <li>
                    <div class="list_inner">
                      <h3>Equilibrée</h3>
                      <span>Forme Corporelle</span>
                    </div>
                  </li>
                  <li>
                    <div class="list_inner">
                      <h3>Bleus</h3>
                      <span>Yeux</span>
                    </div>
                  </li>
                  <li>
                    <div class="list_inner">
                      <h3>Châtains</h3>
                      <span>Cheveux</span>
                    </div>
                  </li>
                  <li>
                    <div class="list_inner">
                      <h3>Complète</h3>
                      <span>Barbe</span>
                    </div>
                  </li>
                   <li>
                    <div class="list_inner">
                      <h3>42</h3>
                      <span>Pointure</span>
                    </div>
                  </li>
                </ul>
                <!-- End ul -->
              </div>
              <!-- End .counter -->
              <div class="partners">
                <div class="about_title">
                  <h3>Our Partners</h3>
                </div>
                <Brand />
              </div>
              <!-- End .partner -->
            </div>
            <!-- End .tokyo_tm_modalbox_about -->
          </div>
        </div>
      </div>
    </transition>
    <!-- End Modalbox -->
  </div>
  <!-- End about -->
</template>

<script>
import Brand from "../Brand.vue";
export default {
  components: {
    Brand,
  },
  data() {
    return {
      isActive: false,
      isVisible: false,
    };
  },
  methods: {
    showModal: function () {
      this.isActive = true;
      this.isVisible = true;
    },
    closeModal: function () {
      this.isActive = false;
      this.isVisible = false;
    },
  },
};
</script>
