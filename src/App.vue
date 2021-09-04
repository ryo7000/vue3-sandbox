<script lang="tsx">
import { defineComponent } from "vue";
import logo from "./assets/logo.png";
import HelloWorld from "./components/HelloWorld.vue";
import { VApp, VMain } from "vuetify/components";

export default defineComponent({
  name: "App",
  setup() {
    return () => (
      <>
        <VApp>
          <VMain>
            <img alt="Vue logo" src={logo} />
            <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" />
          </VMain>
        </VApp>
      </>
    );
  },
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
