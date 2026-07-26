<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****6611 完成了人工智能商业计划书 12 Page PPT 大纲生成"
  },
  {
    "text": "用户 189****9012 生成了季度销售业绩汇报对比图表设计建议"
  },
  {
    "text": "用户 131****4455 完成了医疗科技发布会沉浸式开场白与配色方案"
  },
  {
    "text": "用户 156****7710 生成了毕业答辩 PPT 逻辑框架与数据图表布局"
  },
  {
    "text": "用户 177****3389 取得了高管年度战略复盘 Page-by-Page 指南"
  }
]);
</script>
