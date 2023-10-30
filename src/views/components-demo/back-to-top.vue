<template>
  <div class="components-container">
    <aside>
      当页面滚动到指定位置时，右下角会出现Back to Top按钮
    </aside>
    <aside>
      您可以自定义按钮的样式，显示/隐藏，外观高度，返回高度。如果你需要
      文本提示，可以在外部使用element-ui el-tooltip元素
    </aside>
    <div class="占位符-container">
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
      <div>占位符</div>
    </div>
    <!-- you can add element-ui's tooltip -->
    <el-tooltip placement="top" content="tooltip">
      <back-to-top :custom-style="myBackToTopStyle" :visibility-height="300" :back-position="50" transition-name="fade" />
    </el-tooltip>
  </div>
</template>

<script>
import BackToTop from '@/components/BackToTop'

export default {
  name: 'BackToTopDemo',
  components: { BackToTop },
  data() {
    return {
      // customizable button style, show/hide critical point, return position
      myBackToTopStyle: {
        right: '50px',
        bottom: '50px',
        width: '40px',
        height: '40px',
        'border-radius': '4px',
        'line-height': '45px', // 请保持与高度一致以垂直居中 Please keep consistent with height to center vertically
        background: '#e7eaf1'// 按钮的背景颜色 The background color of the button
      }
    }
  }
}
</script>

<style scoped>
.占位符-container div {
  margin: 10px;
}
</style>
