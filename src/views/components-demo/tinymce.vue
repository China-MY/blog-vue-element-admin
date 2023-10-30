<template>
  <div class="components-container">
    <aside>
      富文本是管理后台的一个核心特性，但同时也是一个“坑”多的地方。在选择丰富文本的过程中，我也走了很多弯路。市面上常见的富文本已经基本使用，最后选择了tinyce。详见更详细的富文本比较和介绍。      <a target="_blank" class="link-type" href="https://panjiachen.github.io/vue-element-admin-site/feature/component/rich-editor.html">Documentation</a>
    </aside>
    <div>
      <tinymce v-model="content" :height="300" />
    </div>
    <div class="editor-content" v-html="content" />
  </div>
</template>

<script>
import Tinymce from '@/components/Tinymce'

export default {
  name: 'TinymceDemo',
  components: { Tinymce },
  data() {
    return {
      content:
      `<h1 style="text-align: center;">Welcome to the TinyMCE demo!</h1><p style="text-align: center; font-size: 15px;"><img title="TinyMCE Logo" src="//www.tinymce.com/images/glyph-tinymce@2x.png" alt="TinyMCE Logo" width="110" height="97" /><ul>
        <li>Our <a href="//www.tinymce.com/docs/">documentation</a> is a great resource for learning how to configure TinyMCE.</li><li>Have a specific question? Visit the <a href="https://community.tinymce.com/forum/">Community Forum</a>.</li><li>We also offer enterprise grade support as part of <a href="https://tinymce.com/pricing">TinyMCE premium subscriptions</a>.</li>
      </ul>`
    }
  }
}
</script>

<style scoped>
.editor-content{
  margin-top: 20px;
}
</style>

