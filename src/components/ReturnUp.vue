<template>
    <div class="box">
        <div>
            <i class="fas fa-angle-up"></i>
        </div>
        <div class="txt-base">
            UP
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
.box{
    padding: 14px;
    text-align: center;
    width: 70px;
    height: 70px;
    background-color: $main-blue;
    position: fixed;
    right:0;
    bottom:0;
    color: white;
}

</style>