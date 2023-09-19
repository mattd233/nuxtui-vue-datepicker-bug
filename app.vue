<script setup>
import VueDatePicker from '@vuepic/vue-datepicker';
import '@vuepic/vue-datepicker/dist/main.css'

const email = ref();
const date = ref();
</script>

<template>
  <UForm class="container">
    <UFormGroup label="Email" name="email">
      <UInput v-model="email" />
    </UFormGroup>
    <UFormGroup label="Date" name="password">
      <VueDatePicker v-model="date"></VueDatePicker>
    </UFormGroup>
    <UButton type="submit">
      Submit
    </UButton>
  </UForm>
</template>


<style>
.container {
  width: 200px;
}
</style>
