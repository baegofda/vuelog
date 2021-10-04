<template>
  {{ $route.params.id }}
  <h4>상세 페이지임다</h4>
  <h5>{{ lists[$route.params.id].title }}</h5>
  <h5>{{ lists[$route.params.id].content }}</h5>
  <router-view></router-view>
</template>

<script>
export default {
  name: "Detail",
  props: {
    lists: Array,
  },
};
</script>

<style></style>
