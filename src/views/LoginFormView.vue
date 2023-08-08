<template>
  <div class="w3-container">
    <LoginForm/>
    <PageFooter/>
  </div>
</template>

<script>
// @ is an alias to /src
import LoginForm from '@/components/LoginForm.vue';
import PageFooter from '@/components/PageFooter.vue';

export default {
  name: 'NewAccFormView',
  components: {
    LoginForm,
    PageFooter
  }
}
</script>
