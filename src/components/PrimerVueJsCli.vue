<template>
    <div>
        <img alt="Vue logo" src="@/assets/logo.png">
      <h1 class="text-center">Tabla de Usuarios</h1>
      <table class="table table-striped">
          <thead>
              <tr>
                  <th>#</th>
                  <th>Nombre</th>
                  <th>Apellido</th>
                  <th>RUN</th>
                  <th>Fecha de Nacimiento</th>
                  <th>Edad</th>
              </tr>
          </thead>
          <tbody>
              <tr>
                  <td>{{usuario[0].id}}</td>
                  <td>{{usuario[0].nombre}}</td>
                  <td>{{usuario[0].apellido}}</td>
                  <td>{{usuario[0].run}}</td>
                  <td>{{usuario[0].nacimiento}}</td>
                  <td>{{usuario[0].edad}}</td>
              </tr>
              <tr>
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
              </tr>
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