<template>
  <h1>{{ msg }}</h1>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { helloService } from '/@/service';

export default defineComponent({
  name: 'HelloWorld',
  setup: () => {
    return {
      msg: helloService()
    };
  }
});
</script>
