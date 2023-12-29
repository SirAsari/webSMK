<script>
export default {
    name: 'Section1',
}
</script>

<template>
    <div class="section1-container">
        <h3>Sukses Bersama SMK Wikrama Bogor</h3>
        <p>Sejak 1996, Wikrama turut serta dalam membina masa depan bangsa dengan mendidik generasi muda Indonesia.</p>
        <div class="text-flex">
            <div class="visi-text">
                <div class="title">
                    <h5>Visi</h5>
                    <hr>
                </div>
                <p>Sejak 1996, Wikrama turut serta dalam membina masa depan bangsa dengan mendidik generasi muda Indonesia.</p>
            </div>
            <div class="misi-text">
                <div class="title">
                    <h5>Misi</h5>
                    <hr>  
                </div>
                <p>Sejak 1996, Wikrama turut serta dalam membina masa depan bangsa dengan mendidik generasi muda Indonesia.</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
.section1-container {
    margin-top: 5rem;
    padding: 42px 126px 0px 126px;
    background-color: #EEF1F7;
    position: absolute;
    left: 0;
    right: 0;
    overflow: hidden;
}

.section1-container h3 {
    color: #213866;
    font-size: 30px;
    font-style: normal;
    font-family: 'Poppins', sans-serif;
    font-weight: 600;
    line-height: 39px;
    width: 372px;
}

.section1-container p {
    margin: 16px 0 24px 0;
    width: 660px;
    font-size: 20px;
    color: rgba(33, 56, 102, 0.80);
}

.text-flex {
    display: flex;
}

.title {
    display: flex;
}

.visi-text hr, .misi-text hr {
    margin-top: 13px;
    margin-left: 12px;
    width: 500px;
}
.visi-text h5 { 
    font-family: 'Poppins';
    font-weight: 500;
}

</style>