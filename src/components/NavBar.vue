<template>
  <!-- 顶部导航栏 -->
  <div class="navbar">
    <div class="navbar-inner">
      <!-- 左边导航菜单 -->
      <div class="left-bar">
        <p>小米官网</p>
        <p class="line">|</p>
        <p>小米商城</p>
        <p class="line">|</p>
        <p>小米澎湃OS</p>
        <p class="line">|</p>
        <p>小米汽车</p>
        <p class="line">|</p>
        <p>云服务</p>
        <p class="line">|</p>
        <p>IoT</p>
        <p class="line">|</p>
        <p>有品</p>
        <p class="line">|</p>
        <p>小爱开放平台</p>
        <p class="line">|</p>
        <p>资质证照</p>
        <p class="line">|</p>
        <p>协议规则</p>
        <p class="line">|</p>
        <p>下载app</p>
        <p class="line">|</p>
        <p>Select Location</p>
      </div>

      <!-- 右边功能菜单 -->
      <div class="right-bar">
        <p>登录</p>
        <p class="line">|</p>
        <p>注册</p>
        <p class="line">|</p>
        <p>消息通知</p>

        <!-- 购物车图标和文字 -->
        <div class="shopping-cart">
          <svg t="1751941930629" class="shopping-icon" viewBox="0 0 1024 1024" version="1.1"
               xmlns="http://www.w3.org/2000/svg" p-id="14011" width="200" height="200">
            <path d="M208.0512 76.8a25.6 25.6 0 0 1 25.3696 22.1184l18.3552 134.272h664.6528a25.6 25.6 0 0 1 25.1648 30.2848l-80.128 432.384a25.6 25.6 0 0 1-25.1648 20.9408H263.1936a25.6 25.6 0 0 1-25.3952-22.3744l-6.656-52.3776H230.4L168.5248 153.6H51.2V76.8h156.8512z m646.8096 233.216h-588.288L308.3008 640h485.376l61.184-329.984zM307.2 742.4a102.4 102.4 0 1 1 0 204.8 102.4 102.4 0 0 1 0-204.8z m0 66.56a35.84 35.84 0 1 0 0 71.68 35.84 35.84 0 0 0 0-71.68zM793.6 742.4a102.4 102.4 0 1 1 0 204.8 102.4 102.4 0 0 1 0-204.8z m0 66.56a35.84 35.84 0 1 0 0 71.68 35.84 35.84 0 0 0 0-71.68z"
                  p-id="14012" fill="currentColor"></path>
          </svg>
          <p>购物车</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
// 当前不需要 JS 逻辑
</script>

<style scoped>
/* 外层导航栏，撑满宽度 */
.navbar {
  width: 100%;
  height: 40px;
  background-color: #333;
  display: flex;
  justify-content: center;
}

/* 中间最大 1226px 居中容器 */
.navbar-inner {
  width: 1226px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

/* 左边菜单 */
.left-bar {
  display: flex;
  align-items: center;
  gap: 8px;
}

/* 右边菜单 */
.right-bar {
  display: flex;
  align-items: center;
  gap: 8px;
}

/* 通用文字样式 */
.navbar p {
  margin: 0;
  font-size: 12px;
  color: rgb(176, 176, 176);
  line-height: 40px;
  cursor: pointer;
}

.navbar p:hover {
  color: white;
}

.line {
  opacity: 0.2;
}

/* 购物车整体样式 */
.shopping-cart {
  height: 40px;
  background-color: rgb(66, 66, 66);
  color: rgb(176, 176, 176);
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 4px;
  padding: 0 10px;
  cursor: pointer;
  transition: background-color 0.2s;
}

/* 鼠标悬停效果 */
.shopping-cart:hover {
  background-color: white;
  color: rgb(255, 103, 0);
}

.shopping-cart:hover p {
  color: rgb(255, 103, 0);
}

/* SVG 图标尺寸 */
.shopping-icon {
  width: 20px;
}
</style>
