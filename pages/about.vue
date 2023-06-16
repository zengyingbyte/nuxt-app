<template>
  <div>
    <h2>About</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum,
      voluptates illo maiores dolor possimus laboriosam ut numquam blanditiis
      velit culpa?
    </p>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum,
      voluptates illo maiores dolor possimus laboriosam ut numquam blanditiis
      velit culpa?
    </p>
    <div>{{ data }}</div>
  </div>
</template>

<script lang="ts" setup>
const { data } = await useFetch("/api/currency/CNY");
</script>

<style scoped>
h2 {
  margin-bottom: 20px;
  font-size: 36px;
}

p {
  margin: 20px 0;
}
</style>