<script setup lang="ts">
import { TypographyTitle } from 'ant-design-vue';
import Example1 from './examples/Example1.vue';
import Example2 from './examples/Example2.vue';
import Example3 from './examples/Example3.vue';
import Example4 from './examples/Example4.vue';
import Example5 from './examples/Example5.vue';
import Example6 from './examples/Example6.vue';
import Example7 from './examples/Example7.vue';
import Example8 from './examples/Example8.vue';
</script>

<template>
  <main class="page-wrapper">
    <TypographyTitle>EJS Examples</TypographyTitle>

    <section>
      <TypographyTitle :level="3"><%= ... %></TypographyTitle>
      <Example3></Example3>
    </section>

    <section>
      <TypographyTitle :level="3"><%- ... %></TypographyTitle>
      <Example4></Example4>
    </section>

    <section>
      <TypographyTitle :level="3"><% ... %></TypographyTitle>
      <Example1></Example1>
    </section>

    <section>
      <TypographyTitle :level="3"><%_ ... %></TypographyTitle>
      <Example2></Example2>
    </section>

    <section>
      <TypographyTitle :level="3"><% ... _%></TypographyTitle>
      <Example8></Example8>
    </section>

    <section>
      <TypographyTitle :level="3"><%# ... %></TypographyTitle>
      <Example5></Example5>
    </section>

    <section>
      <TypographyTitle :level="3"><%% ... %%></TypographyTitle>
      <Example6></Example6>
    </section>

    <section>
      <TypographyTitle :level="3"><% ... -%></TypographyTitle>
      <Example7></Example7>
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
