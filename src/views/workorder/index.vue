<template>
    <div class="app-container">
        <el-card shadow="always" :body-style="{ padding: '20px' }">
            <div slot="header">
                <!-- <span>卡片头部</span> -->
                <el-form ref="form" :rules="rules" label-width="100px" :inline="true" size="normal">
                    <el-form-item label="工单类型查询">
                        <!-- <el-input v-model="woform.type"></el-input> -->
                        <el-input  placeholder="请输入工单名称" size="normal" clearable @change=""></el-input>
                    </el-form-item>
                    
                    <el-form-item>
                        <el-button type="primary" @click="onSubmit">确认查询</el-button>
                        <el-button>新建工单类型</el-button>
                    </el-form-item>
                </el-form>
            </div>
            卡片body
        </el-card>
        
    </div>
</template>


<script>
</script>
