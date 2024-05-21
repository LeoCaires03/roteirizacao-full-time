<template>
    <div class="container">
        <div class="form">
            <div>
                <p class="img"><img src="#" alt="" width="105px"></p>
                <h2><b>Cadastrar Motorista</b></h2>
            </div>
            <form>
                <div>
                    <label><b>Nome</b></label>
                    <input type="text" name="saida" id="saida">
                </div>
                <div>
                    <label><b>CPF</b></label>
                    <input type="number" name="car" id="car">
                </div>
                <div>
                    <label><b>CNH</b></label>
                    <input type="number" name="placa" id="placa">
                </div>
                <div>
                    <label><b>Telefone</b></label>
                    <input type="number" name="saida" id="saida">
                </div>
                <div>
                    <label><b>Endereço</b></label>
                    <input type="text" name="saida" id="saida">
                </div>
                <div>
                    <label><b>Data de Nascimento</b></label>
                    <input type="datetime-local" name="data" id="data">
                </div>
                <button onclick="direciona()" type="button" class="btn btn-danger"><i class="bi bi-person-add"></i> Cadastrar</button>
            </form> 
        </div>
    </div>
</template>

<style>
template{
    background: linear-gradient(90deg, rgb(245, 119, 119) 0%, rgb(153, 0, 0) 50%);
    font-family: "Roboto", sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale; 
}

.container{
    width: 500px;
    padding: 8% 0 0;
    margin: auto
}

.form {
  position: relative;
  z-index: 1;
  background: #FFFFFF;
  max-width: 500px;
  margin: 0 auto 100px;
  padding: 45px;
  text-align: center;
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.2), 0 5px 5px 0 rgba(0, 0, 0, 0.24);
}

.form input {
  font-family: "Roboto", sans-serif;
  outline: 0;
  background: #f2f2f2;
  width: 100%;
  border: 0;
  margin: 0 0 15px;
  padding: 15px;
  box-sizing: border-box;
  font-size: 14px;
}

.form button {
  font-family: "Roboto", sans-serif;
  text-transform: uppercase;
  outline: 0;
  width: 50%;
  border: 0;
  padding: 15px;
  color: #FFFFFF;
  font-size: 14px;
  -webkit-transition: all 0.3 ease;
  transition: all 0.3 ease;
  cursor: pointer;
}

.form button:hover,.form button:active,.form button:focus {
  background: #ec4242;
}
</style>