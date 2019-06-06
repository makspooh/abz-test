<template>
    <div class="users">
        <div class="users__container">
            <h2 class="users__headliner">Our cheerful users</h2>
            <h4 class="users__headliner4">Attention! Sorting users by registration date</h4>
            <div class="users__content">
                <div v-for="(user, index) of users" :key="index" class="users__user">
                    <img class="users__avatar" :src='user.image'>
                    <div class="users__text">
                        <h2 class="users__headliner2">{{ user.name }}</h2>
                        <p class="users__position">{{ user.position }}</p>
                        <p class="users__email">{{ user.email }}</p>
                        <p class="users__phone">{{ user.phone }}</p>
                    </div>
                </div>
                <div class="users__button-container">
                    <button class="users__button">Show more</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: () => {
        return {
            users: [
                {
                    name: 'Noah',
                    position: 'Leading specialist of the Control Department',
                    email: 'noah.controldepartment@gmail.com',
                    phone: '+38 (050) 678 03 24',
                    image: require ('../assets/imgs/user-noah-2x.jpg')
                },
                {
                    name: 'Adolph Blaine Charles David Earl',
                    position: 'The contextual advertising specialist',
                    email: 'adolph.blainecharles-davidearl@...',
                    phone: '+38 (095) 556 08 45',
                    image: require ('../assets/imgs/user-adolph-2x.png')
                },
                {
                    name: 'Liamgrievescasey Smith Wiam',
                    position: 'Lead designer',
                    email: 'liamgrievescasey@example.com',
                    phone: '+38 (050) 273 93 32',
                    image: require ('../assets/imgs/user-liam-2x.jpg')
                },
                {
                    name: 'Elizabeth',
                    position: 'Frontend developer',
                    email: 'elisabet.frontend@gmail.com',
                    phone: '+38 (095) 924 66 37',
                    image: require ('../assets/imgs/user-elizabeth-2x.jpg')
                },
                {
                    name: 'Alexander',
                    position: 'Backend developer',
                    email: 'alexander.backend@gmail.com',
                    phone: '+38 (050) 789 24 09',
                    image: require ('../assets/imgs/user-alexander-2x.jpg')
                },
                {
                    name: 'Mason',
                    position: 'QA',
                    email: 'mason.qa@gmail.com',
                    phone: '+38 (095) 283 27 00',
                    image: require ('../assets/imgs/user-mason-2x.jpg')
                },
            ]
        }
    }
}
</script>

<style lang="scss">
    @import '../scss/style';
</style>