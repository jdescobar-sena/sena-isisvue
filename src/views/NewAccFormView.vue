<template>
  <div class="w3-container">
    <NewAccForm/>
    <PageFooter/>
  </div>
</template>

<script>
// @ is an alias to /src
import NewAccForm from '@/components/NewAccForm.vue';
import PageFooter from '@/components/PageFooter.vue';

export default {
  name: 'NewAccFormView',
  components: {
    NewAccForm,
    PageFooter
  }
}
</script>
