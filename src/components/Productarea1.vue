<template>
  <div class="overall">
    <div class="top-area">
      <p style="font-size: 22px; font-weight: 250; color: #333;">手机</p>
      <div class="top-right-area">
        <p class="top-right-p">查看更多</p>
        <svg t="1752477035632" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="16433" width="200" height="200"><path d="M0 512c0 283.733333 228.266667 512 512 512s512-228.266667 512-512S795.733333 0 512 0 0 228.266667 0 512zM405.333333 206.933333l275.2 275.2c8.533333 8.533333 12.8 19.2 10.666667 29.866667 0 10.666667-4.266667 21.333333-10.666667 29.866667L405.333333 817.066667c-14.933333 14.933333-40.533333 14.933333-55.466666 0l-4.266667-4.266667c-14.933333-14.933333-14.933333-40.533333 0-55.466667L588.8 512 343.466667 266.666667c-14.933333-14.933333-14.933333-40.533333 0-55.466667l4.266666-4.266667c14.933333-14.933333 40.533333-14.933333 57.6 0z" p-id="16434" fill="currentColor"></path></svg>
      </div>
    </div>

    <div class="bottom-area">
      <div class="bottom-left">
          <img class="main-img" src="/public/Productarea1/product.webp">
      </div>

      <div class="bottom-right">
        <div class="product">
          <img class="img" src="/public/Productarea1/product1.webp">
          <div class="p1">Xiaomi MIX Flip 2</div>
          <div class="p2">4.01英寸多功能超大外屏</div>
          <div class="p3">5999元起</div>
        </div>
        <div class="product">
          <img class="img" src="/public/Productarea1/product2.webp">
          <div class="p1">REDMI K80至尊版</div>
          <div class="p2">天玑9400+|7410mAh超长续航|大师..</div>
          <div class="p3">2599元起</div>
        </div>
        <div class="product">
          <img class="img" src="/public/Productarea1/product3.webp">
          <div class="p1">Xiaomi 15S Pro</div>
          <div class="p2">小米15周年特别设计</div>
          <div class="p3">5499元起</div>
        </div>
        <div class="product">
          <img class="img" src="/public/Productarea1/product4.webp">
          <div class="p1">Xiaomi Civi 5 Pro</div>
          <div class="p2">徕卡光学Summilux高速镜头|600...</div>
          <div class="p3">2999元起</div>
        </div>
        <div class="product">
          <img class="img" src="/public/Productarea1/product5.webp">
          <div class="p1">REDMI Turbo 4 Pro</div>
          <div class="p2">Turbo 4 Pro 好看，更能打！</div>
          <div class="p3">1899元起</div>
        </div>
        <div class="product">
          <img class="img" src="/public/Productarea1/product6.webp">
          <div class="p1">Xiaomi 15 Ultra</div>
          <div class="p2">暗夜之眼 徕卡光学</div>
          <div class="p3">6499元起</div>
        </div>
        <div class="product">
          <img class="img" src="/public/Productarea1/product7.webp">
          <div class="p1">REDMI Turbo 4</div>
          <div class="p2">REDMI Turbo 4好看又能打</div>
          <div class="p3">1699元起</div>
        </div>
        <div class="product">
          <img class="img" src="/public/Productarea1/product8.webp">
          <div class="p1">Redmi 14C</div>
          <div class="p2">【持久续航】5160mAh大电池</div>
          <div class="p3">469元起</div>
        </div>
      </div>
    
    </div>
  </div>
</template>

<script setup>
</script>

<style scoped>
.main-img {
  transition: all 0.3s;
}

/* 悬浮生效 */
.main-img:hover,
.product:hover{
  transform: translateY(-3px); /* 向上移动 */
  box-shadow: 0 12px 20px rgba(0, 0, 0, 0.1); /* 更明显的下阴影 */
}


.img {
  width: 160px;
  height: 160px;
}

.icon {
  width: 20px;
  height: 20px;
  /* vertical-align: middle; */
}

.overall {
  display: flex;
  /* column情况下align决定水平排列位置，justify决定竖直排列位置 */
  flex-direction: column;
  align-items: center;
  justify-content: end;
  width: 100%;
  height: 695px;
  background-color: #f5f5f5;
}

.top-area {
  display: flex;
  width: 1226px;
  height: 58px;
  align-items: center;
  justify-content: space-between;
}

.top-right-area {
  color: #b0b0b0;
  display: flex;
  align-items: center;
  gap: 6px;
  cursor: pointer;
  transition: color 0.3s;
}

.top-right-p {
  color: #424242; /* 默认文字色 */
  transition: color 0.3s;
}

.top-right-area:hover {
  color: #ff6700;
}

.top-right-area:hover p {
  color: #ff6700;
}

.bottom-area {
  display: grid;
  gap: 14px;
  grid-template-columns: 234px 1fr;
  width: 1226px;
  height: 614px;
}

.bottom-right {
  display: grid;
  gap: 14px;
  grid-template-columns: 1fr 1fr 1fr 1fr;
}

.product {
  /* 上下 左右 */
  padding: 20px 0px;
  background-color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 234px;
  height: 300px;
  /* 让padding不会撑开变大 */
  box-sizing: border-box;
  transition: all 0.3s ease;
}

.p1 {
color: #333333;
font-size: 14px;
/* 上 左右 下 */
margin: 0px 10px 2px;
}

.p2 {
color: #b0b0b0;
font-size: 13px;
margin: 0px 10px 10px;
}

.p3 {
color: #ff6700;
font-size: 16px;
margin: 0px 10px 14px;
}
</style>