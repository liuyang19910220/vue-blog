<template>
  <i-col :span="spanLeft" class="layout-menu-left">
    <Menu active-name="1" theme="dark" width="auto">
        <div class="layout-logo-left"></div>
        <Menu-item name="1">
             <router-link to="/" activeClass="active" exact><Icon type="home" :size="iconSize"></Icon></router-link>
            <span class="layout-text"> <router-link to="/" activeClass="active" exact>平台首页</router-link></span>
        </Menu-item>
        <Menu-item name="2">
            <router-link to="/user" activeClass="active"><Icon type="person" :size="iconSize"></Icon></router-link>
            <span class="layout-text"> <router-link to="/user" activeClass="active">用户模块</router-link></span>
        </Menu-item>
        <Menu-item name="3">
            <router-link to="/log" activeClass="active"><Icon type="document-text" :size="iconSize"></Icon></router-link>
            <span class="layout-text"> <router-link to="/log" activeClass="active">日志模块</router-link></span>
        </Menu-item>
        <Menu-item name="4">
            <router-link to="/upload" activeClass="active"><Icon type="pin" :size="iconSize"></Icon></router-link>
            <span class="layout-text"> <router-link to="/upload" activeClass="active">上传模块</router-link></span>
        </Menu-item>
         <Menu-item name="5">
            <router-link to="/cate" activeClass="active"><Icon type="folder" :size="iconSize"></Icon></router-link>
            <span class="layout-text"> <router-link to="/cate" activeClass="active">分类模块</router-link></span>
        </Menu-item>
    </Menu>
</i-col>
</template>

<script>
    export default {
        props:['spanLeft','iconSize']
    }
</script>

<style lang="scss" scoped>
    .active{
        color:white!important;
    }
</style>