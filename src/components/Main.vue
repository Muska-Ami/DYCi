<script setup>
import { ref } from 'vue'
import Footer from "@/layouts/Footer.vue"

let dialogVisible = ref(false)
</script>

<template>
    <el-main>

        <h1 class="ext-title">Daiyangcheng</h1>
        <p><el-text class="mx-1" type="danger">❤L❤O❤V❤E❤</el-text></p>

        <el-card class="box-card">
            <template #header>
                <div class="card-header">
                    <span>戴先生我最爱<el-text class="mx-1" type="danger">❤</el-text>！</span>
                    <el-button class="button" text @click="dialogVisible = true">awa!</el-button>
                </div>
            </template>
            <div class="text item">
                <el-avatar src="https://q1.qlogo.cn/g?b=qq&nk=3143105972&s=640" />
            </div>
            <h1>Daiyangcheng</h1>
            <p>Daiyangcheng<el-text class="mx-1" type="danger">❤</el-text>，🤤🤤🤤🤤🤤......🤤🤤🤤......</p>
            <p>🥰🥰🥰🥰🥰🥰</p>
        </el-card>

        <el-dialog v-model="dialogVisible" title="Tips" width="30%">
            <h2>被你发现了！</h2>
            <span>这是个按钮唉</span>
            <template #footer>
                <span class="dialog-footer">
                    <el-button type="primary" @click="dialogVisible = false">
                        关掉！
                    </el-button>
                </span>
            </template>
        </el-dialog>
        <Footer />
    </el-main>
</template>
