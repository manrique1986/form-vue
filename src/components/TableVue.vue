<template>
  <table class="table table-success table-striped">
    <thead>
      <tr>
        <th>Nombre</th>
        <th>Edad</th>
        <th>Email</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="usuario in usuarios" :key="usuario">
        <td>{{ usuario.nombre }}</td>
        <td>{{ usuario.edad }}</td>
        <td>{{ usuario.email }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script>
export default {
  name: "TablaVue",

  props: {
    nombre: "",
    email: "",
    edad: "",
  },

  usuarios: []
};
</script>

<style>
.table {
  text-align: right;

  margin: 20px;
}
</style>
