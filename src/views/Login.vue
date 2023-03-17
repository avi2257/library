<template>
    <div class="center">
        <v-row>
            <v-col cols="10" offset="1">
                <v-avatar color="primary" size="56" tile>
                    <v-img src="@/assets/logo.png"></v-img>
                </v-avatar>
                <v-text-field label="Username" v-model="username"></v-text-field>
                <v-text-field label="password" type="password" v-model="password"></v-text-field>
                <v-btn class="base-inverted" block @click="authenticate()">Login</v-btn>
            </v-col>
        </v-row>
        <h1>Login page</h1>

    </div>
</template>

<script>
export default {
    data() {
        return {    
            username: '',
            password: ''
        }
    },
    methods: {
        authenticate() {
            alert("Login")
            console.log(this.username, this.password)
        }
    }
}
</script>
    
<style lang="scss" scoped></style>