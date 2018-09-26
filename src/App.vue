<template>
  <div class="container">
    <appForm>
      <template slot="form-header">
        <h3>Vue Slots Form</h3>
        <p>Information that has been passed from a slot</p>
      </template>
      <template slot="form-fields">
        <div class="group">
          <label for="username">Username: </label>
          <input id="username" type="text" placeholder="username" required>
        </div>
        <div class="group">
          <label for="password">Password: </label>
          <input id="password" type="password" placeholder="password" required>
        </div>
      </template>
      <template slot="form-controls">
        <button v-on:click="handleSubmit">Submit</button>
      </template>
      <template slot="form-links">
        <ul>
          <li><a href="https://github.com/planeswalker1">My GitHub</a></li>
          <li><a href="https://planeswalker1.github.io/">My Website</a></li>
          <li><a href="https://github.com/colorlessenergy">Cool GitHub</a></li>
          <li><a href="https://colorlessenergy.github.io/">Cool Website</a></li>
        </ul>
      </template>
    </appForm>
  </div>
</template>

<script>
import Form from './components/Form.vue'

export default {
  components: {
    appForm: Form
  },
  data: function () {
    return {

    };
  },
  methods: {
    handleSubmit: function (event) {
      event.preventDefault();
      console.log('form submitted');
    }
  }
}
</script>

<style>
  html {
    box-sizing: border-box;
  }

  *,
  *:before,
  *:after {
    box-sizing: inherit;
  }

  body {
    font-family: sans-serif;
    margin: 0;
  }

  .container {
    margin: 0 auto;
    max-width: 1360px;
  }
</style>
