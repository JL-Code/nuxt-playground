<script setup lang="ts">
definePageMeta({ layout: "ssr" });
</script>

<template>
    <div class="main">
        <el-scroller>
            <div class="scroll-container">
                <div class="affix-container">
                    <el-affix target=".scroll-container" :offset="200">
                        <el-button type="primary">Target container</el-button>
                    </el-affix>
                </div>
            </div>
        </el-scroller>
    </div>
</template>
<style>
* {
    margin: 0;
    padding: 0;
}

.main {
    text-align: center;
    height: 100vh;
    border-radius: 4px;
    background: red;
}

.scroll-container {
    height: 2800px;
    padding: 0 16px;
    background-color: aquamarine;
}

.affix-container {
    text-align: center;
    height: 100vh;
    border-radius: 4px;
    background: var(--el-color-primary-light-9);
}
</style>
