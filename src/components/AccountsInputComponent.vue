<template>
  <q-input
    class="rounded-borders"
    :type="type"
    filled
    v-model="name"
    :label="lable"
    lazy-rules
    :rules="[(val) => (val && val.length > 0) || 'Please type something']"
  />
</template>

<script>
export default {
  name: 'AccountsInputComponent',
  props: {
    lable: String,
    type: String,
  },
}
</script>

<style scoped lang="scss">
.inputAccount {
  width: 100%;
  height: 32px;
  border-radius: $input-border-radius;
  background-color: $input-primary;
  color: $input-text-color;
  padding: 0;
}
</style>
