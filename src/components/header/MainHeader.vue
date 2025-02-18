<script setup>
import DropDown from './DropDown.vue'
</script>

<template>
    <header class="section header">
        <div class="container justify-content-between">
            <a href="/"><img class="header-logo" src="\src\assets\icons\logo.svg" alt=""></a>
            <nav class="header-nav">
                <DropDown>
                Tutaj będzie dropdown jak go ogarne
                    
                </DropDown>
                <div class="d-flex flex-row">
                   <div class="d-flex text-white"><span class="mr-5px">iko</span><a class="hover-orange" href="">Login</a></div> 
                    <span class="divider text-white">|</span>
                    <a class="text-white hover-orange" href="">Register</a>
                </div>
                <button class="ml-30px btn btn-or-wh">+ Create event</button>
            </nav>
        </div>
    </header>

</template>

<style scoped>
.header{
    z-index: 10;
    height: 75px;
    align-items: center;
    justify-content: center;

}
.header-logo{
width: 110px;
height: 40px;
}
.header-nav{
    display: flex;
    flex-direction: row;
    align-items: center;

}


</style>