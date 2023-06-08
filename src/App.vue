<template>
  <n-space>
    <n-input-group>
      <n-input :style="{ width: '100%' }" />
      <n-button type="primary" ghost>
          搜索
      </n-button>
    </n-input-group>
  </n-space>
  <n-space>
    <DataTables/>
  </n-space>
</template>

<script>
import { NCard, NSpace, NInputGroup, NInput, NButton } from 'naive-ui';
import ButtonCounter from './components/ButtonCounter.vue';
import DataTables from './components/DataTables.vue';

export default {
  components: {
    ButtonCounter, DataTables, NCard, NSpace, NInputGroup, NInput, NButton
    }
};
</script>