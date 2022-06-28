<template>
  <div class="tools-name">摸鱼专区</div>
  <hr color="#f0f0f0" />
  <a-row type="flex" :gutter="{ xs: 8, sm: 16, md: 24, lg: 32 }">
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="1">
      <a class="tools-hover" href="http://buhuixiao.com" target="blank">
        <div class="icon"
          ><img class="tools-img" src="https://cxy521.com/static/img/index/relax/laughyouth.png"
        /></div>
        <div class="content">
          <span class="title">程序员漫画</span>
          <p class="description">全网唯二的程序员漫画故事</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="2">
      <a class="tools-hover" href="https://tophub.today/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="https://file.ipadown.com/tophub/assets/images/logo.png"
        /></div>
        <div class="content">
          <span class="title">今日热榜</span>
          <p class="description">今日热榜提供各站热榜聚合</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="3">
      <a class="tools-hover" href="https://www.zhihu.com/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="https://static.zhihu.com/heifetz/favicon.ico"
        /></div>
        <div class="content">
          <span class="title">知乎</span>
          <p class="description">中国最大的问答社区</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="4">
      <a class="tools-hover" href="https://mo.fish" target="blank">
        <div class="icon"
          ><img class="tools-img" src="https://cxy521.com/static/img/index/relax/fish.ico"
        /></div>
        <div class="content">
          <span class="title">鱼塘热榜</span>
          <p class="description">聚合每日热门、搞笑、有趣资讯</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="5">
      <a class="tools-hover" href="https://www.qiushibaike.com/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="https://cxy521.com/static/img/index/relax/baike.jpg"
        /></div>
        <div class="content">
          <span class="title">糗事百科</span>
          <p class="description">超搞笑的原创糗事笑话分享社区</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="6">
      <a class="tools-hover" href="http://www.itmind.net/xbw/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="https://cxy521.com/static/img/index/relax/yx.png"
        /></div>
        <div class="content">
          <span class="title">怀旧游戏合集</span>
          <p class="description">小霸王 超级玛丽 魂斗罗 雪人兄弟</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="7">
      <a class="tools-hover" href="https://fishpi.cn/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="https://fishpi.cn/images/favicon.png"
        /></div>
        <div class="content">
          <span class="title">摸鱼派</span>
          <p class="description">以程序员、设计师和极客为核心的社区</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="8">
      <a class="tools-hover" href="https://p.hancel.org/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="https://p.hancel.org/images/mofish.jpg"
        /></div>
        <div class="content">
          <span class="title">摸鱼大闯关</span>
          <p class="description">一个非常烧脑的CTF类闯关游戏</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="9">
      <a class="tools-hover" href="http://adarkroom.doublespeakgames.com/?lang=zh_cn" target="blank">
        <div class="icon"
          ><img class="tools-img" src="http://www.cxy521.com/static/img/index/relax/adr.png"
        /></div>
        <div class="content">
          <span class="title">暗室</span>
          <p class="description">适用于浏览器的极简文字冒险游戏</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="10">
      <a class="tools-hover" href="http://www.chinaunix.net/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="http://cxysite.com/static/img/ltzx/cu.png"
        /></div>
        <div class="content">
          <span class="title">空间站对接</span>
          <p class="description">SpaceX出品的空间站对接模拟器</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="11">
      <a class="tools-hover" href="http://www.itmind.net/tetris/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="http://www.cxy521.com/static/img/index/relax/tetris.jpg"
        /></div>
        <div class="content">
          <span class="title">俄罗斯方块</span>
          <p class="description">经典俄罗斯方块网页版</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="12">
      <a class="tools-hover" href="https://dig.chouti.com/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="http://www.cxy521.com/static/img/index/relax/chouti.png"
        /></div>
        <div class="content">
          <span class="title">抽屉新热榜</span>
          <p class="description">聚合每日热门、搞笑、有趣资讯</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="13">
      <a class="tools-hover" href="https://www.webhek.com/post/draw-a-stickman.html" target="blank">
        <div class="icon"
          ><img class="tools-img" src="http://www.cxy521.com/static/img/index/relax/fwebhek.ico"
        /></div>
        <div class="content">
          <span class="title">神笔马良</span>
          <p class="description">小人历险记-创作型游戏</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="14">
      <a class="tools-hover" href="https://findtheinvisiblecow.com" target="blank">
        <div class="icon"
          ><img class="tools-img" src="http://www.cxy521.com/static/img/index/relax/findtheinvisiblecow.png"
        /></div>
        <div class="content">
          <span class="title">找到那个牛</span>
          <p class="description">一个根据声音找动物的小游戏</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="15">
      <a class="tools-hover" href="https://2020game.io/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="http://www.cxy521.com/static/img/index/relax/2020.png"
        /></div>
        <div class="content">
          <span class="title">2020游戏</span>
          <p class="description">重点推荐，闯关类游戏！</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="16">
      <a class="tools-hover" href="https://mp.weixin.qq.com/s/LWagJEHnitxkYtXeCy3zRg" target="blank">
        <div class="icon"
          ><img class="tools-img" src="http://www.cxy521.com/static/img/index/relax/hongbao.png"
        /></div>
        <div class="content">
          <span class="title">外卖红包</span>
          <p class="description">每天点外卖，免费领红包！</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="17">
      <a class="tools-hover" href="https://strobe.cool/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="http://www.cxy521.com/static/img/index/relax/strobe.ico"
        /></div>
        <div class="content">
          <span class="title">扭曲世界</span>
          <p class="description">你周围的世界会改变形状，显得扭曲和变形</p>
        </div>
      </a>
    </a-col>
    <a-col :xs="12" :sm="8" :md="6" :lg="4" :order="18">
      <a class="tools-hover" href="https://bouncyballs.org/" target="blank">
        <div class="icon"
          ><img class="tools-img" src="http://www.cxy521.com/static/img/index/relax/bouncyballs.ico"
        /></div>
        <div class="content">
          <span class="title">弹力球</span>
          <p class="description">用鼠标去玩弹力球，解压</p>
        </div>
      </a>
    </a-col>
  </a-row>
</template>
<script>
  export default {};
</script>
<style></style>
