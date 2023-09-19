<script setup>
import VueDatePicker from '@vuepic/vue-datepicker';
import '@vuepic/vue-datepicker/dist/main.css'

const date1 = ref();
const date2 = ref();
</script>

<template>
  <UForm class="container">
    <VueDatePicker v-model="date1"></VueDatePicker>
    <UFormGroup label="Date" name="password">
      <VueDatePicker v-model="date2"></VueDatePicker>
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
