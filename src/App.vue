<script setup>
import { ref } from 'vue'
const mostrarDiv = ref(false)
</script>

<template>
  <div class="w-100 d-flex justify-content-around">
    <form action="/action_page.php" @submit.prevent="mostrarDiv = !mostrarDiv">
      <div class="form-floating mt-3 mb-3">
        <input
          type="text"
          class="form-control"
          v-model="name"
          placeholder="Enter nome"
          name="nome"
        />
        <label for="nome" class="form-label">Nome:</label>
      </div>
      <div class="form-floating mt-3 mb-3">
        <input
          type="email"
          class="form-control"
          v-model="email"
          placeholder="Enter email"
          name="email"
          colo
        />
        <label for="email" class="form-label">Email:</label>
      </div>
      <div class="form-floating mt-3 mb-3">
        <input
          type="password"
          class="form-control"
          v-model="pwd"
          placeholder="Enter password"
          name="pwd"
        />
        <label for="pwd" class="form-label">Senha:</label>
      </div>
      <div class="form-floating mt-3 mb-3">
        <input
          type="password"
          class="form-control"
          v-model="confSenha"
          placeholder="Enter confirm password"
          name="csenha"
        />
        <label for="csenha" class="form-label">Confirmar Senha:</label>
      </div>
      <div class="form-floating mt-3 mb-3">
        <input
          type="date"
          class="form-control"
          v-model="dataNasc"
          placeholder="Enter DataNascimento"
          name="dataNasc"
        />
        <label for="dataNasc" class="form-label">Data Nascimento: </label>
      </div>
      <div class="form-floating mt-3 mb-3">
        <input
          type="text"
          class="form-control"
          v-model="endereço"
          placeholder="Enter endereço "
          name="endereço"
        />
        <label for="endereço" class="form-label">Endereço:</label>
      </div>
      <div class="form-floating mt-3 mb-3">
        <input
          type="text"
          class="form-control"
          v-model="Cidade"
          placeholder="Enter cidade "
          name="Cidade"
        />
        <label for="Cidade" class="form-label">Cidade</label>
      </div>

      <div class="form-floating">
        <select class="form-select" v-model="estado" name="sellist">
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
        <textarea
          class="form-control"
          v-model="Hobbies"
          name="text"
          placeholder="Comment goes here"
        ></textarea>
        <label for="comment">Hobbies</label>
      </div>
      <div class="form-floating">
        <textarea
          class="form-control"
          v-model="LingProgramação"
          name="text"
          placeholder="Comment goes here"
        ></textarea>
        <label for="comment">Linguagens de Programação</label>
      </div>
      <div class="form-floating">
        <textarea
          class="form-control"
          v-model="Biografia"
          name="text"
          placeholder="Comment goes here"
        ></textarea>
        <label for="comment">Biografia</label>
      </div>
      <hr />
      <div class="Relembrar">
        <label class="form-check-label">
          <input class="form-check-input" type="checkbox" name="remember" /> Lembre-me
        </label>
        <hr />
        <button class="btn btn-danger" type="submit">Enviar</button>
      </div>
     
    </form>
    <div v-if="mostrarDiv">
        <p>Dados enviados com sucesso!</p>
        <p>Nome: {{ nome }}</p>
        <p>Email: {{ email }}</p>
        <p>Senha: {{ pwd }}</p>
        <p>Confirmação da Senha: {{ confSenha }}</p>
        <p>Data de Nascimento: {{ dataNasc }}</p>
        <p>Endereço: {{ endereço }}</p>
        <p>Cidade: {{ Cidade }}</p>
        <p>Estado: {{ estado }}</p>
        <p>Hobbies: {{ Hobbies }}</p>
        <p>Linguagens de Programação: {{ LingProgramação }}</p>
        <p>Biografia: {{ Biografia }}</p>
      </div>
  </div>
</template>

<style scoped>
body {
  background-color: aqua;
}
</style>
