<script setup lang="ts">
import { TypographyTitle } from 'ant-design-vue';
import Example1 from './examples/Example1.vue';
import Example2 from './examples/Example2.vue';
</script>

<template>
  <main class="page-wrapper">
    <TypographyTitle>EJS Examples</TypographyTitle>

    <section>
      <TypographyTitle :level="3">bind</TypographyTitle>
      <Example1></Example1>
    </section>

    <section>
      <TypographyTitle :level="3">if</TypographyTitle>
      <Example2></Example2>
    </section>
  </main>
</template>

<style scoped lang="less">
.page-wrapper {
  padding: 20px;
  > section {
    margin-bottom: 100px;
  }
}
</style>
