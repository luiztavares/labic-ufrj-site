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
      class="transparent q-px-xl"
    >
      <q-carousel-slide name="tv" class="row no-wrap items-center q-py-xl">
        <div id="aovivo" class="vertical-text col-1 q-mx-sm text-white">
          <p>AO VIVO</p>
        </div>

        <div class="col">
          <q-video id="video" :ratio=16/9 src="https://www.youtube.com/embed/_chmTnA--9I"/>
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
      <p class="bluegreat text-h4">É O "MATCH DA INOVAÇÃO"</p>
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
  <q-page class='projeto2 q-pa-xl row'>
        <div
      class="col column justify-center  text-white text-right "
    >
      <p class='col-auto text-h5 q-pa-sm'>
        Os Laboratórios de Inovação Cidadã, os Labics, são baseados numa metodologia que valoriza a formação de equipes de trabalho multidisciplinares interessadas em participas e colaborar com a produção e difusão de protótipos, produtos e serviços que apontem soluções para questões desafiadoras e concretas das cidades e/ou de seus teritórios
      </p>
      <p class="bluegreat col-auto text-h4 q-pa-sm">Os Labics sistematizam, desenvolvem, apoiam e aceleram propostas com potencial para serem replicadas ou que possam ativar outras ações pesquisas e iniciativas.</p>

    </div>
    <div class="q-pa-xl col-6 text-left column justify-center">
      <div class="projeto-header col-auto">
        <p class="align-center no-padding no-margin text-no-wrap">O PROJETO</p>
        <q-separator size="5px" color="purple-13"></q-separator>
      </div>

      <p class="projeto-subheader col-auto q-mt-xl text-no-wrap">
        INOVAÇÃO CIDADÃ
      </p>
    </div>

  </q-page>

  <q-page class='row eixos q-pa-xl'>
    <div class="q-pa-xl col-3 text-left column justify-center text-right">
      <div class="projeto-header2 col-auto">
        <p class="align-center no-padding no-margin text-no-wrap">O PROJETO</p>
        <q-separator size="5px" color="primary"></q-separator>
      </div>

      <p class="projeto-subheader col-auto q-mt-xl text-no-wrap">
        EIXOS
      </p>
    </div>
    <div class="col-9  ">

      <div class="row">
      <div class="col-4 q-pa-xl no-wrap" v-for="eixo in eixos" :key='eixo'>
        <div class="column" >
            <q-icon color="primary" size="50px" class='col' :name='eixo.icon'/>
            <p class='col text-white text-h5 no-margin text-uppercase'>{{eixo.title}}</p>
            <p class="col text-body1 text-weight-medium" >{{eixo.description}}</p>
        </div>
      </div>
      </div>

    </div>
  </q-page>

  <q-page class="row mundo q-pa-xl">
    <div id="aovivo" class="vertical-text col-1 q-mx-sm">
          <p class='color-secondary'>O PROJETO</p>
        </div>

        <div class="col q-ma-md flex">
          <p class="text-h2 color-primary">LABORATÓRIOS NO MUNDO</p>
          <p class="fill-text text-body text-white text-justify">O Laboratório de Inovação Cidadã é um projeto Secretaria-Geral Ibero-americana que tem como objetivo promover a inovação cidadã a fim de fomentar a transformação social, a governança democrática, e o desenvovimento social, cultural e econômico. Inovação Cidadã é um processo que resolve problemas sociais com tecnologias(digitais, sociais, ancestrais) e metodologias inovadoras, através do envolvimento da própria comunidade afetada. Com isso, os cidadãos deixam de ser receptores passivos de ações institucionais e se convertem em protagonistas e produtores de suas próprias soluções.
          </p>
        </div>
        <div class="col flex items-center justify-center">
          <q-icon class='pink' size="40vw" name='language'>
          </q-icon>
          <q-btn  outline size='1.5vw' color='primary' label="Saiba Mais Aqui">

          </q-btn>
        </div>
  </q-page>

  <q-page class="hero row q-pa-xl">
        <div id="aovivo" class="vertical-text col-1 q-mx-sm">
          <p class='color-primary text-uppercase'>Inscrições</p>
        </div>

        <div class="col column q-ma-md justify-center items-center">
          <p class="col-auto text-h2 text-white text-center">Estão abertas até o dia 30 de setembro</p>
          <p class="col-auto text-h4 text-white text-center">as inscrições para o Monitora Labic. Nesta edição, vamos selecionar 13 projetos que já participaram de alguma edição anterior. Serão oferecidos mentorias específicas para recomeçar e fortalecer suas atividades.
          </p>
          <q-btn id='rounder' size='xl' style="width: 40%;" class='q-ma-xl text-white' label='ACESSE A CHAMADA'></q-btn>
        </div>

  </q-page>
  
</template>

<script>
import { defineComponent } from "vue";
import { ref } from "vue";

export default defineComponent({
  name: "PageIndex",
  data: function(){
    return{
      eixos:[
        {
          icon:'smartphone',
          title:'Mídias, Ações Virtuais e Diversidade',
          description:'Projetos, ações, aplicativos e tecnologias que apresentem iniciativas de comunicação em qualquer suporte e linguagem e que estimulem a diuversidade de conteúdos e de produtos de mídias.',
        },
        {
          icon:'pie_chart',
          title:'Tecnologias, Redes, Dados e Plataformas',
          description:'Iniciativas de desenvolvimento de plataformas, redes, aplicativos, programas, tecnologias abertas. Projetos de mineração, análise e visualização de dados.',
        },
        {
          icon:'auto_stories',
          title:'Formação',
          description:'Projetos, propostas, metodologias de formação e educação utilizando qualquer linguagem; formação em rede, formação livre, educação inclusiva, formação de agentes e multiplicadores, formação para a diversidade; educação e inovação.',
        },
        {
          icon:'business',
          title:'Economia e Cidadania',
          description:'Iniciativas em novas economias, sustentabilidade, financiamento colaborativo, empreendedorismo social, redes de proteção, inclusão, visibilidade, ampliação de direitos para a diversidade cultural, de gênero, religiosa, étnica, etc.',
        },
        {
          icon:'coronavirus',
          title:'Ações de enfrentamento a covid-19',
          description:'no campo da saúde, comunicação, da cultura, educacionais e em todos os campos do conhecimento, constituição de redes de apoio e solidariedade pós-pandemia.',
        },
        {
          icon:'add',
          title:'Outros temas',
          description:'',
        },
      ]
    }
  },

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
  height: 49.8vw;
  max-height: 80.8vh;
  border-left: 3px solid white;
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

.projeto-header2 p {
  color: #00d3de;
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
  text-shadow: 1px 1px black;
  color: #00d3de;
  font-weight: bold;
}


.projeto2{
background-color:#8b50ff}

.mundo{
background-color:#8b50ff}

.eixos{
  background-color: #df71ff
}

.color-primary{
  color:#00d3de;
}

.color-secondary{
  color:#df71ff;
}

.pink{
  color:#df71ff
}

.fill-text{
  font-size: 1.5vw;
}

#rounder{
border-radius: 75px 75px;
            padding: 35px;
            text-align: center;
            background-color: #df71ff;

}

</style>
