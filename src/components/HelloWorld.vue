<script lang="tsx">
import { ref, defineComponent } from "vue";
import { VBtn, VIcon } from "vuetify/components";

export default defineComponent({
  name: "HelloWorld",
  props: {
    msg: String,
  },
  setup(props) {
    const count = ref(0);

    return () => (
      <>
        <h1>{props.msg}</h1>

        <p>
          Recommended IDE setup:
          <a href="https://code.visualstudio.com/" target="_blank">
            VSCode
          </a>
          +
          <a href="https://github.com/johnsoncodehk/volar" target="_blank">
            Volar
          </a>
        </p>

        <p>
          See <code>README.md</code> for more information.
        </p>

        <p>
          <a href="https://vitejs.dev/guide/features.html" target="_blank">
            Vite Docs
          </a>
          |
          <a href="https://v3.vuejs.org/" target="_blank">
            Vue 3 Docs
          </a>
        </p>

        <VBtn onClick={() => count.value++}>
          <VIcon left>bolt</VIcon>
          count is: {count.value}
        </VBtn>
        <p>
          Edit
          <code>components/HelloWorld.vue</code> to test hot module replacement.
        </p>
      </>
    );
  },
});
</script>

<style scoped>
a {
  color: #42b983;
}

label {
  margin: 0 0.5em;
  font-weight: bold;
}

code {
  background-color: #eee;
  padding: 2px 4px;
  border-radius: 4px;
  color: #304455;
}
</style>
