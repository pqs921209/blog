<template>
    <div>
        <Menu mode="horizontal" theme="primary" active-name="1" @on-select="onSelect">
            <MenuItem name="home" class="home-font">
                <Icon type="ios-home" />
                博客主页
            </MenuItem>
            <MenuItem name="1">
                <Icon type="ios-paper" />
                内容管理
            </MenuItem>
            <MenuItem name="2">
                <Icon type="ios-people" />
                用户管理
            </MenuItem>
            <MenuItem name="3">
                <Icon type="ios-stats" />
                统计分析                
            </MenuItem>
            <MenuItem name="4">
                <Icon type="ios-construct" />
                综合设置
            </MenuItem>
            <li name="login" class="right-item" @click="onSelect('login')">
                <Icon type="ios-log-in" />
                登录
            </li>
        </Menu>
    </div>
</template>

<script>
export default {
    name:'navbar',
    data() {
        return {
            
        }
    },
    methods: {
        onSelect(name){
            // this.$emit('on-select', name)
            alert(name)
        }
    },
}
</script>
<style scoped>
.home-font{
    font-size: 24px;
}
.right-item{
    color: #fff;
    float: right;
    padding: 0 20px;
    position: relative;
    cursor: pointer;
    z-index: 3;
    transition: all .2s ease-in-out;
}
</style>