<template>
  <div class="components-container">
    <aside>
      基于<a class="link-type" href="https://github.com/rowanwins/vue-dropzone"> dropzone </a>.
      因为我的业务有特殊需求，需要上传图片给qiniu，所以我没有选择第三方，而是选择了自己封装。这很简单，你可以在@/components/Dropzone中看到详细的代码。    </aside>
    <div class="editor-container">
      <dropzone id="myVueDropzone" url="https://httpbin.org/post" @dropzone-removedFile="dropzoneR" @dropzone-success="dropzoneS" />
    </div>
  </div>
</template>

<script>
import Dropzone from '@/components/Dropzone'

export default {
  name: 'DropzoneDemo',
  components: { Dropzone },
  methods: {
    dropzoneS(file) {
      console.log(file)
      this.$message({ message: 'Upload success', type: 'success' })
    },
    dropzoneR(file) {
      console.log(file)
      this.$message({ message: 'Delete success', type: 'success' })
    }
  }
}
</script>

