<template>
    <div>
        <Menu mode="vertical" theme="light" active-name="1" width="auto">
            <MenuItem name="home">
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
        </Menu>
    </div>
</template>

<script>
export default {
    name:'sidebar',
    data() {
        return {
            
        }
    },
    methods: {

    },
}
</script>
<style scoped>
</style>