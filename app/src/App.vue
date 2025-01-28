<template>
  <div>
    <TheHeader>

      <template v-slot:description>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Laborum vel eum ut fugit perferendis ad, cumque, quae porro totam praesentium laboriosam deserunt, dolorum et maxime quaerat molestiae nesciunt fugiat accusantium?</p>
      </template>
 
      Header content - Menu ...
    </TheHeader>
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";

export default {
  name: "App",
  components: { TheHeader },
  data() {
    return {};
  },

  beforeUpdate() {},
  updated() {},
  beforeCreate() {},
  created() {},
  beforeMount() {},
  mounted() {},
  beforeUnmount() {},
  unmounted() {},

  watch: {},

  computed: {},

  methods: {},
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
