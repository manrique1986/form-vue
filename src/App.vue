<template>
  <div id="app">
    <FormularioVue @agregarTabla="addUsuarioTabla" />
    <!-- <TableVue :usuarios="usuarios" /> -->
  </div>
</template>

<script>
import FormularioVue from "./components/FormularioVue.vue";
// import TableVue from "./components/FormularioVue.vue";

export default {
  name: "App",
  components: {
    FormularioVue,
    // TableVue,
  },

  data() {
    return {

      usuarios:[]

    };
  },



};
</script>

<style></style>
