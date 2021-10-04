<template>
  <ul>
    <li v-for="list in lists" :key="list.number">
      <h5 @click="$router.push(`/detail/${list.number}`)">{{ list.title }}</h5>
      <p>{{ list.content }}</p>
      <span>{{ list.date }}</span>
    </li>
  </ul>
</template>

<script>
export default {
  name: "List",
  props: {
    lists: Array,
  },
};
</script>

<style></style>
