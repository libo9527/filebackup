## Mockjs

> [官网](http://mockjs.com/)

### Vue 中使用 Mockjs

1. 安装 mockjs

   ```shell
   npm install mockjs --save
   ```

2. src 下新建 mock 目录，在该目录下新建 index.js 文件

   ```js /src/mock/index.js
   import Mock from 'mockjs'
   
   Mock.mock('/api/user', 'get', {
     'code': 200,
     'message': 'success',
     'data|1-10': [{
       'id|+1': 10,
       'username': '@cname',
       'password': '@string'
     }]
   })
   ```

3. main.js 中 引入 `mock/index.js`

   ```js
   import './mock/index'
   ```

4. 组件中请求数据

   ```vue
   <template>
   <div class="hello" align="center">
     <el-table :data="tableData" style="width: 20%; align: center;">
       <el-table-column label="User #" prop="id"></el-table-column>
       <el-table-column label="Username" prop="username"></el-table-column>
       <el-table-column label="Password" prop="password"></el-table-column>
     </el-table>
     </div>
   </template>
   
   <script>
     export default {
       name: 'Test',
       data () {
         return {
           tableData: []
         }
       },
       created () {
         this.getUsers()
       },
       methods: {
         getUsers () {
           this.$axios.get('/api/user').then(res => {
             // console.log('res.data', res.data)
             if (res.data.code === 200) {
               this.tableData = res.data.data
             }
           })
         }
       }
     }
   </script>
   ```

   