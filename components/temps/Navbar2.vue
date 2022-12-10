<template>
  <div v-for="(model, index) in models" :key="index">
    <nuxt-link :to="model.path">
      {{ model.name }}
    </nuxt-link>
  </div>
</template>

<script>
export default {
  props: {
    path: {
      type: String,
      default: "/test",
    },
    name: {
      type: String,
      default: "test",
    },
  },
  data() {
    return {
      models: [
        {
          name: "home",
          path: "/",
        },
        {
          name: "menu",
          path: "/menu",
        },
        {
          name: "test",
          path: "/test",
        },
      ],
    };
  },
};
</script>

<style></style>
