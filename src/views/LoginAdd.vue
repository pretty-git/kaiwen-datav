<template>
    <div class="main">
        <div class="login">
            <div class="login-title">中央控制管理系统</div>
            <el-form :model="ruleForm" :rules="rules" ref="ruleForm" label-width="100px" class="demo-ruleForm">
                <el-form-item label="账号" prop="count">
                    <el-input v-model="ruleForm.count"></el-input>
                </el-form-item>
                <el-form-item label="密码" prop="pass">
                    <el-input type="password" v-model="ruleForm.pass" autocomplete="off"></el-input>
                </el-form-item>

                <el-form-item>
                    <el-button type="primary" @click="submitForm('ruleForm')">立即登录</el-button>
                </el-form-item>
            </el-form>
        </div>
    </div>
</template>

<script>
export default {
    name: 'LoginAdd',
    data() {
        return {
            ruleForm: {
                count: '',
                pass: ''
            },
            rules: {}
        }
    },
    beforeCreate() {
        //生成虚拟demo
    },
    created() {
        //完成了虚拟demo
    },
    beforeMount() {
        //         渲染demo之前
    },
    mounted() {
        //渲染demo完成
    },
    beforeUpdate() {
        //更新之前
    },
    updated() {
        //完成demo页面更新
    },
    beforeDestroy() {
        //组件之前
    },
    destroyed() {
        //组件完成销毁
    },
    methods: {
        submitForm() {

        }
    }


}
</script>

<style>
.main {
    width: 100%;
    height: 100vh;
    background: url('../assets/img/bg-2.jpg') no-repeat;
    background-size: cover;
    display: flex;
    align-content: center;
}
.login {
    width: 30%;
    min-width: 300px;
    margin: auto;
    background-color: aquamarine;
    
}
.login-title {
    text-align: center;
}
</style>