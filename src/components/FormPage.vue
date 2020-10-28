<template>
  <div class="container">
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
      formData: {},
      form: [
        // form-title
        { title: "Police Brutality Report Form" },
        [
          {
            name: "name",
            label: "What is the name of the officer in question?",
            type: "text",
          },
          {
            name: "date",
            label: "When was the date of the incident?",
            type: "date",
          },
          {
            name: "number",
            label: "How much is the bribe that was paid?",
            type: "number",
          },
        ],
        //button
        { buttontitle: "Submit" },
      ],
    };
  },
  props: {},
  methods: {
 
  },

  components: {
    FormGenerator,
  },
};
</script>

<style >



</style>
