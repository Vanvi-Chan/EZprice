<template>
  <!-- <a-space direction="vertical" :style="{ width: '100%' }" :size="[0, 48]"> -->
  <!-- <a-space> -->
  <a-layout>
    <a-layout-header :style="headerStyle">Header</a-layout-header>
    <a-layout has-sider>
      <a-layout-sider :style="siderStyle">Sider</a-layout-sider>
      <a-layout-content :style="contentStyle">Content</a-layout-content>
    </a-layout>
    <a-layout-footer :style="footerStyle">Footer</a-layout-footer>
  </a-layout>
  <!-- </a-space> -->
  <!-- </a-space> -->

</template>

<script setup lang='ts'>
import { ref, reactive } from 'vue';
import type { CSSProperties } from 'vue';
const headerStyle: CSSProperties = {
  textAlign: 'center',
  color: '#fff',
  height: '10vh',
  // width: '100%',
  paddingInline: 50,
  lineHeight: '10vh',
  backgroundColor: '#7dbcea',
};

const contentStyle: CSSProperties = {
  textAlign: 'center',
  minHeight: 120,
  lineHeight: '80vh',
  color: '#fff',
  backgroundColor: '#108ee9',
};

const siderStyle: CSSProperties = {
  textAlign: 'center',
  lineHeight: '80vh',
  color: '#fff',
  backgroundColor: '#3ba0e9',
};

const footerStyle: CSSProperties = {
  height: '10vh',
  lineHeight: '10vh',
  textAlign: 'center',
  color: '#fff',
  backgroundColor: '#7dbcea',
};
</script>

<style scoped>
.layout {
  width: 100%;
  height: 100%;
}
</style>