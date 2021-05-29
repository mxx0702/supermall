<template>
   <tab-bar>
     <tab-bar-item path="/home" activeColor="red">
       <img src="~assets/img/shouye.png" alt="" slot="item-icon">
       <img src="~assets/img/shouye-active.png" alt="" slot="item-icon-active">
       <div slot="item-text">首页</div>
     </tab-bar-item>
     <tab-bar-item  path="/category" activeColor="blue">
       <img src="~assets/img/zan.png" alt="" slot="item-icon">
       <img src="~assets/img/zan-active.png" alt="" slot="item-icon-active">

       <div slot="item-text">分类</div>
     </tab-bar-item>
     <tab-bar-item  path="/cart" activeColor="blue">
       <img src="~assets/img/youjian.png" alt="" slot="item-icon">
       <img src="~assets/img/youjian-active.png" alt="" slot="item-icon-active">
       <div slot="item-text">购物车</div>

     </tab-bar-item>
     <tab-bar-item  path="/profile" activeColor="blue">
       <img src="~assets/img/bussiness-man.png" alt="" slot="item-icon">
       <img src="~assets/img/bussiness-man-active.png" alt="" slot="item-icon-active">

       <div slot="item-text">我的</div>
      </tab-bar-item>    

   </tab-bar>
</template>

<script>
import TabBarItem from 'components/common/tabbar/TabBarItem.vue'
import TabBar from'components/common/tabbar/TabBar.vue'
export default {
  name: 'MainTabBar',
  components:{
     TabBarItem,
     TabBar 
  }
}
</script>

<style>

</style>
