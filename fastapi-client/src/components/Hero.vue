<template>
  this is test
</template>

<script setup>
import axios from "axios"
import { onMounted } from "vue";

const fetchData = async () => {
  const response = await axios.get('/')
  const { data } = response;
  console.log("response", data);
}

onMounted(() => {
  fetchData()
})
</script>

