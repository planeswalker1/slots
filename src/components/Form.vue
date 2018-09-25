<template>
  <div>
    <h1>Slots</h1>
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

</style>
