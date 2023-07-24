<script setup lang="ts">
import { ref } from 'vue'

const companies = ref([
  {
    label: 'Softtek',
    date: '2022/04-至今',
    description: [
    `负责产品功能的前端架构设计和优化，以及日常开发。`,
      `1. 根据项目需求选择并配置前端的框架。封装通用组件`,
      `2. 根据设计稿完成页面开发`,
      `3. 带领团队攻克项目中的难点、帮助同事解决问题`
    ],
  },
  {
    label: '因方科技(无锡)有限公司',
    date: '2021/09-2022/03',
    description: [
      '1、负责前端框架、相关工具包的调研和选择',
      '2、npm包开发并发布公司组件库 ',
      '3、参与项目CR',
    ],
  },
  {
    label: '江苏中育优教科技发展有限公司',
    date: '2019/03-2021/08',
    description: [
      '1. 新项目的需求分析、框架选择、任务安排',
      '2. 项目中的难点攻克',
      '3. 公司框架从vue2转向React + Ts，全面拥抱Ts',
      '4. 开发相关技术探索',
    ],
  },
])
</script>

<template>
  <resume-block title="工作经历">
    <var-steps
      class="resume-timeline"
      direction="vertical"
      :active="companies.length - 1"
    >
      <var-step
        current-icon="map-marker"
        active-icon="map-marker"
        v-for="c in companies"
        :key="c.label"
      >
        <div class="resume-timeline-company">
          <div class="resume-timeline-label">{{ c.label }}</div>
          <div class="resume-timeline-date">{{ c.date }}</div>
          <div 
            class="resume-timeline-description" 
            v-for=" d  in  c.description "
            :key="d"
          >{{ d }}</div>
        </div>
      </var-step>
    </var-steps>
  </resume-block>
</template>

<style lang="less" scoped>
.resume-timeline {
  &-company {
    margin-left: 10px;
  }

  &-label {
    font-size: 16px;
  }

  &-date {
    color: #aaa;
    margin: 6px 0;
  }

  &-description {
    color: #555;
  }
}
</style>
