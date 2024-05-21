
<template>
    <div class="login-page">
    <div class="form">
      <div class="login-form" id="login-form">
        <p class="img"><img src="#" alt="" width="105px"></p>
        <input type="text" placeholder="E-mail..." id="txtEmail"/>
        <span class="error" id="errorEmail" hidden>Por favor, informe este campo.</span>
        <input type="password" placeholder="Senha..." id="txtSenha"/>
        <span class="error" id="errorSenha" hidden>Por favor, informe este campo.</span>
        <button onclick="login()">entrar</button>
      </div>
      <div id="loading" hidden>
        <h2>Carregando...</h2>
      <button onclick="cancel()">cancelar</button>
      </div>
    </div>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

body {  
  background: linear-gradient(90deg, rgb(245, 119, 119) 0%, rgb(153, 0, 0) 50%);
    font-family: "Poppins", sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;      
  }

.login-page {
  width: 360px;
  padding: 8% 0 0;
  margin: auto;
}

.form {
  position: relative;
  border-radius: 10px;
  z-index: 1;
  background: rgb(236, 108, 108);
  max-width: 360px;
  margin: 0 auto 100px;
  padding: 45px;
  text-align: center;
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.2), 0 5px 5px 0 rgba(0, 0, 0, 0.24);
}

.form, .img{
    padding-top: 6px;
}

.form input {
  font-family: "Poppins", sans-serif;
  outline: 0;
  border-radius: 10px;
  background: #f2f2f2;
  width: 100%;
  border: 0;
  margin: 0 0 15px;
  padding: 15px;
  box-sizing: border-box;
  font-size: 14px;
}

.form button {
  font-family: "Poppins", sans-serif;
  text-transform: uppercase;
  outline: 0;
  background: #ff0000;
  width: 100%;
  border: 0;
  padding: 15px;
  color: #ffffff;
  font-size: 14px;
  -webkit-transition: all 0.3 ease;
  transition: all 0.3 ease;
  cursor: pointer;
}

.form button:hover,.form button:active,.form button:focus {
  background: #e92424;
}

.container {
  position: relative;
  z-index: 1;
  max-width: 300px;
  margin: 0 auto;
}


.error {
  color: #ffffff;
  margin: -15px;
  padding-bottom: 5px;
}

</style>