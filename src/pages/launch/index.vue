<script lang="ts" setup>
import { onMounted } from 'vue'

definePage({
  type: 'home',
  style: {
    navigationStyle: 'custom',
  },
})

onMounted(() => {
  // 2秒后自动跳转到首页
  setTimeout(() => {
    uni.reLaunch({
      url: '/pages/home/index',
    })
  }, 2000)
})
</script>

<template>
  <view class="launch-container">
    <image
      src="/static/images/launch.png"
      mode="scaleToFill"
    />
  </view>
</template>

<style lang="scss" scoped>
.launch-container {
  width: 100vw;
  height: 100vh;
  image {
    width: 100%;
    height: 100%;
  }
}
</style>
