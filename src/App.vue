<script>
export default {
  mounted() {
    const el = document.getElementById('programming-languages');
    const instances = M.Chips.init(el, {
      placeholder: 'Enter a tag',
      secondaryPlaceholder: 'Add a Tag',
      data: [
        { tag: 'HTML' },
        { tag: 'CSS' },
        { tag: 'JavaScript' },
      ],
      autocompleteOptions: {
        data: {
          'HTML': null,
          'CSS': null,
          'JavaScript': null,
          'Python': null,
          'SQL': null,
        },
        limit: Infinity,
        minLength: 1,
      }
    });
  }
}
</script>

<template>
  <div class="container">
    <div class="row">
      <div class="col s6">
        <div id="programming-languages" class="chips input-field">
          <input class="input">
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
</style>
