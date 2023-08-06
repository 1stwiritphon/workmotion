<template>
<div class="nav d-flex">
  
    <nuxt-link to="/">หน้าหลัก</nuxt-link>
    <nuxt-link to="/service">บริการของเรา</nuxt-link>
    <nuxt-link to="/article">บทความจากเรา</nuxt-link>
    <nuxt-link to="/about">เกี่ยวกับเรา</nuxt-link>
    <nuxt-link to="/partner">พาร์ทเนอร์</nuxt-link>
    <nuxt-link to="/team">สมาชิก</nuxt-link>
    <nuxt-link to="/contact">ติดต่อเรา</nuxt-link>

</div>
</template>

<script>
export default {
  name: "navbar",
};
</script>

<style scoped>
.nav {
  margin-top: 49px;
  position: fixed;
}
a {
text-decoration: none;
margin-right: 40px;
font-family: 'SF Pro Text';
font-style: normal;
font-weight: 600;
font-size: 16px;
line-height: 19px;
/* identical to box height */


color: rgba(255, 255, 255, 0.5);
}
a:hover {
color: #fff;
}
</style>