<template>
  <div>
    <h2>About</h2>
    <p>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Enim tempore
      delectus vitae, nesciunt itaque harum aliquam minus incidunt similique
      explicabo.
    </p>
    <p>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Enim tempore
      delectus vitae, nesciunt itaque harum aliquam minus incidunt similique
      explicabo.
    </p>
    <div>{{ data }}</div>
  </div>
</template>

<script setup>
const { data } = await useFetch("/api/ninja?name=akira", {
  method: "post",
  body: {
    age: 30,
  },
});
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
