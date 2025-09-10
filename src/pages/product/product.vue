<script lang="ts" setup>
definePage({
  style: {
    navigationBarTitleText: '商品',
  },
})
onReady(() => {
  console.log('onReady uniKuRoot exposeRef')
})
onShow(() => {
  console.log('onShow uniKuRoot exposeRef')
})
</script>

<template root="uniKuRoot">
  <view>
    商品
  </view>
</template>
