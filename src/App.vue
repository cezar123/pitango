<script setup>
    import {Delete} from '@element-plus/icons-vue';
</script>

<template>
    <div>
        <el-container>
            <el-header>
                <h1>Users(3)</h1>
                <el-button type="primary" size="normal">Create User</el-button>
            </el-header>
            <el-main>
                <div class="card" v-for="x in 4" :key="x">
                    <div class="wrap-img">
                        <img class="profile" src="@/assets/image.png" alt="">
                    </div>
                    <h3>Jane Doe</h3>
                    <p>email@gmail.com</p>
                    <div class="wrap-button">
                        <el-button type="danger" :icon="Delete" circle/>
                    </div>
                </div>
            </el-main>
        </el-container>
    </div>
</template>

<style scoped>

    .el-container {
        width: 33.3rem;
    }

    .el-header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1rem;
        height: 4.8rem;
        background: #FFFFFF;
        box-shadow: 0px 0px 12px rgba(0, 0, 0, 0.12);
        border-radius: 4px;
        margin-bottom: 0.5rem;
    }

    .el-header > h1 {
        font-weight: 400;
        font-size: 1.6rem;
    }

    .el-button {
        font-weight: 300;
        font-size: 16px;
        font-style: italic;
    }

    .el-main {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        background: #FFFFFF;
        box-shadow: 0px 0px 12px rgba(0, 0, 0, 0.12);
        border-radius: 4px;
        gap: 1rem;
    }

    .card {
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: stretch;
        width: 14.1rem;
        height: 14rem;
        box-shadow: 0px 0px 12px rgba(0, 0, 0, 0.12);
        border-radius: 4px;
    }

    .card > * {
        align-self: center;
    }

    .card .wrap-button {
        align-self: start;
        margin-left: 0.5rem;
        margin-bottom: 0.5rem;
    }

    .card > p {
        font-weight: 300;
        margin-bottom: auto;
    }

    .wrap-img{
        margin-top: 1rem;
    }

</style>
