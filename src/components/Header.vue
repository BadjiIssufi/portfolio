<template>
  <div
    id="header"
    class="container">
    <header
      class="header">
      <h1 class="title bg-color white-text z-depth-3">
        {{ title }}
      </h1>
      <blockquote
        v-if="apresentation"
        class="title grey z-depth-3 lighten-5">
        {{ apresentation }}
      </blockquote>
    </header>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    title: {
      type: String,
      required: false,
      default: null
    },
    apresentation: {
      type: String,
      required: false,
      default: null
    }
  }
}
</script>

<style scoped>

.title{
  font-weight: 100;
  padding: 3%;
  text-align: left;
}

h1.title{
  text-transform: uppercase;
  font-size: 2.5rem;
}

</style>
