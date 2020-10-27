<template>
  <div>
    <FormGenerator :form="form" :handleSubmission="handleSubmission" />
  </div>
</template>

<script>
import FormGenerator from "./FormGenerator";
export default {
  name: "FormPage",
  created() {},
  data() {
    return {
      drawer: "hello world",
      form: [
        // form-title
        "Police Brutality Report Form",
        // form title end
        [
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
        ]
       
      ],
    };
  },
  props: {},
  methods: {
    handleSubmission() {},
  },

  components: {
    FormGenerator,
  },
};
</script>

<style lang="scss" scoped></style>
