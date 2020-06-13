<template>
  <div id="app">
    <table class="table table-striped">
      <thead>
        <tr>
          <th scope="col">Nombre</th>
          <th scope="col">Apellidos</th>
          <th scope="col">RUN</th>
          <th scope="col">Nacimiento</th>
          <th scope="col">Edad</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(item, index) in users" :key="index">
          <td>{{ item.nombre }}</td>
          <td>{{ item.apellido }}</td>
          <td>{{ item.rut }}</td>
          <td>{{ item.bday }}</td>
          <td>{{ item.age }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      users: [
        {
          nombre: "Carolina",
          apellido: "Herrera",
          rut: "17.937.565-6",
          bday: "15-09-1991",
          age: 28,
        },
        {
          nombre: "Lucero",
          apellido: "Herrera",
          rut: "14.6378.112-3",
          bday: "24-09-1991",
          age: 28,
        },
        {
          nombre: "Mauro",
          apellido: "Herrera",
          rut: "19.711.636-6",
          bday: "02-02-1998",
          age: 22,
        },
      ],
    };
  },
};
</script>
