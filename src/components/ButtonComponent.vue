<template>
  <q-btn :label="text" type="submit" :to="to" />
</template>

<script>
export default {
  name: 'ButtonComponent',
  props: {
    text: String,
    to: String,
  },
}
</script>

<style scoped lang="scss">
.q-btn {
  width: 100%;
  height: 32px;
  background-color: $btn-primary;
  color: $btn-text-color;
  border-radius: $btn-border-radius;
}
</style>
