<template>
    <el-table
            :data="tableData"
            border
            style="width: 100%;text-align: left">
        <el-table-column
                prop="id"
                label="用户openID"
                width="300"
        text-alige>
        </el-table-column>
        <el-table-column
                prop="name"
                label="用户名"
                width="180">
        </el-table-column>
        <el-table-column
                prop="sex"
                label="性别(1:男，2女)"
                width="180">
        </el-table-column>
        <el-table-column
                prop="grade"
                label="会员等级"
                width="180">
        </el-table-column>
        <el-table-column
                prop="time"
                label="加入时间"
                width="180">
        </el-table-column>
        <el-table-column label="操作">
            <template scope="scope">
                <el-button
                        size="small"
                        @click="handleEdit(scope.$index, scope.row)">编辑</el-button>
                <el-button
                        size="small"
                        type="danger"
                        @click="handleDelete(scope.$index, scope.row)">删除</el-button>
            </template>
        </el-table-column>
    </el-table>
</template>

<script>
    export default {
        data() {
            return {
                tableData: [{
                    id: 'oU2M1wOZqhjLz3pd6r0RB1qi8KVY',
                    name: '王小虎',
                    sex: '1',
                    grade: '0',
                    time: '2017-09-19 15:42:57'
                }, {
                    id: 'oU2M1wOZqhjLz3pd6r0RB1qi8KVY',
                    name: '王小虎',
                    sex: '1',
                    grade: '0',
                    time: '2017-09-19 15:42:57'
                }, {
                    id: 'oU2M1wOZqhjLz3pd6r0RB1qi8KVY',
                    name: '王小虎',
                    sex: '1',
                    grade: '0',
                    time: '2017-09-19 15:42:57'
                }, {
                    id: 'oU2M1wOZqhjLz3pd6r0RB1qi8KVY',
                    name: '王小虎',
                    sex: '1',
                    grade: '0',
                    time: '2017-09-19 15:42:57'
                }]
            }
        },
        methods: {
            handleEdit(index, row) {
                console.log(index, row);
            },
            handleDelete(index, row) {
                console.log(index, row);
            }
        }
    }
</script>