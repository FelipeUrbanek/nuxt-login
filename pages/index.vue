<template>
<section class="login">
  <div class="columns">
    <div id="esquerda" class="column is-6 is-flex esquerda">
      <h4>Bem-vindo de volta!!!</h4>
      <span>Mantenha se conectado conosco<br>
      estamos sempre em busca de novas soluções</span>
      <nuxt-link to="login"><button>Login</button></nuxt-link>
    </div>
    <div id="direita" class="column is-6 is-flex direita">
      <h2>Crie sua Conta</h2>
      <input type="text" placeholder="Nome">
      <input type="email" name="" id="" placeholder="E-mail">
      <input type="password" name="" id="" placeholder="Password">
      <button @click="funcao">Criar</button>
      

      

    </div>
  </div>
</section>
</template>

<script>
import Card from '~/components/Card'

export default {
  name: 'IndexPage',
  components: {
    Card
  },
methods: {
  funcao() {
    var div = document.getElementById("esquerda");
    console.log(div);
    div.style.display = "none";
}}}
</script>

<style lang="css">
@import url('https://fonts.googleapis.com/css2?family=Epilogue:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Rubik:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

* {
  
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Epilogue, sans-serif;
}

body{
  overflow: hidden;
}
.column{
  padding: 0px !important;
}

.esquerda{
  display: flex;
  flex-direction: column;
  height: 100vh;
  align-items: center;
  justify-content: center;
  background-color: #047e4b;
}
.esquerda h4{
  font-size: 3rem;
  font-weight: bold;
  color: rgb(255, 255, 255);
}

.esquerda button{
  padding: 10px 30px;
  border: solid 2px rgb(255, 255, 255);
  color: white;
  font-size: 1.5rem;
  font-weight: bold;
  background-color: transparent;
  border-radius: 15px;
}

.esquerda button:hover{
  cursor: pointer;
  background-color: transparent;
  color: rgb(206, 204, 204);
  border: solid 2px rgb(206, 204, 204);
  transform: scale(1.1);

}

.esquerda span{
  color: white;
  margin-bottom: 60px;
  font-style: lighter;
  font-weight: 200;
}
  
.direita{
  display: flex;
  flex-direction: column;
  height: 100vh;
  align-items: center;
  justify-content: center;

}

.direita h2{
  font-size: 3rem;
  font-weight: bold;
  color: #047e4b;
}

.direita input{
  background: #e2e2e2;
  width: 70%;
  height: 50px;
  margin: 10px 0px;
  border-radius: 15px;
  border: solid 3px #047e4b;
}

.direita input::placeholder{
  padding-left: 20px;
  color: #757373;
}
.direita button{
  padding: 10px 30px;
  border: solid 2px #047e4b;
  color: #ffffff;
  font-size: 1.5rem;
  font-weight: bold;
  background-color: #047e4b;
  border-radius: 15px;
}
.direita button:hover{
  cursor: pointer;
  transform: scale(1.1);
}

input ::target-text
{
  color: #047e4b;
}
</style>