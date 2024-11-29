<script setup lang="ts">
import { Textarea } from 'ant-design-vue';
import ejs from 'ejs';

const a = `Hello, <%= text _%>          !`;

const b = ejs.render(a, { text: 'EJS' });
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
      font-size: 12px;
      padding: 16px;
    }
  }
  .output {
    height: 222px;
    flex: 1;
    background-color: #f1f1f1;
    padding: 16px;
    border-radius: 4px;
    font-family: consolas;
    font-size: 12px;
  }
}
</style>
