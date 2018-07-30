<template>
    <div>
        <title>宮崎市民活動センター</title>
        <div v-if="isAdmin">
            <admin-panel></admin-panel>
        </div>
    </div>
</template>


<script>
    export default {
        components: {
            'admin-panel': require('./layouts/AdminPanel'),
        },
        data: function () {
            return {}
        },
        computed: {
            authenticated: function () {
                return this.$store.getters.isAuthenticated
            },
            
        },
        
        
        created() {
            //console.log( this.$store.state.user)
            //window.location.reload(true)
            //this.$router.go(this.$router.currentRoute)
            //console.log('token', localStorage.getItem('token'))

            // let recaptchaScript = document.createElement('script')
            // recaptchaScript.setAttribute('src', 'https://unpkg.com/nprogress@0.2.0/nprogress.js')
            // document.head.appendChild(recaptchaScript)

            
        }
    }
</script>