<template>
    <div>
        <full-page :options="options">
            <Banner />
            <div class="main-container">
                <h1>"Monte o seu hamburguer</h1>
                <Burger-form />
            </div>
        </full-page>
    </div>
</template>

<script>
    import Banner from '@/components/Banner.vue'
    import BurgerForm from '@/components/BurgerForm.vue'
    import Full_Page from 'vue-fullpage.vue'

    export default {
        name: 'Home',
        components: {
            Banner,
            BurgerForm
        },
        data() {
            return {
                options: {
                    paddingTop: '30px'
                },
            }
        }
    }
</script>
