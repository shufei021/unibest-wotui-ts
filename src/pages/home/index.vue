<script lang="ts" setup>
import { safeAreaInsets } from '@/utils/systemInfo'

defineOptions({
  name: 'Home',
})
definePage({
  // 使用 type: "home" 属性设置首页，其他页面不需要设置，默认为page
  // type: 'home',
  style: {
    // 'custom' 表示开启自定义导航栏，默认 'default'
    navigationBarTitleText: '首页',
  },
})
</script>

<template>
  <view class="bg-white px-4 pt-2" :style="{ marginTop: `${safeAreaInsets?.top}px` }">
    首页
  </view>
</template>
