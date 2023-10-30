<template>
  <div class="errPage-container">
    <ErrorA />
    <ErrorB />
    <h3>请点击右上角的bug图标</h3>
    <aside>
      现在的管理系统基本上都是spa的形式，它增强了用户体验，但也增加了页面出现问题的可能性，稍有疏忽就可能导致整个页面死锁。幸运的是，Vue提供了一种捕获异常处理的方法，您可以在其中处理错误或报告异常。 <a
        target="_blank"
        class="link-type"
        href="https://panjiachen.github.io/vue-element-admin-site/guide/advanced/error.html"
      >
        文档简介
      </a>
    </aside>
    <a href="#">
      <img src="https://wpimg.wallstcn.com/360e4842-4db5-42d0-b078-f9a84a825546.gif">
    </a>
  </div>
</template>

<script>
import ErrorA from './components/ErrorTestA'
import ErrorB from './components/ErrorTestB'

export default {
  name: 'ErrorLog',
  components: { ErrorA, ErrorB }
}
</script>

<style scoped>
.errPage-container {
  padding: 30px;
}
</style>
