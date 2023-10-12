<template>
  <q-drawer
    :model-value="drawer"
    show-if-above
    :mini="mini"
    @click.capture="drawerClick"
    :width="250"
    :breakpoint="500"
    bordered
    class="bg-blue-1"
  >
  </q-drawer>
</template>

<script>
import { ref } from "vue";
export default {
  name: "Drawer",
  props: ["drawer", "mini"],
  setup() {
    //variables
    const menu = ref([{}]);

    //finctions

    return {
      //variables
      menu,
      //functions
    };
  },
};
</script>
