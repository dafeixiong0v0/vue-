<template>
    <div class="up">
        <h1>about</h1>
        <p>{{aboutMsg}}</p>
        <ast v-bind:my-message="parentMsg"></ast>
        <p>{{tle1}}:<comp :total="123+456">
                 
            </comp></p>  
        <p>{{tle2}}:<comp :total="1023+456"></comp></p>  

        <input type="text" v-model="parentMsg">
    </div>
</template>
<script>
    import ast from './com.vue'
    import comp from './表达式计算，传递值.vue'
    export default {
        components: {
            comp,ast
        },
        data () {
            return {
                aboutMsg: '我是about组件',
                tle1: '这里传递是字符串',  
                tle2: '用了v-bind动态语法，传递值会通过js的表达式计算，得到个值' ,
                parentMsg:'121212'
            }
        }
    }
</script>