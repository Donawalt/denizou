<template>
    <div>
        <p>Contactez nous au <a href='tel:0478844471'>04 78 84 44 71</a></p>
    </div>
</template>

<style lang="scss" scoped>
    div{
        height: 25vh;
        margin-left: 11.25vw;
        margin-right: 11.25vw;
        p{
            font-size: 100px;
            font-family: Arial, Helvetica, sans-serif;
            text-transform: uppercase;
            color: transparent;
            font-weight: bold;
            -webkit-text-stroke-color: white;
            -webkit-text-stroke-width: 4px;
            a{
                text-decoration: none;
                color: #FFAFAF;
                -webkit-text-stroke-color: white;
                -webkit-text-stroke-width: 0px;
                &:hover{
                    color:#046BD9;
                    transition: 300ms;
                }
            }
        }
    }
</style>