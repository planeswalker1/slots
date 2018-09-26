<template>
  <div>
    <h1>Please fill out our form...</h1>
    <form class="form" action="">
      <div class="form__header">
        <slot name="form-header"></slot>
      </div>
      <div class="form__fields">
        <slot name="form-fields"></slot>
      </div>
      <div class="form__controls">
        <slot name="form-controls"></slot>
      </div>
      <div class="form__links">
        <slot name="form-links"></slot>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  data: function () {
    return {

    };
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1,
  form {
    margin: 0 auto;
    max-width: 600px;
  }

  h1 {
    margin-top: 1em;
  }

  .form__header,
  .form__fields,
  .form__controls {
    margin: 10px 0;
    padding: 5px;
  }

  /* form control styles */
  .group {
    margin-bottom: 10px;
  }

  label {
    display: inline-block;
    margin-bottom: .5em;
  }

  input {
    background-color: #fff;
    background-clip: padding-box;
    border: 1px solid #ced4da;
    border-radius: .25em;
    color: #495057;
    display: block;
    font-size: 1em;
    width: 300px;
    line-height: 1.5;
    padding: .375em .75em;
    transition: border-color .15s ease-in-out,box-shadow .15s ease-in-out;
  }

  input:focus {
    background-color: #fff;
    border-color: #80bdff;
    box-shadow: 0 0 0 0.2em rgba(0,123,255,.25);
    color: #495057;
    outline: 0;
  }

  button {
    background-color: #007bff;
    border: 1px solid transparent;
    border-color: #007bff;
    border-radius: .25em;
    color: #fff;
    display: inline-block;
    font-size: 1em;
    font-weight: 400;
    line-height: 1.5;
    padding: .375em .75em;
    text-align: center;
    transition: color .15s ease-in-out,background-color .15s ease-in-out,border-color .15s ease-in-out,box-shadow .15s ease-in-out;
    user-select: none;
    -webkit-user-select: none;
    -moz-user-select: none;
    -ms-user-select: none;
    vertical-align: middle;
    white-space: nowrap;
  }

  button:hover {
    background-color: #0069d9;
    border-color: #0062cc;
    color: #fff;
    cursor: pointer;
  }

  button:focus {
    outline: 0;
    box-shadow: 0 0 0 0.2em rgba(0,123,255,.5);
  }
  /* link styles */
  ul {
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;
    width: 100%;
  }

  li {
    margin-right: 10px;
  }

  a {
    background-color: transparent;
    color: #007bff;
    text-decoration: none;
  }

  a:hover {
    color: #0056b3;
    text-decoration: underline;
  }
</style>
