<template>
  <div class="body">
    <div class="panels">
      <table class="table table-hover" rules=rows frame=below>
        <thead>
          <tr>
            <th>编号</th>
            <th>标题</th>
            <th>状态</th>
            <th>操作</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(list, index) in currentList">
            <td>{{index + 1}}</td>
            <td>{{list.title}}</td>
            <td>{{list.status}}</td>
            <td><span class="blue">编辑</span>&nbsp;&nbsp;<span class="red">删除</span></td>
          </tr>
        </tbody>
      </table>
    </div>
    <pagination :num="num" :limit="limit" @getNew="getNew"></pagination>
  </div>
</template>

<script>
  import pagination from "./pagination.vue"
  export default {
    name: 'demo',
    data() {
      return {
        num: 0,
        limit: 10,
        currentList: [],
        dataList: [{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },
          {
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },
          {
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          },{
            title: "test1, kelvin",
            view: "6",
            status: "正常"
          }
        ]
      }
    },
    components: {
      pagination
    },
    methods: {
      getNew(value) {
        this.currentList = this.dataList.slice(value, value + this.limit);
      }
    },
    mounted() {
      this.getNew(0);
      this.num = this.dataList.length;
    }
  }

</script>

<style scoped>
  .body {
    background-color: #ffffff;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    justify-content: flex-start;
    font-size: 12px;
    color: #606266;
  }

  .blue {
    color: #409EFF;
  }

  .red {
    color: #FF6947;
  }

  .panels {
    text-align: center;
  }

  .panels tr {
    height: 40px;
    text-align: center;
  }

  .panels th {
    text-align: center;
  }

  table {
    border: #eeeeee;
  }

</style>
