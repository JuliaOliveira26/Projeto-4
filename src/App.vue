<script setup>

import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap'
</script>

<template>
  <form action="/action_page.php">
    <div class="form-floating mt-3 mb-3">
      <input type="text" class="form-control" id="nome" placeholder="Enter nome" name="nome">
       <label for="nome" class="form-label">Nome:</label>
    </div>
  <div class="form-floating mt-3 mb-3">
  <input type="email" class="form-control" id="email" placeholder="Enter email" name="email">
      <label for="email" class="form-label">Email:</label>
  </div>
  <div class="form-floating mt-3 mb-3">
  <input type="password" class="form-control" id="pwd" placeholder="Enter password" name="pwd">
      <label for="pwd" class="form-label">Senha:</label>
  </div>
  <div class="form-floating mt-3 mb-3">
  <input type="password" class="form-control" id="csenha" placeholder="Enter confirm password" name="csenha">
      <label for="csenha" class="form-label">Confirmar Senha:</label>
  </div>
  <div class="form-floating mt-3 mb-3">
 <input type="date" class="form-control" id="dataNasc" placeholder="Enter DataNascimento" name="dataNasc">
       <label for="dataNasc" class="form-label">Data Nascimento: </label>
  </div>
  <div class="form-floating mt-3 mb-3">
    <input type="text" class="form-control" id="endereço" placeholder="Enter endereço " name="endereço">
    <label for="endereço" class="form-label" >Endereço:</label>
    
  </div>
  <div class="Relembrar">
    <label class="form-check-label">
      <input class="form-check-input" type="checkbox" name="remember"> Lembre-me 
    </label>
  </div>
  <button type="submit" class="btn btn-primary">Enviar</button>
</form>
</template>

<style scoped>

</style>
