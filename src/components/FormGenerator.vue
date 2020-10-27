<template>
  <div>
    <h1>Form Component goes here</h1>
    <h1 class="form-title">{{ form[0] }}</h1>
    


    <div v-for="forms in form[1]" :key="forms.label" class="=">
      <form>
       
        <label> {{ forms.label }}</label>
        <input :type="forms.type" />
      </form>
    </div>
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
    handleSubmission: Function,
    form: Array,
  },
  methods: {},
};
</script>

<style>
input {
  width: 400px;
  border-radius: 5px;
  border: 0.5px solid black;
  padding: 8px 10px;
  margin-bottom: 10px;
  margin-top: 5px;
}

label {
  display: block;
  margin-bottom: 10px;
  font-size: 16px;

  font-weight: 600;
}
</style>
