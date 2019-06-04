<template>
    <div class="signup">
        <div class="signup__container">
            <div class="signup__text text">
                <div class="text__headliner headliner">
                    <h1 class="headliner__text">Test assignment for Frontend Developer position</h1>
                </div>
                <div class="text__paragraph paragraph"></div>
                <p class="paragraph__text">
                    We kindly remind you that your test assignment should be submitted as a link 
                    to github/bitbucket repository. Please be patient, we consider and respond 
                    to every application that meets minimum requirements. We look forward to your 
                    submission. Good luck!
                </p>
                <div class="text__button button">
                    <button class="button__button">Sign Up</button>
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
    @import 'https://fonts.googleapis.com/css?family=Source+Sans+Pro:200,200i,300,300i,400,400i,600,600i,700,700i,900,900i&display=swap';
    @import 'https://fonts.googleapis.com/css?family=Overpass:100,400,600&display=swap';

    $mainOrangeColor: #ef6c00;

    @mixin displayFlexCenter() {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    @mixin fontStyles() {
        color: white;
        font-family: 'Overpass', sans-serif;
    }

    .signup {
        position: relative;
        z-index: 1;
        top: 65px;
        margin-bottom: 65px;
        height: 725px;
        background-image: url('../assets/imgs/bg-1.jpg');
        background-size: cover;
        @include displayFlexCenter();

        &__container {
            width: 930px;
        }

    }

    .text {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: flex-start;
        height: 460px;
    }

    .headliner {

        &__text {
            @include fontStyles();
            font-size: 50px;
            font-weight: 600;
            width: 450px;
            line-height: 1.2;
        }
    }

    .paragraph {
        margin-top: -35px;

        &__text {
            font-family: 'Source Sans Pro', sans-serif;
            font-size: 20px;
            font-weight: 400;
            color: white;
            width: 430px;
            line-height: 1.3;
            margin-block-start: 0;
        }
    }

    .button {
        padding-bottom: 25px;

        &__button {
            font-family: 'Source Sans Pro', sans-serif;
            font-size: 20px;
            font-weight: 600;
            width: 290px;
            height: 40px;
            background-color: $mainOrangeColor;
            color: white;
            border-radius: 5px;
        }
    }

</style>
