<!--
 * @Author: qianqian.zhao
 * @Date: 2020-03-25 18:50:33
 * @LastEditors: qianqian.zhao
 * @LastEditTime: 2020-04-04 17:27:12
 * @Description: 单页面首页组件
 -->

<template>
  <div class="miao">
    <!-- 这是项目的根目录文件app -->
    <!-- 路由匹配的组件渲染到这里 -->
    <router-view></router-view>
  </div>
</template>

<script>
  export default {
    name: 'app',

    data () {
      return {
      }
    },

    beforeCreate () {
      console.log('App实例创建之前,什么都访问不到')
      console.log(this, this.$el, this.$option, this.$data)
    },
    created () {
      console.log('App实例创建完成，data，prop准备好')
      console.log(this, this.$el, this.$option, this.$data)
    },
    beforeMount () {
      debugger
      console.log('App实例挂载之前，进行占位？')
      console.log(this, this.$el, this.$option, this.$data)
    },
    mounted () {
      debugger
      console.log('App实例挂载完成，真实数据进行占位填充')
      console.log(this, this.$el, this.$option, this.$data)
    }
  }
</script>

<style lang="scss" scoped>

</style>
