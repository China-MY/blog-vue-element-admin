<template>
  <aside>
    创建和编辑页面不能由keep-alive缓存，因为keep-alive include目前不支持
    基于路由缓存，所以目前是基于组件名称缓存。如果你想实现类似的缓存
    效果，你可以使用浏览器缓存方案，如localStorage。或者不使用keep-alive include来缓存所有
    页直接。看到细节
    <a
      href="https://panjiachen.github.io/vue-element-admin-site/guide/essentials/tags-view.html"
      target="_blank"
    >文档</a>
  </aside>
</template>

