<template>
    <div class="signup">
        <div class="signup__container">
            <h2 class="signup__headliner">Register to get a work</h2>
            <h4 class="signup__headliner4">
                Attention! After successful registration and alert, update 
                the list of users in the block from the top
            </h4>
            <form class="signup__form form" action="" method="get">
                <div class="form__first-line">
                    <input type="text" class="form__name" placeholder="Your name">
                    <input type="text" class="form__email" placeholder="Your email">
                    <input type="text" class="form__phone" placeholder="+38 (___)  ___ __ __">
                </div>
                <div class="form__secondline">
                </div>
            </form>
        </div>
    </div>
</template>

<script>
export default {
    data: () => {
        return {}
    }
}
</script>

<style lang="scss">
    @import '../scss/style';
</style>