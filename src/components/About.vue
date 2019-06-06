<template>
    <div class="about">
        <div class="about__container">
            <h2 class="about__headliner">Let's get acquainted</h2>
            <div class="about__content content">
                <div class="content__image-container">
                    <img class="content__image" src="../assets/imgs/man-mobile.svg">
                </div>
                <div class="content__text">
                    <h3 class="content__headliner">I am cool frontend developer</h3>
                    <p class="content__paragraph">
                        When real users have a slow experience on mobile, they're much less 
                        likely to find what they are looking for or purchase from you in the 
                        future. For many sites this equates to a huge missed opportunity, 
                        especially when more than half of visits are abandoned if a mobile page 
                        takes over 3 seconds to load.
                    </p>
                    <p class="content__paragraph">
                        Last week, Google Search and Ads teams announced two new speed initiatives 
                        to help improve user-experience on the web. 
                    </p>
                    <a href="#" class="content__link">Sign Up</a>
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
    @import '../scss/style';
</style>