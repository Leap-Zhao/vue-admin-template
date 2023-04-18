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
                        <el-button type="primary" icon="el-icon-search" @click="onSubmit">查询</el-button>
                        <el-button icon="el-icon-circle-plus">新建工单类型</el-button>
                    </el-form-item>
                </el-form>
            </div>
            <div class="workflow-classify-title" style="margin-bottom: 20px;">
            Demo演示
            </div>
            <!-- <el-button type="" size="default" @click="" class="ow-body-content">
                <div style="" class="ow-body-content-main-icon"><i class="el-icon-s-unfold"></i></div>
                <div class= "ow-body-content-main-title" style="">自动化工单</div>
                <div class="ow-body-content-sub-title">用于提交自动化问题</div>
            </el-button> -->
            
            <!-- <div class="ow-body-content">
                <el-button type="" size="default" @click=""> -->
                    <!-- <div style="font-size: 30px;"><i class="el-icon-s-unfold"></i></div>
                    <div>自动化工单</div>
                    <div>针对自动化环境问题</div> -->
                <!-- </el-button>
            </div> -->
            <div class="workflow-classify-div">
                <el-button style="width: 100%" plain @click="">
                    <div class="process-button-div">
                        <div class="process-div-icon">
                            <i class="el-icon-s-unfold" style="font-size: 30px; padding-top: 8px;"></i> 
                        </div>
                        <div class="process-div-body">
                            <div class="process-div-title ellipsis">
                                自动化工单
                            </div>
                            <div class="process-div-remarks ellipsis">
                                提交自动化中的环境问题
                            </div>
                        </div>
                    </div>
                </el-button>
            </div>
            <div class="workflow-classify-div">
                <el-button style="width: 100%" plain @click="">
                    <div class="process-button-div">
                        <div class="process-div-icon">
                            <i class="el-icon-folder" style="font-size: 30px; padding-top: 8px;"></i> 
                        </div>
                        <div class="process-div-body">
                            <div class="process-div-title ellipsis">
                                项目工单
                            </div>
                            <div class="process-div-remarks ellipsis">
                                提交项目中的环境问题
                            </div>
                        </div>
                    </div>
                </el-button>
            </div>
            <div class="workflow-classify-div">
                <el-button style="width: 100%" plain @click="">
                    <div class="process-button-div">
                        <div class="process-div-icon">
                            <i class="el-icon-menu" style="font-size: 30px; padding-top: 8px;"></i> 
                        </div>
                        <div class="process-div-body">
                            <div class="process-div-title ellipsis">
                                其它工单
                            </div>
                            <div class="process-div-remarks ellipsis">
                                提交其它环境问题
                            </div>
                        </div>
                    </div>
                </el-button>
            </div>
        </el-card>
    </div>
</template>


<script>
</script>

<style>
.ow-body-content{
    /* background-color: antiquewhite; */
    /* height: 100px; */
    width: 200px;
    height: 100px;
}

.workflow-classify-title{
    padding-left: 5px;
    border-left: 3px solid rgb(64, 158, 255);
}
.workflow-classify-div {
    width: 20%;
    display: inline-block;
    margin-left: 0;
    margin-top: 12px;
    margin-right: 12px;
    /* background-color: yellow; */
}
.process-div-icon {
    float: left;
    width: 50px;
    height: 100%;
    margin-right: 10px;
    /* background-color: antiquewhite; */
    /* font-size: 30px; */
}
.process-div-body {
    float: left;
    width: 150px;
    height: 100%;
    text-align: left;
    /* background-color: red; */
}
.process-div-title {
    font-size: 15px;
    margin-top: 6px;
    color: #606266;
    height: 18px;
    line-height: 18px;
}
.process-div-remarks {
    color: #999999;
    margin-top: 6px;
    font-size: 12px;
}

.ellipsis {
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
}


.ow-body-content-main-icon{
    font-size: 30px; 
    /* background-color: yellow;  */
    /* width: 20%;  */
    float: left;
}

.ow-body-content-main-title{
    padding-left: 10px;
    float: left;
    font-size: 20px;
}

.ow-body-content-sub-title{
    float: right;
    padding-top: 10px;
    box-sizing: border-box;
}

</style>
