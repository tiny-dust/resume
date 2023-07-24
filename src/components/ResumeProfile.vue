<template>
  <div class="resume-profile">
    <var-row :gutter="20">
      <var-col justify="center" :span="12" :xs="24">
        <var-paper class="resume-profile-paper" :elevation="2" :radius="4">
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-cake class="resume-profile-icon" />
              <span>出生日期: 93-12-24</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-school class="resume-profile-icon" />
              <span>学校: 无锡科技职业学院</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-calendar class="resume-profile-icon" />
              <span>工作年限: 5年</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-account-group class="resume-profile-icon" />
              <span>期望岗位: 前端开发工程师</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-cash class="resume-profile-icon" />
              <span>期望薪资: 18k</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0">
            <div class="resume-profile-cell">
              <icon-city class="resume-profile-icon" />
              <span>期望城市: 无锡</span>
            </div>
          </var-cell>
        </var-paper>
      </var-col>

      <var-col :span="12" :xs="24">
        <var-paper class="resume-profile-paper" :elevation="2" :radius="4">
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-phone class="resume-profile-icon" />
              <span>手机: 17625022511</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-email class="resume-profile-icon" />
              <span>邮箱: idioticzhou@outlook.com</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-tencent class="resume-profile-icon" />
              <span>QQ: 1710940645</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-wechat class="resume-profile-icon" />
              <span>微信: Tiny_dust_z</span>
            </div>
          </var-cell>
          <var-cell :border-offset="0" border>
            <div class="resume-profile-cell">
              <icon-post class="resume-profile-icon" />
              <span>掘金: 
                <a href="https://juejin.cn/user/3491704662659464">tiny_dust</a>
              </span>
            </div>
          </var-cell>
          <var-cell :border-offset="0">
            <div class="resume-profile-cell">
              <icon-github class="resume-profile-icon" />
              <span>Github: <a href="https://github.com/tiny-dust">tiny-dust</a></span>
            </div>
          </var-cell>
        </var-paper>
      </var-col>
    </var-row>
  </div>
</template>

<style lang="less" scoped>
.resume-profile {
  width: 100%;

  &-paper {
    width: 100%;
    margin-top: 30px;
  }

  &-cell {
    display: flex;
    align-items: center;
  }

  &-icon {
    width: 22px;
    margin-right: 10px;
    fill: var(--color-primary)
  }
}
</style>
