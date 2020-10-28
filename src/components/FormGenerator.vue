<template>
  <div>
    <h1 class="form-title">{{ form[0].title }}</h1>
    <div>
      <form
        @submit.prevent="
          {
            handleSubmission;
          }
        "
      >
        <div v-for="forms in form[1]" :key="forms.label">
          <label> {{ forms.label }}</label>
          <input :type="forms.type" @change="handleSubmission" required />
        </div>
        <button class="btn" type="submit">{{ form[2].buttontitle }}</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "FormGenerator",

  data() {
    return {};
  },

  created: {},

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

.btn {
  outline: none;
  border: none;
  padding: 12px 14px;
  background-color: grey;
  border-radius: 5px;
  color: #fff;
  cursor: pointer;
}
</style>
