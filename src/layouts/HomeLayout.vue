<template>
  <q-layout view="lHh lpr lFf">
    <q-header elevated >
      <q-toolbar class="bg-primary text-accent">
          <q-btn flat to="/#home">
          <q-img
            class="q-ma-md"
            width="200px"
            alt="Inovação Cidadã"
            src="../../public/icons/logo.png"
          /></q-btn>
          <q-space />
          <div>
          <q-btn
            flat
            v-for="link in links"
            :key="link.label"
            :label="link.label"
            :to="link.hash"
            class="text-no-wrap"
          >
          </q-btn>
          </div>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "MainLayout",
  data: function () {
    return {
      links: [
        {label: "AO Vivo", hash:"#aovivo"},
        {label: "O Projeto", hash:"#oprojeto"},
        {label: "Inscrições", hash:"#inscricoes"},
        {label: "Ações Participantes", hash:"#acoesparticipantes"},
        {label: "Programação", hash:"#programacao"},
        {label: "Edições Anteriores", hash:"#edicoesanteriores"},
        {label: "Mentores e Colabs", hash:"#mentores"},
        {label: "Materiais", hash:"#materiais"},
      ],
    };
  },
  setup() {},
    methods:{
  },
});
</script>
