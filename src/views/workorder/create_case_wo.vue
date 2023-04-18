<template>
    <div class="app-container">
        <!-- <div class="main-content"></div> -->
        <el-card shadow="always" :body-style="{ padding: '20px' }">
            <div slot="header">
                <span>公共信息</span>
            </div>
            <!-- card body 部分 -->
            <div>
                <el-form :model="testCreateCaseForm" ref="form" :rules="rules" label-width="80px" :inline="false" size="normal">
                    <el-form-item label="标题">
                        <el-input v-model="testCreateCaseForm.test"></el-input>
                    </el-form-item>
                    <el-form-item>
                        <el-button type="primary" @click="onSubmit">立即创建</el-button>
                        <el-button>取消</el-button>
                    </el-form-item>
                </el-form>
                
            </div>
        </el-card>
    </div>
</template>

<script>
export default{
    data(){
        return {
            testCreateCaseForm:{
                test: "aaa"
            },
        }
    },
}
</script>

<style>
.main-content{
    width: 100px;
    height: 100px;
    background-color: aqua;
}
</style>