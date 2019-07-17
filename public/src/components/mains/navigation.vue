<template>
    <div>
        <div class="navigations">
            <div><img src="../../assets/images/linkbg.jpg" alt=""></div>
            <div style="padding: 10px 0;margin-right:-30px ">
                <Select v-model="model18" clearable style="width:240px;margin-right:10px">
                    <Option v-for="item in cityList" :value="item.value" :key="item.value">{{ item.label }}</Option>
                </Select>
                <Select v-model="model19" clearable style="width:240px;margin-right:10px">
                    <Option v-for="item in cityList2" :value="item.value" :key="item.value">{{ item.label }}</Option>
                </Select>
                <Select v-model="model20" clearable style="width:240px">
                    <Option v-for="item in cityList3" :value="item.value" :key="item.value">{{ item.label }}</Option>
                </Select>
            </div>
            <div><img src="../../assets/images/linkbg2.jpg" alt=""></div>
        </div>


    </div>

</template>

<script>
    export default {
        data () {
            return {
                cityList: [
                    {
                        value: '全国导航',
                        label: '全国导航'
                    },
                    {
                        value: '公安部',
                        label: '公安部'
                    },
                    {
                        value: '北京',
                        label: '北京'
                    },
                ],
                model18:'全国导航',
                cityList2: [
                    {
                        value: '省内导航',
                        label: '省内导航'
                    },
                    {
                        value: '咸阳',
                        label: '咸阳'
                    },
                    {
                        value: '西安',
                        label: '西安'
                    },
                ],
                model19:'省内导航',
                cityList3: [
                    {
                        value: '市内导航',
                        label: '市内导航'
                    },
                    {
                        value: '市局',
                        label: '市局'
                    },
                    {
                        value: '渭城',
                        label: '渭城'
                    },
                ],
                model20:'市内导航'
            }
        },
        methods: {
            maxTagPlaceholder (num) {
                return 'more '+ num;
            }
        }
    }
</script>

<style scoped>
.navigations{
    border:1px solid #ccc;
    width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    height: 50px;
}


</style>