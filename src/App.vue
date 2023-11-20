<template>
  <div class = "name">
    {{ name }}
  </div>
  <button class="btn btn-primary" @click="updateName">click</button>
</template>

<script setup>
import {ref} from "vue"
import {reactive} from "vue"

  const name = reactive({
    id: 1
  });

  const updateName = () => {
    name.id += 1;
  }

</script>

<style scoped>
</style>
