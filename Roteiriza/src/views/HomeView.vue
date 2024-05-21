<script setup>

</script>


<template>
  <div class="container-fluid">
    <div class="content">
      <div class="map">
        <iframe 
          src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d30414.433160073808!2d-49.946820320885834!3d-22.2182830365842!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e0!3m2!1spt-BR!2sbr!4v1712085569850!5m2!1spt-BR!2sbr" 
          width="100%" 
          height="100%" 
          style="border:0;" 
          allowfullscreen="" 
          loading="lazy">
        </iframe>
      </div>
      <div class="table-container">
        <table class="table">
          <thead>
            <tr>
              <th scope="col">ID</th>
              <th scope="col">Destinatario</th>
              <th scope="col">Endereço</th>
              <th scope="col">Email</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <th scope="row">1</th>
              <td>Leonardo Caires</td>
              <td>Rua Guilherme Sheffer Netto 555 A </td>
              <td>leocaires03@gmail.com</td>
            </tr>
            <tr>
              <th scope="row">2</th>
              <td>Bruno Alves Demetrio</td>
              <td>Rua Almeida de Andrade 1181</td>
              <td>brunodemetriob@gmail.com</td>
            </tr>
            <tr>
              <th scope="row">3</th>
              <td>Felipe Augusto</td>
              <td>Rua Alcidez Nunes</td>
              <td>felipeaugusto123@gmail.com</td>
            </tr>
            <tr>
              <th scope="row">4</th>
              <td>Falecido Tubarão</td>
              <td>Rua Perdida no Santa Antonieta</td>
              <td>tutubarão@gmail.com</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
    <div class="main">
      <router-view></router-view>
    </div>
  </div>
</template>

<style scoped>
.container-fluid {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  min-height: 100vh; 
  margin: 0;
  padding: 0;
}

.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 80%; 
  max-width: 1200px; 
}

.map {
  width: 100%;
  margin-bottom: 15px;
}

.map iframe {
  width: 100%;
  height: 400px; 
  border: none;
}

.table-container {
  width: 100%;
}

.table {
  width: 100%;
  margin: 0;
}

.main {
  margin: 15px;
}
</style>