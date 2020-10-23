<template>
    <el-row>
        <el-col :span="24">
             <el-card shadow="always">
                 彩券
                 <i class="el-icon-video-pause" @click="jy" width="50px"></i>
                 <audio v-if="muted"
                         src="http://m801.music.126.net/20201023171257/3333518f2f6f0fd3c2b6400a5e665e9d/jdymusic/obj/wo3DlMOGwrbDjj7DisKw/4387351108/698b/39d2/91d9/dabe5d3eb8e4efaeeb43dcfc72c70f52.mp3" autoplay="autoplay"></audio>
            </el-card>
            <el-card class="box-card" >
                <el-carousel indicator-position="outside" height="200px">
                    <el-carousel-item>
                        <img src="../img/2.jpg" width="100%" height="100%">
                    </el-carousel-item>
                    <el-carousel-item>
                        <img src="../img/1.jpg" width="100%" height="100%">
                    </el-carousel-item>
                </el-carousel>
            </el-card>
        </el-col>
    </el-row>


</template>

<script>
    export default {
        name: 'HelloWorld',
        data() {
            return {
                show: true,
                muted: false
            }
        },
        created() {
            // this.getData();
        },
        methods: {
            getData() {
                this.show = !this.show
            },
            jy(){
                console.log(this.muted)
                this.muted = !this.muted
            }
        }
    }
</script>

<style scoped>

</style>
