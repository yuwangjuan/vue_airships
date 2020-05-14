<template>
  
      <div class="main_box">
          <div class="main_left">
            <div class="main_left_head">
              <p class="main_left_text"><span>第</span><span class="add_red">2020051</span><span>期:</span><span class="add_blue">10,10,10</span></p>
              <p class="main_left_time"> <span class="right_time">05:00</span></p>
            </div>
            <div class="main_left_contain_left">
            <p class="reward_list0">开奖列表：</p>
            <!-- <a-table  :columns="columns" :dataSource="data" /> --><el-table
      :data="tableData"
      class="tab_sly">
      <el-table-column
        prop="date"
        label="期号"
        >
      </el-table-column>
      <el-table-column
        prop="name"
        label="开奖号码"
        >
      </el-table-column>
    </el-table>
            </div>
            <div class="main_left_contain_right">
            <p class="reward_list"><span class="format_list">公式列表：</span>
            <span><a-checkbox>全选</a-checkbox></span>
            <span><a-checkbox>反选</a-checkbox></span>
            <span class="stop_win">止赢：<a-input-number></a-input-number></span>
            <span class="stop_lose">止损：<a-input-number></a-input-number></span>
            <span class="get_change"><a-button type="primary">修改</a-button></span>
            <span class="all_get">总亏盈：</span>
            </p>
            <!-- <a-table class="tab_left" :columns="columns1" :data-source="dataSource1" ></a-table> -->
            <el-table
      :data="tableData1"
      class="tab1_sly">
      <el-table-column
        prop="date"
        label="期号"
        >
      </el-table-column>
      <el-table-column
        prop="name"
        label="开奖号码"
        >
      </el-table-column>
    </el-table>
            </div>
          </div>
          <div class="main_right">
          <div class="main_right_box">
         <div class="all_mn"><a-checkbox>全部模拟下注</a-checkbox></div> 
            <div class="a_select_box">
            <a-select defaultValue="lucy"  class="add_width">
            <a-select-option value="jack" class="add_width">Jack</a-select-option>
            <a-select-option value="lucy" class="add_width">Lucy</a-select-option>
            <a-select-option value="disabled" class="add_width">
              Disabled
            </a-select-option>
            <a-select-option value="Yiminghe">yiminghe</a-select-option>
          </a-select>
            </div>
            <div class="a_select_box">
            <a-select defaultValue="lucy" class="add_width" >
            <a-select-option value="jack" class="add_width">Jack</a-select-option>
            <a-select-option value="lucy" class="add_width">Lucy</a-select-option>
            <a-select-option value="disabled" class="add_width">
              Disabled
            </a-select-option>
            <a-select-option value="Yiminghe" class="add_width">yiminghe</a-select-option>
          </a-select>
            </div>
            <div class="right_btn">
                <p><a-button type="primary" class="btn_top" >开始</a-button></p>
                <p><a-button type="danger" class="btn_top1" >停止</a-button></p>
                <p><a-button type="primary" class="btn_top2" >账号</a-button></p>
                <p><a-button type="primary" class="btn_top3" >公式</a-button></p>
                <p><a-button type="primary" class="btn_top4" >设置</a-button></p>
               <p> <a-button type="primary" class="btn_top5" >删除</a-button></p>
               <p> <a-button type="primary" class="btn_top6" >清空</a-button></p>
            </div>
          </div>
          
          </div>
      </div>
      
</template>

<script>

const dataSource1 = [
  {
    key: '1',
    name: '胡彦斌',
    age: 32,
  },
  {
    key: '2',
    name: '胡彦祖',
    age: 42,
  },
  {
    key: '2',
    name: '胡彦祖',
    age: 42,
  },
  {
    key: '2',
    name: '胡彦祖',
    age: 42,
  },
  {
    key: '2',
    name: '胡彦祖',
    age: 42,
  },
  {
    key: '2',
    name: '胡彦祖',
    age: 42,
  },
  {
    key: '2',
    name: '胡彦祖',
    age: 42,
  },
  {
    key: '2',
    name: '胡彦祖',
    age: 42,
  },
  {
    key: '2',
    name: '胡彦祖',
    age: 42,
  },
];

const columns1 = [
  {
    title: '序号',
    dataIndex: 'name',
    key: 'name',
  },
  {
    title: '公式名称',
    dataIndex: 'age',
    key: 'age',
  },
  {
    title: '位置',
    dataIndex: 'age',
    key: 'age',
  },
  {
    title: '号码',
    dataIndex: 'age',
    key: 'age',
  },
  {
    title: '金额',
    dataIndex: 'age',
    key: 'age',
  },
  {
    title: '中奖',
    dataIndex: 'age',
    key: 'age',
  },
  {
    title: '盈亏',
    dataIndex: 'age',
    key: 'age',
  },
  {
    title: '余额',
    dataIndex: 'age',
    key: 'age',
  },
  {
    title: '模拟下注',
    dataIndex: 'age',
    key: 'age',
  },
  {
    title: '开始停止',
    dataIndex: 'age',
    key: 'age',
  },
];
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
       tableData: [{
            date: '2016',
            name: '王小虎',
            
          }, {
            date: '2016',
            name: '王小虎',
            
          }, {
            date: '2016',
            name: '王小虎',
            
          }, {
            date: '2016',
            name: '王小虎',
            
          }],
           tableData1: [{
            date: '2016',
            name: '王小虎',
            
          }, {
            date: '2016',
            name: '王小虎',
            
          }, {
            date: '2016',
            name: '王小虎',
            
          }, {
            date: '2016',
            name: '王小虎',
            
          }],
      data : [
  {
    key: '1',
    name: 'John Brown',
    age: 32,
    address: 'New York No. 1 Lake Park',
    tags: ['nice', 'developer'],
  },
  {
    key: '2',
    name: 'Jim Green',
    age: 42,
    address: 'London No. 1 Lake Park',
    tags: ['loser'],
  },
  {
    key: '3',
    name: 'Joe Black',
    age: 32,
    address: 'Sidney No. 1 Lake Park',
    tags: ['cool', 'teacher'],
  },
],

columns : [
  {
    dataIndex: 'name',
    key: 'name',
    slots: { title: 'customTitle' },
    scopedSlots: { customRender: 'name' },
  },
  {
    title: 'Age',
    dataIndex: 'age',
    key: 'age',
  },
  {
    title: 'Address',
    dataIndex: 'address',
    key: 'address',
  },
  {
    title: 'Tags',
    key: 'tags',
    dataIndex: 'tags',
    scopedSlots: { customRender: 'tags' },
  },
  {
    title: 'Action',
    key: 'action',
    scopedSlots: { customRender: 'action' },
  },
  
],
      dataSource1,
      columns1,
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style >
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
*{
  margin:0;
  padding:0;
}
/* html,body{
  width:100%;
  height:100%;
} */
.main_box{
  margin:5px;
  height:calc(100vh - 10px);
}
.main_left{
  width:82%;
  /* background:blue; */
  display:inline-block;
  height:calc(100vh - 10px);
  /* border:1px solid #afa; */
  float:left;
}
.main_right{
  width:17%;
  display:inline-block;
  height:calc(100vh - 10px);
  vertical-align: top;
}
.main_left_head{
  width:100%;
  height:100px;
  /* border:1px solid yellow; */
  font-size: 45px;
  
}
.add_red{
  color:red;
  /* padding: 0 10px; */
}
.add_blue{
  color:blue;
  /* padding-left:20px; */
}
.main_left_text{
  text-align:center;
  /* width:83%; */
  display:inline-block;
}
.main_left_time{
  width:10%;
  /* text-align:right; */
  display:inline-block;
  color:red;
  /* font-size: 45px; */
}
.main_left_contain_left{
    width:30%;
    height:calc(100vh - 110px);
    display:inline-block;
    float:left;
    border:1px solid grey;
    
}
.main_left_contain_right{
  width:69%;
  height:calc(100vh - 110px);
  display:inline-block;
  margin-left:1%;
  float:right;
  border:1px solid grey;
  
}
.tab_left{
  border:1px solid grey;
  height:calc(100vh - 10px);
 
}
.reward_list0{
  height:120px;
  line-height:120px;

  
}
.reward_list{
  height:50px;
  line-height:50px;
  margin-bottom:90px;
  
}
.format_list{
  padding-right:100px;
  height:50px;
}
.stop_win{
  color:#0187fb;
  padding: 35px;
}
.stop_lose{
  color:#0187fb;
  padding-left:10px;
}
.all_get{
  color:#0187fb;
  padding: 50px;
}
.get_change{
  padding-left:70px;
}
.main_right_box{
  /* border:1px solid #afa; */
  margin-left:10px;
  font-size:50px;
}
.a_select_box{
  margin:10px 0;
  /* margin-top:70px; */
}
.all_mn{
  /* margin-top:-180px; */
}
.add_width{
  width:110px;
}
.btn_top{
  top:-10px;
  /* height:30px; */
}
.btn_top1{
  top:-50px
}
.btn_top2{
  top:-100px
}
.btn_top3{
  top:-150px
}
.btn_top4{
  top:-200px
}
.btn_top5{
  top:-200px
}
.btn_top6{
  top:-250px
}
.tab_sly{
  width:100%;
  overflow-x:auto;
 
}
.tab1_sly{
  width:100%;
  overflow-x:auto;
  margin-top:40px;
}
/* .ant-btn{
  height:2rem !important;
  line-height: 2rem !important;
} */

</style>
