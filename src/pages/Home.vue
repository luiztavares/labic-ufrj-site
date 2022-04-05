<template>
  <q-page id="home" class="hero">
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
      <q-carousel-slide name="tv" class="row no-wrap items-center q-py-xl">
        <div id="aovivo" class="vertical-text col-1 q-mx-sm text-white">
          <p>AO VIVO</p>
        </div>

        <div class="col">
          <q-video
            id="video"
            :ratio="16 / 9"
            src="https://www.youtube.com/embed/_chmTnA--9I"
          />
        </div>
      </q-carousel-slide>
    </q-carousel>
  </q-page>

  <q-page id="oprojeto" class="row">
    <div class="projeto-left q-pa-xl col-5 text-right column justify-center">
      <div class="projeto-header col-auto">
        <p class="align-center no-padding no-margin text-no-wrap">O PROJETO</p>
        <q-separator size="5px" color="purple-13"></q-separator>
      </div>

      <p class="projeto-subheader col-auto q-mt-xl text-no-wrap">
        LABORATÓRIO DE
        <br />INOVAÇÃO CIDADÃ
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

  <q-page class="projeto2 q-pa-xl row">
    <div class="col column justify-center text-white text-right">
      <p class="col-auto text-h5 q-pa-sm">
        Os Laboratórios de Inovação Cidadã, os Labics, são baseados numa
        metodologia que valoriza a formação de equipes de trabalho
        multidisciplinares interessadas em participas e colaborar com a produção
        e difusão de protótipos, produtos e serviços que apontem soluções para
        questões desafiadoras e concretas das cidades e/ou de seus teritórios
      </p>
      <p class="bluegreat col-auto text-h4 q-pa-sm">
        Os Labics sistematizam, desenvolvem, apoiam e aceleram propostas com
        potencial para serem replicadas ou que possam ativar outras ações
        pesquisas e iniciativas.
      </p>
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

  <q-page class="row eixos q-pa-xl">
    <div class="q-pa-xl col-3 text-left column justify-center text-right">
      <div class="projeto-header2 col-auto">
        <p class="align-center no-padding no-margin text-no-wrap">O PROJETO</p>
        <q-separator size="5px" color="primary"></q-separator>
      </div>

      <p class="projeto-subheader col-auto q-mt-xl text-no-wrap">EIXOS</p>
    </div>
    <div class="col-9">
      <div class="row">
        <div class="col-4 q-pa-xl no-wrap" v-for="eixo in eixos" :key="eixo">
          <div class="column">
            <q-icon color="primary" size="50px" class="col" :name="eixo.icon" />
            <p class="col text-white text-h5 no-margin text-uppercase">
              {{ eixo.title }}
            </p>
            <p class="col text-body1 text-weight-medium">
              {{ eixo.description }}
            </p>
          </div>
        </div>
      </div>
    </div>
  </q-page>

  <q-page class="row mundo q-pa-xl">
    <div id="aovivo" class="vertical-text col-1 q-mx-sm">
      <p class="color-secondary">O PROJETO</p>
    </div>

    <div class="col q-ma-md flex">
      <p class="text-h2 color-primary">LABORATÓRIOS NO MUNDO</p>
      <p class="fill-text text-body text-white text-justify">
        O Laboratório de Inovação Cidadã é um projeto Secretaria-Geral
        Ibero-americana que tem como objetivo promover a inovação cidadã a fim
        de fomentar a transformação social, a governança democrática, e o
        desenvovimento social, cultural e econômico. Inovação Cidadã é um
        processo que resolve problemas sociais com tecnologias(digitais,
        sociais, ancestrais) e metodologias inovadoras, através do envolvimento
        da própria comunidade afetada. Com isso, os cidadãos deixam de ser
        receptores passivos de ações institucionais e se convertem em
        protagonistas e produtores de suas próprias soluções.
      </p>
    </div>
    <div class="col flex items-center justify-center">
      <q-icon class="pink" size="40vw" name="language"></q-icon>
      <q-btn
        outline
        size="1.5vw"
        color="primary"
        label="Saiba Mais Aqui"
      ></q-btn>
    </div>
  </q-page>

  <q-page id="inscricoes" class="hero row q-pa-xl">
    <div id="aovivo" class="vertical-text col-1 q-mx-sm">
      <p class="color-primary text-uppercase">Inscrições</p>
    </div>

    <div class="col column q-ma-md justify-center items-center">
      <p class="col-auto text-h2 text-white text-center">
        Estão abertas até o dia 30 de setembro
      </p>
      <p class="col-auto text-h4 text-white text-center">
        as inscrições para o Monitora Labic. Nesta edição, vamos selecionar 13
        projetos que já participaram de alguma edição anterior. Serão oferecidos
        mentorias específicas para recomeçar e fortalecer suas atividades.
      </p>
      <q-btn
        id="rounder"
        size="xl"
        style="width: 40%; background: #ff4aa1"
        class="q-ma-xl text-white"
        label="ACESSE A CHAMADA"
      ></q-btn>
    </div>
  </q-page>

  <q-page id="acoesparticipantes" class="column q-pa-md">
    <h1 class="text-h1 col-2 underlined" style="color: #a0d628">
      Ações Participantes
    </h1>
    <q-separator
      class="col-1"
      size="3px"
      style="background-color: #a0d628"
    ></q-separator>
    <p class="col-1 text-h3 q-pt-xl">mais informações em breve</p>
    <div class="col-2 row items-start">
      <q-img
        v-for="index in 6"
        :key="index"
        fit="none"
        class="col"
        alt="Inovação Cidadã"
        src="../../public/carousel-icon.svg"
      />
    </div>
    <div class="col-4"></div>
  </q-page>

  <q-page id="programacao" class="row">
    <div
      class="col-1 vertical-text bgpink text-white text-h2 items-center justify-center flex"
    >
      PROGRAMAÇÃO
    </div>
    <div class="col-4 column q-ma-xl">
      <q-img
        id="maximg"
        class="col-11 no-padding no-margin"
        src="A07F64CF.png"
        alt
      />
      <div class="text-5 col-1 row items-center q-pt-md" style="color: #522de2">
        <q-separator
          size="3px"
          class="col-3"
          style="background-color: #522de2"
        ></q-separator>
        <p class="col-6 text-4 text-center text-h5 text-no-wrap">
          NESTA SEMANA
        </p>
        <q-separator
          size="3px"
          class="col-3"
          style="background-color: #522de2"
        ></q-separator>
      </div>
    </div>
    <div class="col-6 column">
      <div
        class="col-2 bgpink text-h3 text-white flex text-center align-center items-center justify-center"
      >
        ÚLTIMAS MENTORIAS
      </div>
      <div class="row col-10 bgpurple">
        <div
          class="col-6 q-video q-pa-md"
          v-for="ultimaMentoria in ultimasMentorias"
          :key="ultimaMentoria"
        >
          <iframe
            :src="ultimaMentoria"
            frameborder="0"
            allowfullscreen
          ></iframe>
        </div>
      </div>
    </div>
  </q-page>

  <q-page id="edicoesanteriores" class="row bgpink">
    <div class="col-6 column no-wrap items-center">
      <p class="col-10 text-h5 text-right q-pa-xl">
        Após 5 anos, 7 edições e mais de 180 projetos atendidos, o Laboratório
        de Inovação Cidadà abriu uma chamada em setembro de 2021 para saber a
        que pé estavam as iniciativas que fizeram parte desse sucesso que foi o
        Labic UFRJ. 15 desses projetos (pelo menos um de cada edição) retornaram
        e tiveram a oportunidade de participar de novos encontros, criar novas
        redes e encontrar novas parcerias e apoios. Durante oito encontros form
        realizadas mentorias específicas direcionadas para cada um dos
        selecionados. Trocamos conhecimento em diversas áreas, como design e
        comunicação visual; criação e envio de newsletter; elaboração de
        projetos e captação de recursos; gestão de mídias e redes sociais;
        operação de plataformas de streaming e transmissão a vivo; e narrativas.
        Todo esse material está disponível no Youtube do Pontão através do Labic
        Sob Demanda, que reúne conversas com nossos mentores e mentorias
        práticas em uma só playlist!
      </p>
      <q-btn
        id="rounder2"
        class="text-white text-h6 col-1 text-center"
        label="CONFIRA!"
        target = '_blank'
        href = 'https://drive.google.com/file/d/1eLt25u7MLNrzVXOVvzutljgwlSE45-_I/view'
      ></q-btn>
    </div>
    <div class="col q-pa-xl column justify-center">
      <p class="col-1 text-h4 no-padding no-margin yellow">
        EDIÇÕES ANTERIORES
      </p>
      <q-separator class="col-1 yellow" color="yellow" size="3px"></q-separator>
      <p class="col-3 text-h1 q-pt-xl text-white">
        MONITORA
        <br />LABIC
      </p>
    </div>
  </q-page>

  <q-page class="row bgmagenta no-padding no-margin">
    <div class="col-6 column bg-white q-my-xl">
      <div class="col-9 items-center flex no-wrap q-mx-xl">
        <span class="ultralarge yellow">15</span>
        <span class="text-h5 q-ml-md">projetos</span>
        <q-space></q-space>
        <span class="ultralarge yellow">8</span>
        <span class="text-h5 q-ml-md">encontros</span>
      </div>
      <div class="col-3 column bgpink text-center items-center">
        <q-btn outline color="yellow" class="col q-ma-lg" href = 'https://drive.google.com/file/d/1yT6lf60wwKfLnav7fg6ivNOl5730av6j/view' target="_blank">
          <p class="text-white text-h6">
            Confira a lista dos
            <br />Projetos Participantes
          </p>
        </q-btn>
      </div>
    </div>
    <q-img
      id="tesst"
      :ratio="16 / 9"
      fit="fill"
      class="col-6 q-my-xl"
      src="images/Screen Shot 2022-02-15 at 10.51.08.png"
    />
  </q-page>

  <q-page class="column">
    <div class="col-6 row bgpink q-pa-md items-center">
      <p class="col-1 text-h1 vertical-text yellow">2021</p>
      <div class="col-5 column text-right text-white q-pl-xl">
        <p class="text-h3">PROGRAMAÇÃO</p>
        <q-separator
          size="3px"
          style="background-color: rgb(255, 212, 51)"
        ></q-separator>
        <p class="text-h2 q-pt-md">MONITORA LABIC</p>
      </div>
      <div class="col-6 row justify-evenly">
        <img
          class="col q-ml-lg"
          v-for="index in 3"
          :key="index"
          fit="fill"
          src="images/WhatsApp Image 2021-06-22 at 18.42.39.jpeg"
        />
      </div>
    </div>
    <div class="col-5 row q-ma-xl justify-evenly no-wrap">
      <iframe
        class="col-3"
        v-for="video in 3"
        :key="video"
        src="https://www.youtube.com/embed/BDSdW6HjFSA"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
    <div class="col-1 row items-center">
      <q-separator class="col" size="3px" color="black"></q-separator>
      <q-btn outline class="col" label="ACESSE A PROGRAMAÇÃO COMPLETA" href = 'https://www.youtube.com/watch?v=_chmTnA--9I&list=PLT6dlUCLrobCp3l27rvAvD3C7gqkvMOH6' target='_blank'></q-btn>
      <q-separator class="col" size="3px" color="black"></q-separator>
    </div>
  </q-page>

  <q-page class="row">
    <div class="col bgyellow q-pa-xl column justify-center text-right">
      <p class="col-1 text-h4 no-padding no-margin magenta">
        EDIÇÕES ANTERIORES
      </p>
      <q-separator
        class="col-1"
        style="background-color: #ff4aa1"
        size="3px"
      ></q-separator>
      <p class="col-3 text-h1 q-pt-xl text-white">LABIC 2021</p>
      <p class="col-3 text-h2 text-white">EDIÇÃO TERRITÓRIOS</p>
    </div>
    <div class="col-6 bgmagenta column no-wrap items-center">
      <p class="col-10 text-h5 text-right text-white q-pa-xl">
        A urgência de vida trazida pela pandemia, sentida de forma ainda mais
        profunda nas periferias, nos fez testemunhar que as respostas mais
        inovadoras de enfrentamento à Covid-19 e suas consequências foram
        desenvolvidas justamente nesses territórios. O Labic Territórios,
        realizado no primeiro semestre de 2021, olhou para essas iniciativas,
        buscou intensificar a troca de experiências entre realizadores,
        possibilitou a colaboração de universitários, especialistas,
        professores, consultores, gestores, numa verdadeira profusão de troca de
        conhecimentos, saberes, tecnologias, metodologias, criatividade e
        inovação.
        <br />
        <br />O Labic Territórios teve apoio do Pontão de Cultura Digital da
        Escola de Comunicação da UFRJ, da Pró-Reitoria de Extensão da UFRJ, da
        Fundação Universitária José Bonifácio, da FAPERJ e do CNPq.
      </p>
    </div>
  </q-page>

  <q-page class="row bgpurple no-padding no-margin">
    <q-img
      id="tesst"
      :ratio="16 / 9"
      fit="fill"
      class="col-6 q-mb-xl"
      src="images/Screen Shot 2022-02-15 at 11.19.47.png"
    />
    <div class="col-6 column bg-white q-mb-xl">
      <div class="col-9 row">
        <div class="col-7 column justify-center">
          <div class="col row items-center">
            <span class="col text-h1 magenta text-right">17</span>
            <span class="col text-h5 q-ml-md">participações especiais</span>
          </div>
          <div class="col row items-center">
            <span class="col text-h1 magenta text-right">12</span>
            <span class="col text-h5 q-ml-md">encontros</span>
          </div>
          <div class="col row items-center">
            <span class="col text-h1 magenta text-right">9</span>
            <span class="col text-h5 q-ml-md">podcast</span>
          </div>
        </div>
        <div class="col-5 column items-center justify-center">
          <span class="col-4 yellow ultralarge">40</span>
          <span class="col-1 text-h5 q-py-md">projetos</span>
        </div>
      </div>
      <div class="col-3 row bgmagenta text-center items-center">
        <q-btn outline style="color: #8b50ff" class="col q-ma-lg" href = 'https://bit.ly/ResultadoLabicT' target='_blank'>
          <p class="text-white text-h6">
            Confira a lista dos
            <br />Projetos Participantes
          </p>
        </q-btn>

        <q-btn outline style="color: #8bf0ff" class="col q-ma-lg" href = ' https://bit.ly/ResumoLabicT' target='_blank'>
          <p class="text-white text-h6">
            Confira os resumos
          </p>
        </q-btn>
      </div>
    </div>
  </q-page>

  <q-page class="column">
    <div class="col-6 row bgmagenta q-pa-xl items-center">
      <p class="col-1 text-h1 vertical-text yellow">2021</p>
      <div class="col-5 column text-right text-white">
        <p class="text-h3">PROGRAMAÇÃO</p>
        <q-separator size="3px" class="bgyellow"></q-separator>
        <p class="text-h2 q-pt-md">LABIC TERRITÓRIOS</p>
      </div>
      <div class="col-6 row justify-evenly">
        <img
          class="col q-ml-lg"
          v-for="index in 3"
          :key="index"
          fit="fill"
          src="images/WhatsApp Image 2021-06-22 at 18.42.39.jpeg"
        />
      </div>
    </div>
    <div class="col-5 row q-ma-xl justify-evenly no-wrap">
      <iframe
        class="col-3"
        v-for="video in 3"
        :key="video"
        src="https://www.youtube.com/embed/BDSdW6HjFSA"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
    <div class="col-1 row items-center">
      <q-separator class="col" size="3px" color="black"></q-separator>
      <q-btn outline class="col" label="ACESSE A PROGRAMAÇÃO COMPLETA" href='https://www.youtube.com/watch?v=Zuzm1BaDM_M&list=PLT6dlUCLrobD1Rm9Ac9GT73BjwBTTTZ7c' target='_blank'></q-btn>
      <q-separator class="col" size="3px" color="black"></q-separator>
    </div>
  </q-page>

  <q-page class="row bgyellow">
    <div class="col-6 column no-wrap items-end q-ma-xl">
      <p class="col-10 text-h5 text-right">
        2020 trouxe a pandemia do coronavírus, acarretando mudanças na vida da
        maioria das pessoas. Foram tempos de ruas desertas, escolas e
        universidades fechadas, afastamento sanitário. Nosso desafio era
        produzir um Labic totalmente virtual. oferecendo respostas - vindas de
        dentro - a essa crise mundial. Formamos uma equipe de 13 pessoas para
        atender 40 projetos e gerir 325 colaboradores de todo o Brasil. De 11 de
        setembro a 11 de dezembro de 2020, produzimos 13 encontros e reunimos
        projetos, colaboradores e mentores às sextas-feiras, das 14h às 19h, em
        ambiente virtual. Os encontros foram divididos em conferências,
        mentorias, oficinas, aconselhamento e consultorias específicas, além de
        espaços de troca de expertises entre os grupos e projetos, mesmo num
        ambiente virtual.
      </p>
      <q-btn
        id="rounder3"
        class="magenta text-h6 col-1 text-center"
        label="ACESSE AQUI O RELATÓRIO COMPLETO!"
        href ='https://bit.ly/labic2020'
        target = '_blank'
      ></q-btn>
    </div>
    <div class="col q-pa-xl column justify-center text-left">
      <p class="col-1 text-h4 no-padding no-margin magenta">
        EDIÇÕES ANTERIORES
      </p>
      <q-separator class="col-1 bgmagenta" size="3px"></q-separator>
      <p class="col-3 text-h1 q-pt-xl magenta">LABIC 2020</p>
      <p class="col-3 text-h2 magenta">EDIÇÃO VIRTUAL</p>
    </div>
  </q-page>

  <q-page class="row bgpurple no-padding no-margin">
    <div class="col-6 column bg-white q-mb-xl">
      <div class="col-9 row">
        <div class="col-7 column justify-center">
          <div class="col row items-center">
            <span class="col text-h1 purple text-right">325</span>
            <span class="col text-h5 q-ml-md">colaboradores</span>
          </div>
          <div class="col row items-center">
            <span class="col text-h1 purple text-right">65H</span>
            <span class="col text-h5 q-ml-md">de trabalho</span>
          </div>
          <div class="col row items-center">
            <span class="col text-h1 purple text-right">13</span>
            <span class="col text-h5 q-ml-md">encontros</span>
          </div>
        </div>
        <div class="col-5 column items-center justify-center">
          <span class="col-4 yellow ultralarge">40</span>
          <span class="col-1 text-h5 q-py-md">projetos</span>
        </div>
      </div>
      <div class="col-3 column bgyellow text-center items-center">
        <q-btn style="border: 3px solid #ff4aa1" class="col q-ma-lg" href='https://bit.ly/LABIC2020_PROJETOS_SELECIONADOS' target ='_blank'>
          <p class="text-black text-h6">
            Confira a lista dos
            <br />Projetos Participantes
          </p>
        </q-btn>
      </div>
    </div>
    <q-img
      id="tesst"
      :ratio="16 / 9"
      fit="fill"
      class="col-6 q-mb-xl"
      src="images/Screen Shot 2022-02-15 at 11.19.47.png"
    />
  </q-page>

  <q-page class="column">
    <div class="col-6 row bgyellow q-pa-xl items-center">
      <div class="col-6 row justify-evenly">
        <img
          class="col q-mr-lg"
          v-for="index in 3"
          :key="index"
          fit="fill"
          src="images/WhatsApp Image 2021-06-22 at 18.42.39.jpeg"
        />
      </div>
      <div class="col-5 column text-right text-white">
        <p class="text-h3 text-white">PROGRAMAÇÃO</p>
        <q-separator class="bgmagenta" size="3px"></q-separator>
        <p class="text-h2 text-white q-pt-md">LABIC VIRTUAL</p>
      </div>
      <p class="col-1 text-h1 vertical-text2 magenta">2020</p>
    </div>
    <div class="col-5 row q-ma-xl justify-evenly no-wrap">
      <iframe
        class="col-3"
        v-for="video in 3"
        :key="video"
        src="https://www.youtube.com/embed/BDSdW6HjFSA"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
    <div class="col-1 row items-center">
      <q-separator class="col" size="3px" color="black"></q-separator>
      <q-btn outline class="col" label="ACESSE A PROGRAMAÇÃO COMPLETA" href='https://www.youtube.com/watch?v=c7v6gca2BqQ&list=PLT6dlUCLrobAV6b3H0iRnZZRVxuqj4jZk' target = '_blank'></q-btn>
      <q-separator class="col" size="3px" color="black"></q-separator>
    </div>
  </q-page>

  <q-page class="row bgmagenta">
    <div class="col q-pa-xl column justify-center text-right">
      <p class="col-1 text-h4 no-padding no-margin yellow">
        EDIÇÕES ANTERIORES
      </p>
      <q-separator class="col-1 yellow" color="yellow" size="3px"></q-separator>
      <p class="col-3 text-h1 q-pt-xl yellow">LABIC 2019</p>
      <p class="col-3 text-h2 yellow">EDIÇÃO RIO</p>
    </div>
    <div class="col-6 column no-wrap items-center">
      <p class="col-12 text-h5 text-left q-pa-xl text-white">
        2019 foi um ano intenso. Além da edição anual, realizamos outras duas
        edições do Labic em formato reduzido, duas visitas técnicas e um ciclo
        de formação em análise de dados.
        <br />
        <br />Uma das visitas foi ao Laboratório de Estudos sobre Imagem e
        Cibercultura (Labic) da Universidade Federal do Espírito Santo (UFES) é
        academicamente um dos expoentes brasileiros da Ciência de Dados, tendo
        se tornado, ao longo dos anos, um dos mais respeitados centros de
        referência no assunto.
        <br />
        <br />A segunda, foi à sexta edição do Simpósio Internacional LAVITS:
        Assimetrias e (In)Visibilidades: Vigilância, Gênero e Raça, corrida em
        junho, na Universidade Federal da Bahia (UFBA). No evento, testamos a
        aplicação de uma metodologia de ativação de redes em curtíssimo tempo,
        mapeamos redes parceiras em outros estados, expandindo nossa incidência
        e relevância.
      </p>
    </div>
  </q-page>

  <q-page class="row bgmagenta">
    <div class="col-6 column no-wrap">
      <p class="col-10 q-px-md text-h5 text-right q-pa-xl text-white">
        Foram 25 projetos atendidos por 11 mentores e 5 conferencistas que
        abordaram temas como: redes e narrativas; aplicativos e tecnologias do
        comum, economia colaborativa, sustentabilidade, gestão e governança;
        articulação, mobilização, mídia e ativismo; produção audiovisual; dados
        e algoritmos; dados e narrativas; construção de narrativas para projetos
        e apresentações: ferramentas de gestão de projetos; além das mentorias
        de redes sociais, design e construção de aplicativos.
        <br />
        <br />O Labic Ninja Lisboa aconteceu como integrate da programação da
        Casa Ninja Lisboa em Portugal. Durante três dias, projetos lusitanos
        participaram de oficinas, palestras e mentorias intensas sobre
        desenvolvimento, elaboração de ações, prototipagem, pesquisa aplicada,
        sistematização, uso de tecnologias e ferramentas para gestão de redes,
        ativismo, mídia live etc.
      </p>
      <p class="col-2 text-h2 q-pl-xl text-left yellow">RIO 2019</p>
    </div>
    <div class="col-6 column no-wrap">
      <p class="col-12 q-px-md text-h5 text-left q-pa-xl text-white">
        Nossa consagrada edição regular anual do Labic foi realizada de setembro
        a dezembro de 2019. Reuniu projetos, colaboradores e mentores às
        sextas-feiras, das 16h30 às 20h30, na Central de Produção Multimídia da
        Escola de Comunicação da UFRJ (CPM/ECO). Selecionamos 25 projetos que
        foram atendidos por 70 colaboradores. Os temas das conferências foram:
        cultura de redes e inovação cidadá; gestão de redes e construção de
        narrativas; revolução dos dados: dados abertos e dados cidadãos;
        financiamento coletivo; narrativas, mídias e tecnologias de mobilização;
        vídeo, TV e documentários; gestão e planejamento de projetos;
        ferramentas de organização de equipes; dados abertos e narrativas;
        metodologias de intervenção social em territórios; maratona de mídias
        sociais e design; novas estratégias e linguagens políticas; maratona de
        criação de sites; dados e plataformas; articulação e mobilização; mídias
        sociais; audiovisual e podcasting; design; narrativas e formação.
      </p>
    </div>
  </q-page>

  <q-page class="row bgyellow no-padding no-margin">
    <q-img id="tesst" fit="fill" class="col-7 q-mb-xl" src="images/2019.jpg" />
    <div class="col-5 column bg-white q-mb-xl">
      <div class="col-9 row">
        <div class="col-7 column justify-center">
          <div class="col row items-center">
            <span class="col text-h1 yellow text-right">70</span>
            <span class="col text-h5 q-ml-md">colaboradores</span>
          </div>
          <div class="col row items-center">
            <span class="col text-h1 yellow text-right">5</span>
            <span class="col text-h5 q-ml-md">conferencistas</span>
          </div>
          <div class="col row items-center">
            <span class="col text-h1 yellow text-right">11</span>
            <span class="col text-h5 q-ml-md">mentores</span>
          </div>
        </div>
        <div class="col-5 column items-center justify-center">
          <span class="col-4 magenta ultralarge">26</span>
          <span class="col-1 text-h5 q-py-md">projetos</span>
        </div>
      </div>
      <div class="col-3 row bgpink text-center items-center">
        <q-btn outline color="white" class="col q-ma-lg" href ='https://drive.google.com/file/d/1SaxV27ECuxNdrHv0McCyVgVh4FwjjUaZ/view?usp=sharing 
' target='_blank'>
          <p class="yellow text-h6">
            Confira a lista dos
            <br />Projetos Participantes
          </p>
        </q-btn>
        <q-btn outline color="gray" class="col q-ma-lg" href='https://drive.google.com/file/d/16Mfm7FYsmX0yLi9chQ5WEVOg9qgEyWCp/view?usp=sharing' target='_blank' >
          <p class="yellow text-h6">
            Projetos na íntegra 
          </p>
        </q-btn>
      </div>
    </div>
  </q-page>

  <q-page class="bgmagenta row">
    <div class="col-5 column no-wrap">
      <q-img
        class="col-6 q-mb-sm"
        src="images/27.9 primeiro encontro c colabs.jpg"
        fit="fill"
      />
      <q-img
        class="col-6"
        fit="fill"
        src="images/70817574_2523949274314774_1584828428119441408_n.jpg"
      />
    </div>
    <div class="col-7 column no-wrap q-pl-sm">
      <div class="col-2 self-center">
        <span class="text-h3 text-white">
          PROGRAMAÇÃO
          <span class="yellow text-h1">|</span>
          <span class="text-h3"> LABIC RIO</span>
          <span class="yellow text-h2"> 2019</span>
        </span>
      </div>
      <q-img
        class="col-9 q-pa-xl"
        src="images/74667953_2691170994259267_6604921933240729600_n.jpg"
      />

      <div class="col-1 self-center q-pa-md">
        <q-btn
          unelevated
          color="yellow"
          class="text-black"
          label="ACESSE A PROGRAMAÇÃO COMPLETA"
        ></q-btn>
      </div>
    </div>
  </q-page>

  <q-page class="row">
    <div class="col-6 column no-wrap items-center bgyellow">
      <p class="col-12 text-h5 text-right q-pa-xl">
        Nosso ciclo formativo em fluxo seguiu para a cidade de Salvador (BA)
        durante o Simpósio Internacional LAVITS: Assimetrias e
        (In)Visibilidades: Vigilância, Gênero e Raça, ocorrido em junho, na
        Universidade Federal da Bahia (UFBA). No evento, testamos a aplicação de
        uma metodologia de ativação de redes em curtíssimo tempo, mapeamos redes
        parceiras em outros estados, expandindo nossa incidência e relevância.
        Foram 25 projetos atendidos por 11 mentores e 5 conferencistas que
        abordaram temas como: redes e narrativas; aplicativos e tecnologias do
        comm, economia colaborativa, sustentabilidade, gestão e governança;
        articulação, mobilização, mídia e ativismo; produção audiovisual; dados
        e algorítimos; dados e narrativas; construção de narrativas para
        projetos e apresentações; ferramentas de gestão de projetos; além das
        mentorias de redes sociais, design e construção de aplicativos.
      </p>
    </div>
    <div class="col q-pa-xl column bgpink justify-center text-left">
      <p class="col-1 text-h4 no-padding no-margin yellow">
        EDIÇÕES ANTERIORES
      </p>
      <q-separator class="col-1 yellow" color="yellow" size="3px"></q-separator>
      <p class="col-3 text-h1 q-pt-xl text-white">LABIC 2019</p>
      <p class="col-3 text-h2 text-white">EDIÇÃO BAHIA</p>
    </div>
  </q-page>

  <q-page class="row bgmagenta no-padding no-margin">
    <div class="col-6 column bg-white q-mb-xl">
      <div class="col-9 row q-mx-xl">
        <div class="col-8 column justify-evenly">
          <div class="col-6 row items-end">
            <span class="col ultralarge yellow text-right">11</span>
            <span class="col text-h5 q-my-lg"> mentorias</span>
          </div>
          <div class="col-6 row items-end">
            <span class="col ultralarge yellow text-right">5</span>
            <span class="col text-h5 q-my-lg">conferencistas</span>
          </div>
        </div>
        <div class="col-4 column items-center justify-center">
          <span class="col-4 magenta ultralarge">25</span>
          <span class="col-1 text-h5 q-py-md">projetos</span>
        </div>
      </div>
      <div class="col-3 column bgpink text-center items-center">
        <q-btn style="border: 3px solid rgb(255, 212, 51)" class="col q-ma-lg">
          <p class="text-white text-h5">
            Confira a lista dos
            <br />Projetos Participantes
          </p>
        </q-btn>
      </div>
    </div>
    <q-img
      id="tesst"
      fit="cover"
      class="col-6 q-mb-xl"
      src="images/BA 2019.png"
    />
  </q-page>

  <q-page class="bgmagenta row">
    <div class="col-5 column no-wrap">
      <q-img
        class="col-6 q-mb-sm"
        src="images/pense-em-libras-min-1024x560.png"
        fit="fill"
      />
      <q-img class="col-6" fit="fill" src="images/iami-agbá-min-1024x559.png" />
    </div>
    <div class="col-7 column no-wrap q-pl-sm">
      <div class="col-2 self-center">
        <span class="text-h3 text-white">
          PROGRAMAÇÃO
          <span class="text-h1">|</span>
          <span class="text-h3"> LABIC BAHIA</span>
          <span class="yellow text-h2"> 2019</span>
        </span>
      </div>
      <q-img class="col-9" src="images/femini-2-min-1024x576.png" fit="fill" />

      <div class="col-1 self-center q-pa-md">
        <q-btn
          unelevated
          color="yellow"
          class="text-black"
          label="ACESSE A PROGRAMAÇÃO COMPLETA"
        ></q-btn>
      </div>
    </div>
  </q-page>

  <q-page class="row bgpink">
    <div class="col q-pa-xl column justify-center text-right">
      <p class="col-1 text-h4 no-padding no-margin yellow">
        EDIÇÕES ANTERIORES
      </p>
      <q-separator class="col-1 yellow" color="yellow" size="3px"></q-separator>
      <p class="col-3 text-h1 q-pt-xl text-white">LABIC 2018</p>
    </div>
    <div class="col-6 row justify-center items-center q-pa-xl">
      <p class="col text-h5 text-left text-black">
        Em 2018, o Labic foi desafiado a alcançar voos mais amplos. Com apoio da
        UFRJ, renovamos e consolidamos o projeto e de suas atividades, que já
        eram referência em cultura digital e ambient cognitivo de diversidade,
        produção e partilha de saberes e cosmovisões plurais. A segunda edição
        do Labic reuniu lideranças e gestores de projetos, pesquisadores,
        mentores e colaboradores entre os meses de setembro e dezembro de 2018
        no Rio de Janeiro, conectando pessoas interessadas no intercâmbio de
        ideas de práticas pioneiras e inovadoras da economia criativa. Vinte
        projetos participaram dessa edição e tiveram a oportunidade de
        desenvolver suas propostas, compartilhar experiências, mapear as
        melhorias necessárias e planejar seus próximos passos. Para isso, 58
        colaboradores se uniram as projetos, contribuindo para seu
        desenvolvimento e sustentabilidade em rede.
      </p>
    </div>
  </q-page>

  <q-page class="row bgmagenta">
    <q-img id="tesst" fit="cover" class="col-6 q-mb-xl" src="images/2018.jpg" />
    <div class="col-6 column bg-white q-mb-xl">
      <div class="col-9 row q-mx-md">
        <div class="col-9 column justify-evenly">
          <div class="col-6 row items-end">
            <span class="col ultralarge2 magenta text-right">10</span>
            <span class="col text-h5 q-my-lg"> encontros</span>
          </div>
          <div class="col-6 row items-end">
            <span class="col ultralarge2 magenta text-left">100</span>
            <span class="col text-h5 q-my-lg">participantes</span>
          </div>
        </div>
        <div class="col-3 column items-center justify-center">
          <span class="col-4 pink ultralarge2">20</span>
          <span class="col-1 text-h5 q-py-md">projetos</span>
        </div>
      </div>
      <div class="col-3 column bgyellow text-center items-center">
        <q-btn style="border: 3px solid #df71ff" class="col q-ma-lg">
          <p class="text-black text-h5">
            Confira a lista dos
            <br />Projetos Participantes
          </p>
        </q-btn>
      </div>
    </div>
  </q-page>

  <q-page class="bgpink row">
    <div class="col-5 column no-wrap">
      <img class="col-6 q-mb-sm" src="images/26.jpg" fit="fill" />
      <img
        class="col-6"
        fit="fill"
        src="images/45687332_2023787100997663_8309980793921339392_n.jpg"
      />
    </div>
    <div class="col-7 column no-wrap q-pl-sm">
      <div class="col-2 self-center row items-center">
        <span class="text-h3 col text-white">
          PROGRAMAÇÃO
          <span class="text-h3 col yellow">----</span>
          <span class="text-h3 col"> LABIC 2018</span>
        </span>
      </div>
      <img
        class="col-8"
        src="images/42730788_2082385008461525_2027607868068331520_n.jpg"
        fit="fill"
      />

      <div class="col-2 self-center q-pa-md">
        <q-btn
          unelevated
          color="yellow"
          class="text-black"
          label="ACESSE A PROGRAMAÇÃO COMPLETA"
        ></q-btn>
      </div>
    </div>
  </q-page>

  <q-page class="row">
    <div class="col q-pa-xl bgyellow column justify-center text-right">
      <p class="col-1 text-h4 no-padding no-margin magenta">
        EDIÇÕES ANTERIORES
      </p>
      <q-separator class="col-1 yellow bgmagenta" size="3px"></q-separator>
      <p class="col-3 text-h1 q-pt-xl magenta">LABIC 2017</p>
    </div>
    <div class="col-6 row justify-center bgmagenta items-center q-pa-xl">
      <p class="col text-h5 text-left text-white">
        O Labic foi implementado na Escola de Comunicação da UFRJ em 2017. O
        laboratório incidiu em toda a Região Metropolitana fluminense. Teve
        Labic no Pontão da ECO, na Central de Produção Multimídia da ECO, no
        Território Inventivo (Centro), na Comunidade da Maré/Redes da Maré, na
        Rede BOTAFOGO Solidária e na ANF -Agência de Notícias da Favela. Além
        desses projetos e iniciativas que viraram parceiros, o Labic contou com
        a colaboração da Mídia Ninja, do Circuito Fora do Eixo, da Companhia
        Teatral Língua de Trapo, da Encantamento Filmes e do Projeto
        Visionárias. Na primeira edição, o Labic realizou 13 encontros, aos
        sábados, das 14h às 18h. Para atender 27 projetos, captou 50
        colaboradores voluntários, mentores e conferencistas, envolvendo
        diretamente 150 pessoas.
      </p>
    </div>
  </q-page>

  <q-page class="row bgpink no-padding no-margin">
    <div class="col-6 column bg-white q-mb-xl">
      <div class="col-9 row">
        <div class="col-7 column justify-center">
          <div class="col row items-center">
            <span class="col text-h1 yellow text-right">150</span>
            <span class="col text-h5 q-ml-md">pessoas</span>
          </div>
          <div class="col row items-center">
            <span class="col text-h1 yellow text-right">50</span>
            <span class="col text-h5 q-ml-md">colaboradores</span>
          </div>
          <div class="col row items-center">
            <span class="col text-h1 yellow text-right">13</span>
            <span class="col text-h5 q-ml-md">encontros</span>
          </div>
        </div>
        <div class="col-5 column items-center justify-center">
          <span class="col-4 pink ultralarge">27</span>
          <span class="col-1 text-h5 q-py-md">projetos</span>
        </div>
      </div>
      <div class="col-3 column bgmagenta text-center items-center">
        <q-btn outline style="color: rgb(255, 212, 51)" class="col q-ma-lg">
          <p class="text-white text-h6">
            Confira a lista dos
            <br />Projetos Participantes
          </p>
        </q-btn>
      </div>
    </div>
    <q-img
      id="tesst"
      :ratio="16 / 9"
      fit="fill"
      class="col-6 q-mb-xl"
      src="images/Screen Shot 2022-02-15 at 11.19.47.png"
    />
  </q-page>

  <q-page class="bgyellow row">
    <div class="col-5 column no-wrap">
      <img
        class="col-6 q-mb-sm"
        src="images/22904764_1583326375043740_1146566215308148923_o.jpg"
        fit="fill"
      />
      <img class="col-6" fit="fill" src="images/9.jpg" />
    </div>
    <div class="col-7 column no-wrap q-pl-sm">
      <div class="col-2 self-center row items-center">
        <span class="text-h3 col text-white">
          PROGRAMAÇÃO
          <span class="text-h3 col magenta">----</span>
          <span class="text-h3 col"> LABIC 2017</span>
        </span>
      </div>
      <img
        class="col-8"
        src="images/22861451_1583328818376829_8855819429735089998_o (1).jpg"
        fit="fill"
      />

      <div class="col-2 self-center q-pa-md">
        <q-btn
          unelevated
          class="text-white bgmagenta"
          label="ACESSE A PROGRAMAÇÃO COMPLETA"
        ></q-btn>
      </div>
    </div>
  </q-page>

  <q-page id="mentores" class="row bgpurple">
    <div class="col column justify-center text-right q-px-xl">
      <div>
        <span class="text-h2 yellow">MENTORES E COLABORADORES</span>
        <q-separator class="q-mb-md q-mt-sm bgyellow" size="5px"></q-separator>
        <span class="color-primary text-h5"
          >MENTORES, COLABORADORES E EXTENSIONISTAS SÃO DE FUNDAMENTAL
          IMPORTÂNCIA NO DESENVOLVIMENTO DOS PROJETOS. CONHECA O QUE ELES
          FAZEM!</span
        >
      </div>
    </div>
    <div class="col column justify-center text-left q-px-xl">
      <div>
        <p class="text-h3 yellow">Mentores</p>
        <p class="text-white text-h5">
          São pensadores, gestores, ativistas, empreendedores, estudantes,
          professors, produtores, desenvolvedores, comunicadores e investidores
          que apresentam diagnósticos, propostas e ações inovadoras para os
          projetos.
        </p>
      </div>
      <div>
        <p class="text-h3 yellow">Colaboradores</p>
        <p class="text-white text-h5">
          Os colaboradores participam das equipes dos projetos selecionados e da
          equipe de organização do Laboratório de Inovação Cidadà para
          desenvolvimento, prototipagem, pesquisa aplicada, sistematização, uso
          de tecnologias e ferramentas e documentação de processos ao longo do
          laboratório.
        </p>
      </div>
    </div>

    <div class="col column justify-center text-left q-px-xl">
      <div>
        <q-icon name="img:Asset 2.svg" size="300px" />
      </div>
      <div class="q-pt-xl">
        <p class="text-h3 yellow">Extensionistas</p>
        <p class="text-white text-h5">
          Extensionista é o aluno da UFRJ que foi selecionado através de chamada
          específica para desenvolver atividades com a comunidade externa
          utilizando o conhecimento adquirido na universidade e participando
          ativamente das ações do Labic. Participa como extensionista e é
          creditado com horas de extensàc que são lançadas no seu BOA.
        </p>
      </div>
    </div>
  </q-page>

  <q-page class="bgyellow">
    <div class="">
      <p class="q-pt-xl q-pl-xl text-h3 pink">
        CONHEÇA ALGUNS DE NOSSOS PARCEIROS
      </p>
      <q-separator class="bgpink q-mr-xl" size="5px"></q-separator>
    </div>
    <q-virtual-scroll
      class="q-pa-xl"
      :items="mentores"
      virtual-scroll-horizontal
    >
      <template v-slot="{ item }">
        <q-card class="q-ma-xl mycard">
          <q-img
            class="q-ma-md"
            :src="item.imagem"
            fit='cover'
            height="150px"
            width="150px"
          />

          <q-card-section>
            <div class="text-h6">{{ item.nome }}</div>
            <div class="text-subtitle2">{{item.descricao}}</div>
          </q-card-section>

        </q-card>
      </template>
    </q-virtual-scroll>
  </q-page>

  <q-page id='materiais' class="bg-white row">
    <div class="col-1 ">
      <div id="vertical" class="vertical-text col-8">
        <p class="text-black text-uppercase">Materiais</p>
      </div>

    </div>

    <div class="col-9 column  justify-center ">
      <p class="col-2 magenta   q-mt-xl q-mx-xl text-h4 text-uppercase">baixe aqui nossas cartilhas apresentadas pela nossa equipe</p>
      <div class="col-8 q-px-xl">
        <q-btn color="teal" rounded class="q-mx-md q-my-sm"  v-for="material in materiais" :key="material" :label='material' size="xl"></q-btn>
      </div>
    </div>
    <div class="col-2">
      <q-icon name='star' class="full-width full-height" color="primary" size="300px"></q-icon>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";
import { ref } from "vue";

export default defineComponent({
  name: "PageIndex",
  data: function () {
    return {
      materiais : [
        'Como construir mapas de narrativas',
        'Modelos de Mapa',
        'Guia para cada grupo baixar e construir a sua narrativa',
        'Gestão e Marketing',
        'Novas Economias: Banco Palma',
        'Fundo Rotativo Solidário do Fórum de Cooperativismo Popular'
      ],

      mentores: [
        { imagem: "images/Thiago Vinícius.jpg", nome: "THIAGO VINÍCIUS,", descricao: "fundador da Agência Popular Solano Trindade, é empreendedor social e liderança comunitária que propõe tecnologias sociais que colaboram para geração de renda através de startups focadas em desenvolver serviços e produtos que dialoguem com a qualidade de vida do morador da favela.", video: null },
        { imagem: "images/Dríade Aguiar.png", nome: "DRÍADE AGUIAR", descricao: "da Mídia Ninja, é co-fundadora e editora do Mídia Ninja, ativista do Fora do Eixo, feminista negra, militante body positive. Ela compartilhou com o laboratório alguns segredos da gestão e do monitoramento das redes sociais para a produção de conteúdo e disputa de narrativas.", video: null },
        { imagem: "images/Preto Zeze.jpg", nome: "PRETO ZEZÉ", descricao: "presidente da Central Única das Favelas (CUFA), fez a primeira mentoria do Labic 2021. Empresário, produtor musical e repórter. É o CEO e fundador do Laboratório de Inovação Social, onde trabalha questões próximas às do Labic. ", video: null },
        { imagem: "images/Raull Santiago.jpg", nome: "RAUL SANTIAGO", descricao: " é uma das principais lideranças da favela em nosso país. Fundador da Agência BRECHA e do Coletivo Papo Reto, é integrante de iniciativas e plataformas que versam sobre periferia, direitos humanos, juventude e desenvolvimento sustentável nas favelas.", video: null },
        { imagem: "images/Rene Silva.jpg", nome: "RENE SILVA", descricao: " é uma das principais lideranças da favela em nosso país. Fundador da Agência BRECHA e do Coletivo Papo Reto, é integrante de iniciativas e plataformas que versam sobre periferia, direitos humanos, juventude e desenvolvimento sustentável nas favelas.", video: null },
        { imagem: "images/Marcus Faustini.jpg", nome: "MARCUS FAUSTINI", descricao: "Marcus Faustinié criador da metodologia da Agência de Redes para Juventudes, que potencializa jovens de favelas e periferias a transformarem ideias em projetos de intervenção em seus territórios.", video: null },
        { imagem: "images/Joaquim melo.jpg", nome: "JOAQUIM MELO,", descricao: 'criador do Banco Palmas (@bancopalmas), empreendedor social criou a "socioeconomia solidária" em 1998, no Conjunto Palmeira, um bairro popular de Fortaleza (CE).', video: null },
        { imagem: "images/Flavia Macedo.png", nome: "FÁVIA MACÊDO", descricao: "é escritora, empreendedora social, vice-presidente do Educar+ (@projeto.educar.mais) e construtora de comunidade da Rede Muda Outras Economias (@mudaoutraseconomias).", video: null },
        { imagem: "images/Felipe Altenfelder,.jpg", nome: "FELIPE ALTENFELDER,", descricao: "gestor da Mídia Ninja e do Fora do Eixo, articulador do projeto S.O.M (Sistema Operacional da Música, plataforma de conteúdo e aceleração de oportunidades), e da plataforma 342 de ativismo.", video: null },
        { imagem: "images/Thiago Scherer.jpg", nome: "THIAGO SCHERER,", descricao: "fundador do Design Ativista (@designativista) e gestor da frente de design da Mídia NINJA e do coletivo Fora do Eixo (@foradoeixo).", video: null },
        { imagem: "images/Daniele Moura.jpg", nome: "DANIELE MOURA", descricao: "é editora do Maré de Notícias (@maredenoticias). É jornalista premiada e apaixonada por periferias e favelas do Brasil.", video: null },
        { imagem: "images/Felipe Caruso.jpg", nome: "FELIPE CARUSO", descricao: "Felipe Caruso, jornalista, consultor de crowdfunding e capacitor de fluxos. Foi coordenador de comunicação do Catarse e repórter na Folha de S. Paulo.", video: null },
        { imagem: "images/Bruno Duarte.jpeg", nome: "BRUNO F. DUARTE,", descricao: "é cineasta, pesquisador, performer e ativista do movimento negro LGBT. É criador da CABINE - Da galeria ao banheirão! , plataforma para a expansão de ideias sobre artistas negros/as LGBT.", video: null },
        { imagem: "images/Luís Otávio Ribeiro.jpg", nome: "OTÁVIO RIBEIRO,", descricao: "um dos co-fundadores do Catarse, plataforma pioneira e uma das maiores referências em financiamento coletivo no Brasil. ", video: null },
        { imagem: "images/AYRA.jpg", nome: "AYRA CONSULTORIA", descricao: "é uma Empresa Júnior de Gestão de Negócios vinculada à UFRJ. Possui 18 anos de mercado, +20 prêmios recebidos e tem como propósito entregar soluções personalizadas para o seu negócio e/ou projetos. ", video: null },
        { imagem: "images/oliver kornblihtt.png", nome: "OLIVER KORNBLIHTT", descricao: "fotógrafo, ativista e editor da mídia ninja. Integra o coletivo Fora do Eixo e é gestor da frente projeto da NINJA.", video: null },
        { imagem: "images/Adriano Belisário 1.jpg", nome: "ADRIANO BELISÁRIO", descricao: "é Coordenador da Escola de Dados na Open Knowledge Brasil e pesquisador do MediaLab UFRJ. ", video: null },
        { imagem: "images/Raissa Galvão.jpg", nome: "RAÍSA GALVÃO", descricao: "fundadora e coordenadora nacional da Mídia NINJA, além de editora das redes sociais e da editoria de opinião e meio ambiente.", video: null },
        { imagem: "images/Lori Regattieri.jpg", nome: "LORI REGATTIERI,", descricao: "Lori Regattieri,cientista de Dados, co-editora da revista DR e pesquisadora na ECO/UFRJ.", video: null },
      ],
      slide: ref("style"),
      ultimasMentorias: [
        "https://www.youtube.com/embed/XDmN6eIxOOw",
        "https://www.youtube.com/embed/BDSdW6HjFSA",
        "https://www.youtube.com/embed/q5FX5_kescM",
        "https://www.youtube.com/embed/NZppOfA6KWk",
      ],
      eixos: [
        {
          icon: "smartphone",
          title: "Mídias, Ações Virtuais e Diversidade",
          description:
            "Projetos, ações, aplicativos e tecnologias que apresentem iniciativas de comunicação em qualquer suporte e linguagem e que estimulem a diuversidade de conteúdos e de produtos de mídias.",
        },
        {
          icon: "pie_chart",
          title: "Tecnologias, Redes, Dados e Plataformas",
          description:
            "Iniciativas de desenvolvimento de plataformas, redes, aplicativos, programas, tecnologias abertas. Projetos de mineração, análise e visualização de dados.",
        },
        {
          icon: "auto_stories",
          title: "Formação",
          description:
            "Projetos, propostas, metodologias de formação e educação utilizando qualquer linguagem; formação em rede, formação livre, educação inclusiva, formação de agentes e multiplicadores, formação para a diversidade; educação e inovação.",
        },
        {
          icon: "business",
          title: "Economia e Cidadania",
          description:
            "Iniciativas em novas economias, sustentabilidade, financiamento colaborativo, empreendedorismo social, redes de proteção, inclusão, visibilidade, ampliação de direitos para a diversidade cultural, de gênero, religiosa, étnica, etc.",
        },
        {
          icon: "coronavirus",
          title: "Ações de enfrentamento a covid-19",
          description:
            "no campo da saúde, comunicação, da cultura, educacionais e em todos os campos do conhecimento, constituição de redes de apoio e solidariedade pós-pandemia.",
        },
        {
          icon: "add",
          title: "Outros temas",
          description: "",
        },
      ],
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

#vertical {
  height: 49.8vw;
  max-height: 80.8vh;
  border-left: 3px solid black;
  font-size: 5vw;
}

.vertical-text {
  writing-mode: vertical-rl;
  text-orientation: mixed;
  -webkit-transform: rotate(180deg);
  -moz-transform: rotate(180deg);
}

.vertical-text2 {
  writing-mode: vertical-rl;
  text-orientation: mixed;
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

.projeto2 {
  background-color: #8b50ff;
}

.mundo {
  background-color: #8b50ff;
}
.bgpurple {
  background-color: #8b50ff;
}

.purple {
  color: #8b50ff;
}

.eixos {
  background-color: #df71ff;
}

.color-primary {
  color: #00d3de;
}

.magenta {
  color: #ff4aa1;
}

.color-secondary {
  color: #df71ff;
}

.pink {
  color: #df71ff;
}

.bgpink {
  background-color: #df71ff;
}

.fill-text {
  font-size: 1.5vw;
}
.green {
  color: green;
}

#rounder {
  border-radius: 75px 75px;
  padding: 35px;
  text-align: center;
  background-color: #df71ff;
}

.yellow {
  color: rgb(255, 212, 51);
}

.bgyellow {
  background-color: rgb(255, 212, 51);
}

#rounder2 {
  border-radius: 75px 75px;
  padding: 20px;
  text-align: center;
  max-width: 20%;
  background-color: rgb(228, 77, 150);
}

#rounder3 {
  border-radius: 75px 75px;
  text-align: center;
  background-color: white;
}

.bgmagenta {
  background-color: rgb(228, 77, 150);
}

.ultralarge {
  font-size: 12rem;
  line-height: 1;
}

.ultralarge2 {
  font-size: 10rem;
  line-height: 1;
}

.mycard{
  min-width: 200px;
}


</style>
