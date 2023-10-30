<template>
  <div class="app-container">
    <aside>
      指南页面对于第一次进入这个项目的人很有用。你可以简单介绍一下
      项目的特点。演示基于
      <a href="https://github.com/kamranahmedse/driver.js" target="_blank">driver.js</a>
    </aside>
    <el-button icon="el-icon-question" type="primary" @click.prevent.stop="guide">
      节目指南
    </el-button>
  </div>
</template>

<script>
import Driver from 'driver.js' // import driver.js
import 'driver.js/dist/driver.min.css' // import driver.js css
import steps from './steps'

export default {
  name: 'Guide',
  data() {
    return {
      driver: null
    }
  },
  mounted() {
    this.driver = new Driver()
  },
  methods: {
    guide() {
      this.driver.defineSteps(steps)
      this.driver.start()
    }
  }
}
</script>
