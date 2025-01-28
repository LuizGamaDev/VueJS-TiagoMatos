<template>
  <div>
    <TheHeader v-if="showHeader"/>
    <h1>Hello World !</h1>
    <br>
    <input 
    v-model="name"
    type="text"
    >
    {{ name }} <br>

    <button @click="showHeader = !showHeader">
      Ativar e desativar Header
    </button>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';

export default {
  name: "App",
  components: { TheHeader },
  data() {
    return {
      name: 'Jon Snow',
      showHeader: true,
    };
  },
    // Criação
      // Prepara o componente
      // Ajax, inicializar algumas variáveis
      // Não tem acesso ao template (DOM)
    // Montagem
      // Inicializar uma lib externa (new Lib())
      // Precisa de acesso ao template (DOM)
      // Tem acesso ao template (DOM)
    // Atualização
      // Debug
    // Desmontagem
      // Remover tudo o que for necessário (lib->destroy())
      // para liberar memória

      // HOOKS
      // beforeUpdate() {
      //   console.log('beforeUpdate', this.name)
      // },
      // updated() {
      //   console.log('updated', this.name)
      // },
      // beforeCreate() {
      //   console.log('beforeCreate');
      //   console.log('Estado:', this.name);
      //   console.log('DOM:', this.$el);
      // },
      // created() {
      //   console.log('created');
      //   console.log('Estado:', this.name);
      //   console.log('DOM:', this.$el);
      // },
      // beforeMount() {
      //   console.log('beforeMount');
      //   console.log('Estado:', this.name);
      //   console.log('DOM:', this.$el);
      // },
      // mounted() {
      //   console.log('mounted');
      //   console.log('Estado:', this.name);
      //   console.log('Estado:', this.name);
      // },
      // beforeUnmount() {
      //   console.log('beforeUnmount')
      // },
      // unmounted() {
      //   console.log('unmounted')
      // },


  watch: {
    
  },

  computed: {},

  methods: {
   
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 60px;
}
</style>
