- VUE 
   VueRouter 路由
   Vuex 数据流
   
   ElementUI PC
   MintUI/IVIew mobile

插件 
 Vue 瘦身 MVVM
 其他的都是他的周边生态
 插件机制往里面加
 Vue.use(plugin)
 plugin 按一定的规定
 this.$route
 Vue.prototype

- ElementUI 有两种引入组件的方式
   <el-button/>
 Vue-component(component.name,component)
 const components = []
component.forEach(
    (component) =>{
        Vue.component(component.name,component);
    }
)

- 写一个vue组件 ，开源的插件 100+
{
    install:function(){
       Vue.component(component.name,component)
       Vue.prototype.$message = Message;
    }
}
Vue.install(piugin) 执行install





