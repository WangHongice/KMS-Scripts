<script setup lang="ts">
import { System, Application, Windows, Word } from '@icon-park/vue-next'
</script>

<template>
  <a-layout>
    <a-layout-sider>
      <a-menu :style="{ height: '100%' }" :default-open-keys="['0', '1']" :default-selected-keys="['0_0']">
        <a-sub-menu key="0">
          <template #icon><System /></template>
          <template #title>系统</template>
          <a-menu-item key="0_0">
            <template #icon><Windows /></template>
            Windows
          </a-menu-item>
        </a-sub-menu>
        <a-sub-menu key="1">
          <template #icon><Application /></template>
          <template #title>软件</template>
          <a-menu-item key="1_0">
            <template #icon><Word /></template>
            Office
          </a-menu-item>
        </a-sub-menu>
      </a-menu>
    </a-layout-sider>
    <a-layout-content class="ml-4">Content</a-layout-content>
  </a-layout>
</template>
