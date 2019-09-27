<template>
  <div>
    <div class="Header"><Head/></div>   
    <Navigator/>
    <Carousel/>
    <h4 class="pt-5">Important Data</h4>
    <el-row type="flex" class="row-bg" justify="space-around">
        <el-col :span="7.5"><div class="grid-content bg-purple"><TimeTable/></div></el-col>
    </el-row>

    <el-container>
        <h4 class="pt-2">Welcome Message</h4>
        <el-main class="pt-4">
        <el-row type="flex" class="row-bg" justify="space-around">
            <el-col :span="18"><div><Body/></div></el-col>
        </el-row>      
        </el-main>
        <el-footer class="pt-4">foot</el-footer>
    </el-container>

</div>
</template>

<script>
import Head from './../components/Head.vue'
import Carousel from './../components/Carousel.vue'
import Navigator from './../components/Navigator.vue'
import Body from './../components/Body.vue'
import TimeTable from './../components/TimeTable.vue'
export default {
  name: 'app',
  components: {
    Head,
    Navigator,   
    Carousel, 
    Body,
    TimeTable,
  }
}
</script>

<style>
   .Header{
      width:80%;
      margin-left: 10%;
  }

  /* .el-header, .el-footer {
    background-color: #B3C0D1;
    color: #333;
    text-align: center; 
     margin-left: 10%;
    width:80%;
  } */
    
   .el-main {
    text-align:justify;
  }
</style>