<script setup lang="ts">
import { Textarea } from 'ant-design-vue';
import ejs from 'ejs';

const a = `Hello, <%= name %>!`;

const b = ejs.render(a, { name: 'EJS' });
</script>

<template>
  <div class="example-wrapper">
    <div class="input">
      <Textarea
        v-model:value="a"
        :rows="10"
        placeholder="type template"
      ></Textarea>
    </div>
    <div class="output">
      <pre>{{ b }}</pre>
    </div>
  </div>
</template>

<style scoped lang="less">
.example-wrapper {
  display: flex;
  gap: 20px;
  align-items: center;
  .input {
    width: 450px;
    textarea {
      resize: none;
      font-family: consolas;
      padding: 16px;
    }
  }
  .output {
    height: 253px;
    flex: 1;
    background-color: #f1f1f1;
    padding: 16px;
    border-radius: 4px;
    font-family: consolas;
  }
}
</style>
