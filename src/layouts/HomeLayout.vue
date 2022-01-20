<template>
  <q-layout view="lHh lpr lFf">
    <q-header elevated class="bg-primary text-accent">
      <q-toolbar>
        <q-toolbar-title>
          <q-img
            class="q-ma-md"
            width="200px"
            alt="Inovação Cidadã"
            src="../../public/icons/logo.png"
          />
        </q-toolbar-title>
        <div class="gt-md">
          <q-btn
            flat
            v-for="link in links"
            :key="link"
            :label="link"
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
        "AO Vivo",
        "O Projeto",
        "Inscrições",
        "Ações Participantes",
        "Programação",
        "Mentores e Colabs",
        "Materiais",
        "Edições Anteriores",
        "Equipe",
      ],
    };
  },
  setup() {},
});
</script>
