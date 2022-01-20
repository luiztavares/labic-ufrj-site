<template>
  <q-page class="hero">
    <q-carousel
      v-model="slide"
      transition-prev="scale"
      transition-next="scale"
      swipeable
      animated
      control-color="white"
      navigation
      navigation-position="bottom"
      padding
      class="transparent"
    >
      <q-carousel-slide name="tv" class="row no-wrap items-center">
        <div id="aovivo" class="vertical-text col-1 q-mx-sm text-white">
          <p>AO VIVO</p>
        </div>

        <div id="video" class="col-11">
          <q-video :ratio=16/9 src="https://www.youtube.com/embed/_chmTnA--9I"/>
        </div>
      </q-carousel-slide>
      <q-carousel-slide
        name="style"
        class="full-width row no-wrap justify-between items-center"
      >
        <img
          class="col-8"
          alt="Inovação Cidadã"
          src="../../public/carousel-header.svg"
        />
        <img
          class="col-3"
          alt="Inovação Cidadã"
          src="../../public/carousel-icon.svg"
        />
      </q-carousel-slide>
    </q-carousel>
  </q-page>
  <q-page class="row">
    <div class="projeto-left q-pa-xl col-5 text-right column justify-center">
      <div class="projeto-header col-auto">
        <p class="align-center no-padding no-margin text-no-wrap">O PROJETO</p>
        <q-separator size="5px" color="purple-13"></q-separator>
      </div>

      <p class="projeto-subheader col-auto q-mt-xl text-no-wrap">
        LABORATÓRIO DE<br />INOVAÇÃO CIDADÃ
      </p>
    </div>
    <div
      class="col-7 flex projeto-right q-pl-xl q-pt-xl q-pr-sm vertical-middle"
      vertical-middle
    >
      <p>
        O Laboratório de Inovação Cidadã da UFRJ é uma rede de ações, pesquisa,
        e formação com objetivo de mapear e sistematizar experiências de
        referência em tecnologias sociais e inovação no Estado do Rio de
        Janeiro. São espaços criados para desenvolver, apoiar e acelerar essas
        propostas que surgem e têm potencial para serem replicadas ou ativar
        outras ações, pesquisas e iniciativas
      </p>
      <p class="bluegreat">É O "MATCH DA INOVAÇÃO"</p>
      <p>
        porque aproxima projetos e experiências da cidade com quem pode ajudar a
        concretizá-lo ou melhorá-los.
      </p>
      <p>
        A iniciativa é realizada pelo Pontão de Cultura Digital da Escola de
        Comunicação da UFRJ, coordenado pela professora Ivana Bentes desde 2017.
        As edições anteriores são: Rio de Janeiro 2017,2018,2019 e edições em
        Salvador 2019 e Lisboa 2019.Desde 2020 realizamos edições virtuais
      </p>
      <p>
        O Laboratório de Inovação Cidadã conta com o apoio da Bolsa Cientista do
        Nosso Estado da FAPERJ e CNPQ.
      </p>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import { ref } from "vue";

export default defineComponent({
  name: "PageIndex",

  setup() {
    return {
      slide: ref("tv"),
      lorem:
        "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque voluptatem totam, architecto cupiditate officia rerum, error dignissimos praesentium libero ab nemo.",
    };
  },
});
</script>

<style scoped>
.hero {
  background: url("../../public/carrousel-background.png");
  background-size: 100% 100%;
}

.q-carousel {
  min-height: inherit;
  min-width: inherit;
}

#aovivo {
  min-height: 49.8vw;
  border-left: 5px solid white;
}

#aovivo p {
  font-size: 5vw;
}

.vertical-text {
  writing-mode: vertical-rl;
  text-orientation: mixed;
  -webkit-transform: rotate(180deg);
  -moz-transform: rotate(180deg);
}

.projeto-header p {
  color: #df71ff;
  font-size: 3em;
}

.projeto-left {
  background-color: #8b50ff;
}

.projeto-right {
  background-color: #df71ff;
  font-size: 1.4rem;
}
.projeto-subheader {
  color: white;
  font-size: 3.5rem;
}

.bluegreat {
  font-size: 2.5rem;
  text-shadow: 1px 1px black;
  color: #00d3de;
  font-weight: bold;
}
</style>
