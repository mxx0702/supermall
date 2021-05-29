<template>
   <div class="tabbaritem" @click="itemclick">
         <div v-if="isActive"><slot  name="item-icon-active"></slot></div>  
         <div v-else><slot  name="item-icon"></slot></div>
         <div v-bind:style="activeStyle"><slot   name="item-text"></slot></div>
   </div>
</template>

<script>

export default {
  name: 'TabBarItem',
  computed:{
    isActive(){
      return this.$route.path.indexOf(this.path)!==-1
    },
     activeStyle(){
      return this.isActive ? {color:this.activeColor} : {}
    }

  },
  props:{
    path:String,
    activeColor:{
      type:String,
     
    }
  },
  methods:{
    itemclick(){
      this.$router.push(this.path)
      
    }
  },
 
 
}
</script>

<style>
 .tabbaritem {
  flex: 1;
  text-align: center;
  height: 49px;
  font-size:14px;

}


</style>
