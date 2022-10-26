<!-- my-page.vue -->
<template>
    <div>
      <h1>子应用</h1>
      <el-input v-model="aa" placeholder=""></el-input>
      <!-- 
        name(必传)：应用名称
        url(必传)：应用地址，会被自动补全为http://localhost:3000/index.html
        baseroute(可选)：基座应用分配给子应用的基础路由，就是上面的 `/my-page`
       -->
      <micro-app name='app1' url='http://localhost:9532/'  baseroute='/my-page' keep-router-state></micro-app>
    </div>
  </template>
  <script>
  export default {
    name:'MicroApp122',
        data(){
            return {
                aa:''
            }
        }
    }

</script>
  