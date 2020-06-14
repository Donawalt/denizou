<template>
    <header>
        <img src='~assets/images/logo.png' class='logo'>
        <ul>
            <li><nuxt-link to="">prestations</nuxt-link></li>
            <li><nuxt-link to="">réalisations</nuxt-link></li>
            <li><nuxt-link to="">contact</nuxt-link></li>
        </ul>
    </header>
</template>

<style lang="scss" scoped>
    header{
        z-index: 1000;
        background-color: #232424;
        height: 60px;
        padding-top: 24px;
        padding-bottom: 24px;
        display: flex;
        justify-content: space-between;
        width: 100vw;
        position: fixed;
        top:0;
        left: 0;
        .logo{
            height: 100%;
            width: auto;
            margin-left: 11.25vw;
        }
        ul {
            margin-right: 11.25vw;
            display: flex;
            li{
                margin-left: 16px;
                list-style: none;
                a{
                    color: white;
                    text-decoration: none;
                    font-size: 16px;
                    font-family: Arial, Helvetica, sans-serif;
                    font-weight: lighter;
                }
            }
        }
    }
</style>