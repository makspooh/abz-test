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
                    <img class="form__img-phone" src="../assets/icons/phone.png">
                    <img class="form__img-email" src="../assets/icons/email.png">
                    <img class="form__img-name" src="../assets/icons/name.png">
                    <input type="text" class="form__name" placeholder="Your name">
                    <input type="text" class="form__email" placeholder="Your email">
                    <input type="text" class="form__phone" placeholder="+38 (___)  ___ __ __">
                </div>
                <div class="form__secondline">
                    <select class="form__position" name="position">
                        <option disabled selected>Select your position</option>
                        <option>Admin</option>
                        <option>User</option>
                        <option>Guest</option>
                    </select>
                    <input @change="setFileName()" class="form__file" type="file" name="file" id="file">
                    <div class="form__upload-block">
                        <div class="form__input-block">
                            <div class="form__filename">
                                <p id="filename" class="form__paragraph">Upload your photo</p>
                            </div>
                            <label class="form__label" for="file">Upload</label>
                        </div>
                        <pre><p class="form__file-description">File format jpg  up to 5 MB, the minimum size of 70x70px</p></pre>
                    </div>
                </div>
                <button class="form__submit" type="submit">Sign Up</button>
            </form>
        </div>
    </div>
</template>

<script>
    export default {
        data: () => {
            return {}
        },
        methods: {
            setFileName() {
                let file = document.getElementById('file').value.toString();
                let fileName = document.getElementById('filename');
                let newFileName = file.split('\\');
                fileName.textContent = newFileName[newFileName.length - 1];
            }
        }
    }
</script>

<style lang="scss">
    @import '../scss/style';
</style>