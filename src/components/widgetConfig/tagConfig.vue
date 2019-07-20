<template>
  <div>
    <el-form-item label="内容">
      <el-input v-model="data.options.value"></el-input>
    </el-form-item>
    <el-form-item label="大小">
      <el-radio-group v-model="data.options.size">
        <el-radio-button label="medium">较大</el-radio-button>
        <el-radio-button label>默认</el-radio-button>
        <el-radio-button label="mini">较小</el-radio-button>
      </el-radio-group>
    </el-form-item>
    <el-form-item label="主题">
      <el-radio-group v-model="data.options.effect">
        <el-radio-button label="light">light</el-radio-button>
        <el-radio-button label="dark">dark</el-radio-button>
        <el-radio-button label="plain">plain</el-radio-button>
      </el-radio-group>
    </el-form-item>
    <el-form-item label="类型">
      <el-radio-group v-model="data.options.type" size="mini">
        <el-radio-button label>默认</el-radio-button>
        <el-radio-button label="success">成功</el-radio-button>
        <el-radio-button label="info">信息</el-radio-button>
        <el-radio-button label="warning">警告</el-radio-button>
        <el-radio-button label="danger">危险</el-radio-button>
      </el-radio-group>
    </el-form-item>

    <el-form-item label="边框">
      <el-switch v-model="data.options.hit" active-text="开启" inactive-text="关闭"></el-switch>
    </el-form-item>
    <el-form-item label="背景颜色">
      <el-color-picker v-model="data.options.color"></el-color-picker>
    </el-form-item>
    <el-form-item label="字体颜色">
      <el-color-picker v-model="data.options.fontColor"></el-color-picker>
    </el-form-item>
  </div>
</template>

<script>
export default {
  props: {
    data: Object
  }
};
</script>

<style>
</style>
