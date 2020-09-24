<template>
  
  <div class="bg-white w-100 relative z-9999" >
      <el-row>
        <el-col :span="12">
          <div class="grid-content">
              <el-menu default-active="1" :style="{padding: '8px 12px 10px 12px'}" class="el-menu-demo" mode="horizontal" @select="handleSelect">
                <el-menu-item ><router-link :to="'/'"><img src="/public/logo.png" width="90" height="40"></router-link></el-menu-item>
                
              </el-menu>
          </div>
        </el-col>
        <el-col :span="12">
          <div class="grid-content bg-white text-right">
            <el-menu  :style="{padding: '8px 12px 10px 12px'}" :default-active="activeIndex" class="el-menu-demo" mode="horizontal">
              <el-menu-item ><router-link :to="'/'">Flights</router-link></el-menu-item>
              <el-menu-item ><a href="#" class="">Rooms</a></el-menu-item>
              <el-menu-item ><a href="#" class="">Help</a></el-menu-item>
              <!-- <el-menu-item >
                <a href="#" class="">
                  <el-button :style="{padding : '4px 8px 5px 8px'}" type="primary" circle>€</el-button>
                </a>
              </el-menu-item> -->
              <el-menu-item ><a href="#" class="">Manage Bookings</a></el-menu-item>
              <el-menu-item>
                <el-button type="primary" :style="{padding: '8px 12px 10px 12px'}" plain icon="">Contact Us</el-button>
              </el-menu-item>
            </el-menu>
          </div>
        </el-col>
      </el-row>
    
  </div>

</template>

<script>
  export default {
    name: 'header-nav',
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style>
</style>
