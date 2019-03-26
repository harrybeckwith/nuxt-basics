<template>
  <p>A single user with ID: {{ $route.params.id }}</p>
</template>

<script>
export default {
  validate(data) {
    console.log(data);
    return data.params.id == 1;
  },
  layout: "users"
};
</script>

<style>
</style>
