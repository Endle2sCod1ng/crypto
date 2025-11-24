<script lang="ts">
import Header from '@/widgets/Header.vue';
export default {
  data() {
    return {
      now: new Date().toLocaleDateString(),
      news: ["New 1", "New 2", "New 3"],
    };
  }
};
</script>


<template>
  <div class=" w-full">
    <div class="mx-auto my-0 container xl">
      <Header />

      <div class="w-full h-40 bg-blue-900 rounded-3xl my-5">
        <h2>Actual news {{ now }}</h2>
      </div>
      <div
        class="w-full h-40 bg-blue-900 rounded-3xl my-5"
        v-for="item in news"
        :key="item"
      >
        <h3>{{ item }}</h3>
      </div>
    </div>

    <main>
      <h1>Hello Vue 3</h1>
    </main>
    <!-- 4:33 Create c -->
  </div>


</template>


<style scoped></style>
