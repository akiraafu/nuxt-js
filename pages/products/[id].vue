<template>
  <div>
    <p>Product details for {{ id }}</p>
    <p>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Enim tempore
      delectus vitae, nesciunt itaque harum aliquam minus incidunt similique
      explicabo.
    </p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
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
