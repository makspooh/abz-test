<template>
    <footer class="footer">
        <div class="footer__container">
            <div class="footer__toolbar">
                <img src="../assets/logo/logo.png" class="footer__logo">
                <nav class="footer__nav">
                    <a v-for="link of toolbar" :key="link" href="#" class="footer__toolbar-link">{{ link }}</a>
                </nav>
            </div>
            <div class="footer__other">
                <div class="footer__content">
                    <div class="footer__contacts">
                        <div class="footer__contact-block">
                            <img src="../assets/icons/mail.svg" alt="" class="footer__contact-img">
                            <p class="footer__contact-text footer__email">work.of.future@gmail.com</p>
                        </div>
                        <div class="footer__contact-block">
                            <img src="../assets/icons/phone.svg" alt="" class="footer__contact-img">
                            <p class="footer__contact-text footer__phone1">+38 (050) 789 24 98</p>
                        </div>
                        <div class="footer__contact-block">
                            <img src="../assets/icons/cellphone.svg" alt="" class="footer__contact-img">
                            <p class="footer__contact-text footer__phone2">+38 (095) 556 08 45</p>
                        </div>
                    </div>
                    <div class="footer__links">
                        <div class="footer__column">
                            <a href="#" class="footer__link">News</a>
                            <a href="#" class="footer__link">Blog</a>
                            <a href="#" class="footer__link">Partners</a>
                            <a href="#" class="footer__link">Shop</a>
                        </div>
                        <div class="footer__column">
                            <a href="#" class="footer__link">Overview</a>
                            <a href="#" class="footer__link">Design</a>
                            <a href="#" class="footer__link">Code</a>
                            <a href="#" class="footer__link">Collaborate</a>
                        </div>
                        <div class="footer__column">
                            <a href="#" class="footer__link">Tutorials</a>
                            <a href="#" class="footer__link">Resources</a>
                            <a href="#" class="footer__link">Guides</a>
                            <a href="#" class="footer__link">Examples</a>
                        </div>
                        <div class="footer__column">
                            <a href="#" class="footer__link">FAQ</a>
                            <a href="#" class="footer__link">Terms</a>
                            <a href="#" class="footer__link">Conditions</a>
                            <a href="#" class="footer__link">Help</a>
                        </div>
                    </div>
                </div>
                <div class="footer__social">
                    <p class="footer__copyright">&copy; abz.agency specially for the test task</p>
                    <div class="footer__icons">
                        <img src="../assets/icons/facebook.svg" alt="" class="footer__icon">
                        <img src="../assets/icons/linkedin.svg" alt="" class="footer__icon">
                        <img src="../assets/icons/instagram.svg" alt="" class="footer__icon">
                        <img src="../assets/icons/twitter.svg" alt="" class="footer__icon">
                        <img src="../assets/icons/pinterest.svg" alt="" class="footer__icon">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    data: () => {
        return {
            toolbar: [
                'About me',
                'Relationships',
                'Requirements',
                'Users',
                'Sign Up'
            ]
        }
    }
}
</script>

<style lang="scss">
    @import '../scss/style';
</style>
