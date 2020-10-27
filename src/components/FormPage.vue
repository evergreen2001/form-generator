<template>
  <div>
    <FormGenerator  :form="form"  :drawer="drawer"/>
  </div>
</template>

<script>
import FormGenerator from "./FormGenerator";
export default {
  name: "FormPage",
  created() {},
  data() {
    return {
      cool:'good' , 
      drawer:"hello world",
      form: [
        {
          label: "What is the name of the officer in question?",
          type: "text",
        },
        {
          label: "When was the date of the incident?",
          type: "date",
        },
        {
          label: "How much is the bribe that was paid? (optional)",
          type: "number",
        },
      ],
    };
  },
  props: {},
  methods: {},

  components: {
    FormGenerator,
  },
};
</script>

<style lang="scss" scoped></style>
