<template>
    <div>
        <img alt="Vue logo" src="@/assets/logo.png">
      <h1 class="text-center">Tabla de Usuarios</h1>
      <table class="table table-sm">
          <thead>
              <tr>
                  <th>#</th>
                  <th>Nombre</th>
                  <th>Apellido</th>
                  <th>RUN</th>
                  <th>Fecha Nacimiento</th>
                  <th>Edad</th>
              </tr>
          </thead>
          <tbody v-for="(item,clave) in usuario" :key="clave">
              <tr>
                  <td>{{item.id}}</td>
                  <td>{{item.nombre}}</td>
                  <td>{{item.apellido}}</td>
                  <td>{{item.run}}</td>
                  <td>{{item.nacimiento}}</td>
                  <td>{{item.edad}}</td>
              </tr>
              <!-- <tr>
                  <td>{{usuario[1].id}}</td>
                  <td>{{usuario[1].nombre}}</td>
                  <td>{{usuario[1].apellido}}</td>
                  <td>{{usuario[1].run}}</td>
                  <td>{{usuario[1].nacimiento}}</td>
                  <td>{{usuario[1].edad}}</td>
              </tr>
              <tr>
                  <td>{{usuario[2].id}}</td>
                  <td>{{usuario[2].nombre}}</td>
                  <td>{{usuario[2].apellido}}</td>
                  <td>{{usuario[2].run}}</td>
                  <td>{{usuario[2].nacimiento}}</td>
                  <td>{{usuario[2].edad}}</td>
              </tr> -->
          </tbody>
      </table>
  </div>
</template>

<script>
    export default {
    name: 'PrimerVueJsCli',
    data()
        { return {
            usuario:
            [
                {id:1, nombre:'Mark', apellido:'Otto', run:'22.543.987-k', nacimiento:'12-04-87', edad:"34"},
                {id:2, nombre:'Jacob', apellido:'Thornton', run:'18.987.768-5', nacimiento:'12-02-07', edad:"82"},
                {id:3, nombre:'Larry', apellido:'Bird', run:'21.564.876-0', nacimiento:'12-08-97', edad:"47"}
            ]
            }
        }    
}
</script>

<style scoped>
th {
    font-size: small;
}
td {
    font-size: small;
}
</style>