<template>
    <div :class="[btnClass]">
        <slot/>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                btnClass:'btn'
            }
        }
    }
</script>

<style lang="scss">
@import '../../css/element.scss';
.btn{
    @include btn;
}
</style>