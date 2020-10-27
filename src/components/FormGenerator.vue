<template>
  <div>
    <h1>Form Component goes here</h1>

    <div v-for="forms in form" :key="forms.label">
      <input :type="forms.type" />
    </div>

    {{ drawer }}

    {{ form }}
  </div>
</template>

<script>
export default {
  name: "FormGenerator",
  created() {},
  data() {
    return {};
  },
  props: {
    drawer: String,
    form: Array,
  },
  methods: {},
};
</script>

<style lang="scss" scoped></style>
