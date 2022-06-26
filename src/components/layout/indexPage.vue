<template>
  <a-layout>
    <a-layout-header class="header" style="position: relative; background: #434343">
      <div class="logo" />
      <a-typography-title :level="2" style="color: #fff; float: left; margin: 10px 0px"
        >程序员导航</a-typography-title
      >
      <span
        style="
          font-size: 22px;
          color: #fff;
          float: right;
          position: absolute;
          margin: auto 10px;
          right: 30px;
        "
        >{{ nowTime }}</span
      >
    </a-layout-header>
    <a-layout has-sider>
      <a-layout-sider
        v-model:collapsed="collapsed"
        collapsible
        width="150px"
        style="border-radius: 20px; background: #f0f2f5; margin: 30px 50px; padding: 10px 0px"
        :style="{ overflow: 'auto', position: 'fixed' }"
      >
        <a-menu
          v-model:selectedKeys="selectedKeys2"
          v-model:openKeys="openKeys"
          mode="inline"
          style="height: 100%; background: #f0f2f5"
        >
          <div ref="containerRef">
            <a-affix :target="() => containerRef">
              <a-anchor :affix="false">
                <a-menu-item key="1">
                  <a-anchor-link href="#d1" title="常用工具" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="2">
                  <a-anchor-link href="#d2" title="技术社区" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="3">
                  <a-anchor-link href="#d3" title="限时专区" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="4">
                  <a-anchor-link href="#d4" title="摸鱼专区" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="5">
                  <a-anchor-link href="#d5" title="学习平台" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="6">
                  <a-anchor-link href="#d6" title="协同工作" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="7">
                  <a-anchor-link href="#d7" title="头部社区" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="8">
                  <a-anchor-link href="#d8" title="资源推荐" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="9">
                  <a-anchor-link href="#d9" title="图片专区" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="10">
                  <a-anchor-link href="#d10" title="视频专区" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="11">
                  <a-anchor-link href="#d11" title="站长工具" style="font-size: 1rem" />
                </a-menu-item>
                <a-menu-item key="12">
                  <a-anchor-link href="#d12" title="其他工具" style="font-size: 1rem" />
                </a-menu-item>
              </a-anchor>
            </a-affix>
          </div>
        </a-menu>
      </a-layout-sider>
    </a-layout>

    <a-layout-content style="margin: 0px 30px 0px 200px; padding: 0 50px">
      <a-layout
        style="
          border-radius: 20px;
          padding: 24px 0;
          margin: 30px 10px;
          background: #fff;
          overflow: initial;
        "
      >
        <a-layout-content :style="{ padding: '0 24px', minHeight: '280px' }">
          <div id="d1">
            <UsefulTools />
          </div>
          <div id="d2" style="margin-top: 30px">
            <JishuPage />
          </div>
          <div id="d3" style="margin-top: 30px">
            <XianshiPage />
          </div>
          <div id="d4" style="margin-top: 30px">
            <MoyuPage />
          </div>
        </a-layout-content>
      </a-layout>
    </a-layout-content>
    <a-layout-footer style="text-align: center">
      Ant Design ©2018 Created by Alexander
    </a-layout-footer>
  </a-layout>
  <div id="components-back-top-demo-custom">
    <a-back-top>
      <div class="ant-back-top-inner"><rocket-outlined :style="{ fontSize: '40px' }" /></div>
      TOP
    </a-back-top>
  </div>
</template>
<script>
  import { defineComponent, onMounted, ref } from 'vue';
  import { formateDate } from '@/components/date/nowDate';
  import { RocketOutlined } from '@ant-design/icons-vue';
  import UsefulTools from '@/components/content/usefulTools.vue';
  import JishuPage from '@/components/content/jishuPage.vue';
  import XianshiPage from '@/components/content/xianshiPage.vue';
  import MoyuPage from '@/components/content/moyuPage.vue';

  export default defineComponent({
    components: {
      RocketOutlined,
      UsefulTools,
      JishuPage,
      XianshiPage,
      MoyuPage,
    },

    setup() {
      const containerRef = ref();
      const nowTime = ref('');

      onMounted(() => {
        setInterval(() => {
          nowTime.value = formateDate(new Date());
        });
      });

      return {
        containerRef,
        selectedKeys1: ref(['2']),
        selectedKeys2: ref(['1']),
        openKeys: ref(['sub1']),
        collapsed: ref(false),
        nowTime,
      };
    },
  });
</script>
<style>
  #components-layout-demo-top-side .logo {
    float: left;
    width: 120px;
    height: 31px;
    margin: 16px 24px 16px 0;
    background: rgba(255, 255, 255, 0.3);
  }

  .ant-row-rtl #components-layout-demo-top-side .logo {
    float: right;
    margin: 16px 0 16px 24px;
  }

  .site-layout-background {
    background: #f0f2f5;
  }

  #components-back-top-demo-custom .ant-back-top {
    right: 25px;
    top: 85%;
    position: fixed;
  }

  #components-back-top-demo-custom .ant-back-top:hover {
    background: #fa8c16;
    border-radius: 100%;
    width: 40px;
    height: 40px;
  }

  .ant-anchor-link {
    margin: 10px 0px;
  }

  .ant-anchor-link:hover {
    background: #fa8c16;
    border-radius: 5px;
    width: 100px;
  }

  .ant-anchor-link-active {
    font-weight: 600;
    border-bottom: 3px solid RGB(0, 179, 167);
  }

  ::-webkit-scrollbar {
    display: none;
  }
</style>
