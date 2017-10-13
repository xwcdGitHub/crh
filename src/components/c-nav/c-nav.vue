<template>
    <el-row class="el-nav">
        <el-col :span="24">
            <el-menu default-active="2" class="el-menu-vertical-demo" @open="handleOpen" @close="handleClose">
                <el-submenu index="1">
                    <template slot="title"><i class="el-icon-message"></i><router-link to="/user">用户管理</router-link></template>
                    <el-menu-item-group>
                        <el-menu-item index="1-1">所有成员</el-menu-item>
                        <el-menu-item index="1-2">非会员</el-menu-item>
                        <el-menu-item index="1-3">普通会员</el-menu-item>
                        <el-menu-item index="1-4">高级会员</el-menu-item>
                    </el-menu-item-group>
                </el-submenu>
                <el-submenu index="2">
                    <template slot="title"><i class="el-icon-message"></i>活动管理</template>
                    <el-menu-item-group>
                        <el-menu-item index="2-1">所有活动</el-menu-item>
                    </el-menu-item-group>
                </el-submenu>
                <el-submenu index="3">
                    <template slot="title"><i class="el-icon-message"></i>管理员管理</template>
                    <el-menu-item-group>
                        <el-menu-item index="3-1">所有管理员</el-menu-item>
                    </el-menu-item-group>
                </el-submenu>
                <el-submenu index="4">
                    <template slot="title"><i class="el-icon-message"></i>订单管理</template>
                    <el-menu-item-group>
                        <el-menu-item index="4-1">未支付的所有订单</el-menu-item>
                        <el-menu-item index="4-2">已支付的说有订单</el-menu-item>
                        <el-menu-item index="4-2">待处理的超然订单</el-menu-item>
                    </el-menu-item-group>
                </el-submenu>
            </el-menu>
        </el-col>
    </el-row>
</template>

<script>
    export default {
        methods: {
            handleOpen(key, keyPath) {
                console.log(key, keyPath);
            },
            handleClose(key, keyPath) {
                console.log(key, keyPath);
            }
        }
    }
</script>

<style>
    .el-submenu{
        text-align: left;
    }
    .el-nav{
        width: 200px;
        float: left;
        background-color: #eef1f6;
    }
</style>
