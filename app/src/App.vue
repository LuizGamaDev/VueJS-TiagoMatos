<template>
  <div>
    <div>
      One-way data binding <br />
      Two-way data binding <br />
      v-model -> formulários
    </div>

    <br /><br />

    <div>
      <label>Nome</label>
      <br />
      <input v-model="name" type="text" /> <br />
      {{ name }}
    </div>

    <br /><br />

    <div>
      <label>Sports</label> <br />
      <select v-model="sports">
        <option value="">Escolha</option>
        <option value="futebol">Futebol</option>
        <option value="skate">Skate</option>
        <option value="tenis">Tenis</option>
      </select>
      <br />
      {{ sports }}
    </div>

    <br /><br />

    <div>
      <label>Newsletter</label> <br />
      <input v-model="newsletter" type="radio" value="Sim" /> Sim

      <input v-model="newsletter" type="radio" value="Não" /> Não <br />
      {{ newsletter }}
    </div>

    <br /><br />

    <div>
      <label>Contrato</label> <br />
      <input v-model="contract" type="checkbox" /> Aceita os nossos termos...
      <br />
      {{ contract }}
    </div>

    <br><br>

    <div>
      <label>Clubes de Lisboa</label> <br />
      <input v-model="clubes" type="checkbox" value="Sporting CP" /> Sporting CP
      <input v-model="clubes" type="checkbox" value="SL Benfica" /> SL Benfica
      <input v-model="clubes" type="checkbox" value="FC Porto" /> FC Porto <br />
      {{ clubes }}
    </div>
  </div>

  <br><br>

  <div>
    <label>Nome Completo</label> <br>
    <input v-model="fullName" type="text"> <br>
    {{ fullName }} <br>
    <select v-model="gender">
      <option value="male">Masculino</option>
      <option value="female">Feminino</option>
    </select> <br>
    {{ gender }}
  </div>

  <br><br>

  <div>
    <label>Hobbies</label> <br>
    <input v-model="hobbies" type="checkbox" value="Desporto"> Desporto
    <input v-model="hobbies" type="checkbox" value="Leitura"> Leitura
    <input v-model="hobbies" type="checkbox" value="Música"> Música
    <input v-model="hobbies" type="checkbox" value="Viagem"> Viagem
    <br>
    {{ hobbies }}
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "John Snow",
      sports: "",
      newsletter: "Sim",
      contract: false,
      clubes: [],
      fullName: '',
      gender: 'Escolha o género',
      hobbies: [],
    };
  },
};
</script>

<style>
.title {
  font-size: 20px;
  color: blue;
}
.title-home {
  font-size: 30px;
  color: darkolivegreen;
}
.text {
  color: brown;
}
.text-home {
  color: blueviolet;
}
.users-items {
  background-color: #2c3e50;
  color: white;
  margin: 0 0 4px 0;
  padding: 3px 6px;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 60px;
}
</style>
