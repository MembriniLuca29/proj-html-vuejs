<script>
import mainFirstComponent from './mainFirstComponent.vue';
import mainSecondoComponent from './mainSecondComponent.vue';
import mainThirdComponent from './mainThirdComponent.vue';
import { store } from '../store.js';

export default {
  name: "mainsection",
  components: {
    mainFirstComponent,
    mainSecondoComponent,
    mainThirdComponent,
  },
  data() {
    return {
      store,
    };
  },
};

</script>

<template>
<mainFirstComponent/>
<mainSecondoComponent/>
<mainThirdComponent/>
</template>

<style lang="scss" scoped>

</style>