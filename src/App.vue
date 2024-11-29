<script setup lang="ts">
import { TypographyTitle } from 'ant-design-vue';
import Example1 from './examples/Example1.vue';
</script>

<template>
  <main class="page-wrapper">
    <TypographyTitle>EJS Examples</TypographyTitle>

    <section>
      <TypographyTitle :level="3">基础用法</TypographyTitle>
      <Example1></Example1>
    </section>

    <section>
      <TypographyTitle :level="3">基础用法</TypographyTitle>
      <Example1></Example1>
    </section>
  </main>
</template>

<style scoped lang="less">
.page-wrapper {
  padding: 20px;
  > section {
    margin-bottom: 20px;
  }
}
</style>
