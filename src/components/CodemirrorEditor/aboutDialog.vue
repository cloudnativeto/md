<template>
    <el-dialog
        title="关于"
        class="about__dialog"
        :visible="value"
        @close="$emit('input', false)"
        width="30%"
        center
    >
        <div style="text-align: center">
            <h3>云原生社区公众号 Markdown 编辑器</h3>
        </div>
        <div style="text-align: center; margin-top: 10px">
            <p>扫码关注云原生社区的公众号，获取云原生最新资讯！</p>
            <img
                src=""https://cloudnative.to/images/wechat-qrcode.png
                style="width: 40%; display: block; margin: 20px auto 10px"
            />
        </div>
        <span slot="footer" class="dialog-footer">
            <el-button
                type="primary"
                @click="onRedirect('https://github.com/cloudnativeto/md')"
                plain
                >GitHub 仓库</el-button
            >
            <el-button
                type="primary"
                @click="onRedirect('https://cloudnative.to')"
                plain
                >云原生社区</el-button
            >
        </span>
    </el-dialog>
</template>

<script>
export default {
    props: {
        value: {
            type: Boolean,
            default: false,
        },
    },
    methods: {
        onRedirect(url) {
            window.open(url);
        },
    },
};
</script>

<style lang="less" scoped></style>
