<template>
  <resume-app-bar />

  <div class="resume-layout">
    <resume-profile />

    <resume-blank :size="350"></resume-blank>

    <var-row :gutter="20">
      <var-col :span="12" :xs="24">
        <resume-timeline />
      </var-col>
      <var-col :span="12" :xs="24">
        <resume-skills />
      </var-col>
    </var-row>

    <resume-blank :size="350"></resume-blank>

    <resume-block title="技能清单">
      <resume-block-compact-item description="VUE2/3、React以及相关的生态" />
      <resume-block-compact-item description="Nodejs及相关框架" />
      <resume-block-compact-item description="使用Git进行版本管理" />
      <resume-block-compact-item description="熟练使用TS进行代码开发" />
      <resume-block-compact-item description="了解golang、java、python等后台语言" />
    </resume-block>

    <resume-block title="项目经历" subtitle="**只列举部分典型项目**">
      <resume-block-item
        title="疫情监控系统"
        description="
          <div>背景：2020年疫情爆发，为方便无锡各大学校快速入学、疫情信息上报、统计、分析功能，配合公安、教育局第一时间对异常信息进行处理。</div>
          <div>项目地址：https //yiqing.wxeic.cn </div>
          业绩：
          <ul>
            <li>独立一人完成前端项目的选择、搭建、开发和部署</li>
            <li>参与项目高度复杂的权限设计（包含市、区、街道、校、教师、学生、家长等多身份）</li>
            <li>适应大屏的管理分析后台设计</li>
          </ul>
        "
      />
      <resume-block-item
        title="Reynold"
        description="
          <div>为节省工厂用电成本,保证工厂用电安全,配合光伏建设,提供精准的新能源计算服务。</div>
          <div>项目地址:https://reyold.in2iot.com </div>
          <div>前端技术栈：react+ts+vite+antd+天地图</div>
          <div>责任：前端相关业务开发,封装通用插件并发布到企业内部npm库</div>
        "
      />
      <resume-block-item
        title="农行班牌统计"
        description="
          <div>背景：与农行app合作,为学校提供作业发布、打卡、订餐等功能以及配套后台</div>
          业绩：
            <ul>
              <li>首次在公司内部使用刚刚发布的Vite，并完成相关的功能配置。</li>
              <li>首次完成公司前端由Vue2向React+Ts的迁移</li>
              <li>制定React开发的相关规范。</li>
            </ul>

        "
      />
    </resume-block>

    <resume-block title="开源项目">
      <resume-block-item
        title="Naive UI"
        description="Vue3的一个UI框架，当初还被尤大专门发推了呢，地址在这: https://github.com/tusen-ai/naive-ui"
      />
      <resume-block-item
        title="TDesign UI"
        description="这是腾讯的一个UI库，包含了Vue2/3/React/小程序等，非常喜欢他的文档的清爽，可惜推进太慢。地址在这: https://tdesign.tencent.com/"
      />
      <resume-block-item
          title="Quark UI"
          description="这是一个基于Web Component开发的组件库哦~ 地址在这: https://vue-quarkd.hellobike.com/"
        />
    </resume-block>
  </div>
</template>

<style>
* {
  box-sizing: border-box;
}

@media print {
  * {
    box-shadow: none !important;
  }

  .print-disabled {
    display: none !important;
  }
}

body {
  margin: 0;
  font-family: 'Roboto', sans-serif;
  transition: background-color 0.25s, color 0.25s;
  color: var(--color-text);
  background-color: var(--color-body);
}

::-webkit-scrollbar {
  display: none;
}
</style>

<style lang="less" scoped>
.resume-layout {
  padding: 0 20px 30px;
}
</style>
