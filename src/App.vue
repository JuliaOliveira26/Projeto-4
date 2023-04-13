<script setup>

import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap'
import {ref} from 'vue'

const mostrar = ref(true)
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
<div class="form-floating mt-3 mb-3" >
  <input type="text" class="form-control" id="Cidade" placeholder="Enter cidade " name="Cidade">
  <label for="Cidade" class="form-label">Cidade</label>
</div>

 <div class="form-floating" >
  <select class="form-select" id="sel1" name="sellist">
  <option value="Acre">AC</option>
  <option value="Alagoas">AL</option>
  <option value="Amapá">AP</option>
  <option value="Amazonas">AM</option>
  <option value="Bahia">BH</option>
  <option value="Ceará">CE</option>
  <option value="Distrito Federal">DF</option>
  <option value="Espírito Santo">ES</option>
  <option value="Goiás">GO</option>
  <option value="Maranhão">MA</option>
  <option value="Mato Grosso">MT</option>
  <option value="Mato Grosso do Sul">MS</option>
  <option value="Minas Gerais">MG</option>
  <option value="Pará">PA</option>
  <option value="Paraíba">PB</option>
  <option value="Paraná">PR</option>
  <option value="Pernambuco">PE</option>
  <option value="Piaui">PI</option>
  <option value="Rio de Janeiro">RJ</option>
  <option value="Rio Grande do Norte">RN</option>
  <option value="Rio Grande do Sul">RS</option>
  <option value="Rondônia">RO</option>
  <option value="Roraima">RR</option>
  <option value="Santa Catarina">SC</option>
  <option value="São Paulo">SP</option>
  <option value="Sergipe">SE</option>
  <option value="Tocantins">TO</option>  
</select>
  <label for="sel1" class="form-label">Selecione Estado :</label>
</div>

<div class="form-floating">
  <textarea class="form-control" id="comment" name="text" placeholder="Comment goes here"></textarea>
  <label for="comment">Hobbies</label>
</div>
<div class="form-floating">
  <textarea class="form-control" id="comment" name="text" placeholder="Comment goes here"></textarea>
  <label for="comment">Linguagens de Programação</label>
</div>
<div class="form-floating">
  <textarea class="form-control" id="comment" name="text" placeholder="Comment goes here"></textarea>
  <label for="comment">Biografia</label>
</div>
  <div class="Relembrar">
    <label class="form-check-label">
      <input class="form-check-input" type="checkbox" name="remember"> Lembre-me 
    </label>
  </div>
  <button type="submit" class="btn btn-primary">Enviar</button>
  <button class="btn btn-outline-dark" @click="mostrar = !mostrar"> Mostrar/esconder</button>
  <div v-if="mostrar">form action="/action_page.php">
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
<div class="form-floating mt-3 mb-3" >
  <input type="text" class="form-control" id="Cidade" placeholder="Enter cidade " name="Cidade">
  <label for="Cidade" class="form-label">Cidade</label>
</div>

 <div class="form-floating" >
  <select class="form-select" id="sel1" name="sellist">
  <option value="Acre">AC</option>
  <option value="Alagoas">AL</option>
  <option value="Amapá">AP</option>
  <option value="Amazonas">AM</option>
  <option value="Bahia">BH</option>
  <option value="Ceará">CE</option>
  <option value="Distrito Federal">DF</option>
  <option value="Espírito Santo">ES</option>
  <option value="Goiás">GO</option>
  <option value="Maranhão">MA</option>
  <option value="Mato Grosso">MT</option>
  <option value="Mato Grosso do Sul">MS</option>
  <option value="Minas Gerais">MG</option>
  <option value="Pará">PA</option>
  <option value="Paraíba">PB</option>
  <option value="Paraná">PR</option>
  <option value="Pernambuco">PE</option>
  <option value="Piaui">PI</option>
  <option value="Rio de Janeiro">RJ</option>
  <option value="Rio Grande do Norte">RN</option>
  <option value="Rio Grande do Sul">RS</option>
  <option value="Rondônia">RO</option>
  <option value="Roraima">RR</option>
  <option value="Santa Catarina">SC</option>
  <option value="São Paulo">SP</option>
  <option value="Sergipe">SE</option>
  <option value="Tocantins">TO</option>  
</select>
  <label for="sel1" class="form-label">Selecione Estado :</label>
</div>

<div class="form-floating">
  <textarea class="form-control" id="comment" name="text" placeholder="Comment goes here"></textarea>
  <label for="comment">Hobbies</label>
</div>
<div class="form-floating">
  <textarea class="form-control" id="comment" name="text" placeholder="Comment goes here"></textarea>
  <label for="comment">Linguagens de Programação</label>
</div>
<div class="form-floating">
  <textarea class="form-control" id="comment" name="text" placeholder="Comment goes here"></textarea>
  <label for="comment">Biografia</label>
</div>
  <div class="Relembrar">
    <label class="form-check-label">
      <input class="form-check-input" type="checkbox" name="remember"> Lembre-me 
    </label>
  </div> </div>

  
</form>

</template>

<style scoped>

</style>
