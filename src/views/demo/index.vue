<template>
  <div class="index-page">
    <div class="index-bd">
      <van-cell title="可拖拽悬浮按钮" is-link to="/example/icons" />
      <van-cell title="滚动导航" is-link to="/example/navbar" />
      <van-cell title="生成海报图" is-link to="/example/poster" />
      <van-cell title="返回浏览位置" is-link to="/keepalive/index" />
    </div>
    <T />
  </div>
  <section>
    <div :class="['btn-add', i18n.global.locale]"></div>
  </section>
</template>

<script setup name="DemoPage">
  import { i18n } from '/@/i18n';
  // import { useI18n } from 'vue-i18n';
  // const { locale } = useI18n();
</script>

<style lang="scss" scoped>
  @import '../../styles/mixin.scss';

  section {
    .title {
      margin-bottom: 40px;
      display: inline-block;
    }

    &:nth-child(2) {
      .title {
        margin-top: 20px;
      }
    }
  }

  .demo {
    > :nth-child(n) {
      margin-right: 20px;
      margin-bottom: 20px;
    }
  }
</style>
