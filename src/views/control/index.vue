<template>
  <div>
    <!-- 卡片 -->
    <el-row :gutter="15">
      <el-col :span="8">
        <card bg="success"></card>
      </el-col>
      <el-col :span="8">
        <card bg="warning"></card>
      </el-col>
      <el-col :span="8">
        <card bg="danger"></card>
      </el-col>
    </el-row>
    <!-- 图表 -->
    <!-- <el-row style="margin-top:20px">
      <el-col>
        <LineChart />
      </el-col>
    </el-row> -->
  </div>
</template>

<script>
// import LineChart from "@/components/lineChart";
import Card from "@/components/card";
export default {
  name: "control",
  components: {
    Card,
    // LineChart,
  },
  data() {
    // this.chartSettings = {
    //   area: true,
    // };
    return {
      chartData: {
        columns: ["日期", "访问用户", "下单用户", "下单率"],
        rows: [
          { 日期: "1/1", 访问用户: 1393, 下单用户: 1093, 下单率: 0.32 },
          { 日期: "1/2", 访问用户: 3530, 下单用户: 3230, 下单率: 0.26 },
          { 日期: "1/3", 访问用户: 2923, 下单用户: 2623, 下单率: 0.76 },
          { 日期: "1/4", 访问用户: 1723, 下单用户: 1423, 下单率: 0.49 },
          { 日期: "1/5", 访问用户: 3792, 下单用户: 3492, 下单率: 0.323 },
          { 日期: "1/6", 访问用户: 4593, 下单用户: 4293, 下单率: 0.78 },
        ],
      },
    };
  },
};
</script>

<style>
</style>