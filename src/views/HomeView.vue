<template>
  <div class="home">
    <main>
      <section>
        <card-component direction="column" title="Teste" imageAlt="Teste" />
      </section>
      <section>
        
      </section>
    </main>
  </div>
</template>

<script>
import CardComponent from "@/components/CardComponent.vue";
export default {
  name: "HomeView",
  components: {
    CardComponent,
  },
};
</script>

<style scoped>
</style>
