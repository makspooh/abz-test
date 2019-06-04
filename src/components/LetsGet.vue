<template>
    <div class="letsget">
        <div class="letsget__container">
            <h2 class="letsget__headliner">Let's get acquainted</h2>
            <div class="letsget__content content">
                <img src="../assets/imgs/man-mobile.svg">
                <div class="content__text">
                    <h3 class="content__headliner">I am cool frontend developer</h3>
                </div>
            </div>
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
    @import 'https://fonts.googleapis.com/css?family=Overpass:100,400,600&display=swap';

    .letsget {
        display: flex;
        justify-content: center;

        &__container {
            width: 930px;
        }

        &__headliner {
            font-family: 'Overpass', sans-serif;
            font-size: 41px;
            text-align: center;
            padding-top: 132px;
        }
    }

    .content {
        display: flex;

        &__headliner {
            font-family: 'Overpass', sans-serif;
            text-align: center;
        }
    }
</style>