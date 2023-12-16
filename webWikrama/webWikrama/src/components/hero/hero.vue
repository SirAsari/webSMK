<template>
    <div class="hero-container">
        <div class="hero-content">
            <div class="hero-box hero-box-1">1</div>
            <div class="hero-box hero-box-2">2</div>
            <div class="hero-box hero-box-3">3</div>
            <div class="hero-box hero-box-4">4</div>
            <div class="hero-box hero-box-5">5</div>
            <!-- <div class="hero-box hero-box-6">6</div> -->
        </div>
    </div>
</template>

<script>
export default {
    name: 'Hero',
}
</script>

<style scoped>
.hero-content {
    display: grid;  
    
}
.hero-box-1 {
    
}


.hero-box {
    font-size: 40px;
    padding: 10px;
}
.hero-box-1 {
    background-color: #70e9c9;
}
.hero-box-2 {
    background-color: #63dbbb;
}
.hero-box-3 {
    background-color: #51c9a9;
}
.hero-box-4 {
    background-color: #3dafa0;
}
.hero-box-5 {
    background-color: #309d96;
}
.hero-box-6 {
    background-color: #1e897a;
}
</style>