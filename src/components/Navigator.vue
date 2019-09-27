<template>
<el-menu
  :default-active="activeIndex2"
  class="el-menu-demo"
  mode="horizontal"
  @select="handleSelect"
  background-color="#3E99C9"
  text-color="#FFF"
  
  >
  <el-submenu index="1">
    <template slot="title">About</template>
    <el-menu-item index="1-1">About RCAR 2020</el-menu-item>
    <el-menu-item index="1-2">Experience Asahikawa</el-menu-item>
    <el-menu-item index="1-3">Conference Venue</el-menu-item>
    <el-menu-item index="1-4">Contact Us</el-menu-item>
    <el-menu-item index="1-5">Photos and Videos</el-menu-item>
  </el-submenu>
  <el-submenu index="2">
    <template slot="title">Organization</template>
    <el-menu-item index="2-1">Organizing Committee</el-menu-item>
    <el-menu-item index="2-2">Advisory Council</el-menu-item>
    <el-menu-item index="2-3">Senior Program Committee</el-menu-item>
    <el-menu-item index="2-4">RCAR Conference Paper Review Board</el-menu-item>
    <el-menu-item index="2-5">RA-Letters Editorial Board</el-menu-item>
  </el-submenu>
  <el-submenu index="3">
    <template slot="title">Program</template>
    <el-menu-item index="3-1">Program at a Glance</el-menu-item>
    <el-menu-item index="3-2">Techninal Program</el-menu-item>
    <el-menu-item index="3-3">Plenaries</el-menu-item>
    <el-menu-item index="3-4">Keynotes</el-menu-item>
    <el-menu-item index="3-5">Workshops and Tutorials</el-menu-item>
    <el-menu-item index="3-6">Pioneer's Talks</el-menu-item>
    <el-menu-item index="3-7">Industrial CEO Summit Forum</el-menu-item>
    <el-menu-item index="3-8">Government Forum</el-menu-item>
    <el-menu-item index="3-9">Cutting Edge Forums</el-menu-item>
  </el-submenu>
  <el-submenu index="4">
    <template slot="title">Contributing</template>
    <el-menu-item index="4-1">Instructions for Presenters</el-menu-item>
    <el-menu-item index="4-2">Final Paper Sumission</el-menu-item>
    <el-menu-item index="4-3">Instructions for Selected TRO and RAM papers</el-menu-item>
    <el-menu-item index="4-4">Call for Papers</el-menu-item>
    <el-menu-item index="4-5">Call for Organized Sessions</el-menu-item>
    <el-menu-item index="4-6">Call for Special Forums</el-menu-item>
    <el-menu-item index="4-7">Call for Cutting Edge Forums</el-menu-item>
    <el-menu-item index="4-8">Call for Workshops&Tutorials</el-menu-item>
    <el-menu-item index="4-9">Call for Competitions</el-menu-item>
    <el-menu-item index="4-10">Call for Late Breaking Results Poster</el-menu-item>
  </el-submenu>
  <el-submenu index="5">
    <template slot="title">Competitions</template>
    <el-menu-item index="5-1">Call for Competitions</el-menu-item>
    <el-menu-item index="5-2">Competition Schedule</el-menu-item>
  </el-submenu>
  <el-submenu index="6">
    <template slot="title">Registration & Travel</template>
    <el-menu-item index="6-1">Registration</el-menu-item>
    <el-menu-item index="6-2">Accommodation</el-menu-item>
    <el-menu-item index="6-3">Travel Awards</el-menu-item>
    <el-menu-item index="6-3">Transportation</el-menu-item>
    <el-menu-item index="6-4">Visa Information</el-menu-item>
  </el-submenu>
  <el-submenu index="7">
    <template slot="title">Sponsors & Exhibitors</template>
    <el-menu-item index="7-1">List of Sponsors and Exhibitors</el-menu-item>
    <el-menu-item index="7-2">Job Openings</el-menu-item>
    <el-menu-item index="7-3">Call for Sponsorship and Ehibition</el-menu-item>
  </el-submenu>
  <el-submenu index="8">
    <template slot="title">Job & Events</template>
    <el-menu-item index="8-1">IEEE RAS Jobs and Events</el-menu-item>
    <el-menu-item index="8-2">RCAR Con</el-menu-item>
  </el-submenu>
  <!-- <el-menu-item index="3" disabled>消息中心</el-menu-item>
  <el-menu-item index="4"><a href="https://www.ele.me" target="_blank">订单管理</a></el-menu-item> -->
</el-menu>

</template>

<script>
  export default {
    data() {
      return {
        activeIndex2: '1'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>