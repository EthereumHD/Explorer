<template>
    <div class="footer">
        <div class="footer-info">@{{ tYear }} Powered by EHD</div>
    </div>
</template>
<script>
export default {
    name: "footBottom",
    data() {
        return {
            tYear: ""
        };
    },
    mounted() {
        this.doHandleYear();
    },
    methods: {
        doHandleYear() {
            let myDate = new Date();
            this.tYear = myDate.getFullYear();
        }
    }
};
</script>
<style scoped>
.footer {
    padding-top: 30px;
    width: 100%;
    line-height: 60px;
    color: #9b9b9b;
    font-size: 12px;
    clear: both;
    text-align: center;
}
</style>
