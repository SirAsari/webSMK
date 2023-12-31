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
                <ul>
                    <li>Menjadi sekolah kejuruan teladan nasional yang berbudaya lingkungan</li>
                    <li>berkarakter sesuai profil pelajar pancasila</li>
                    <li>berbasil teknologi informasi dan mampu memenuhi kebutuhan nidustri 4.0</li>
                </ul>
            </div>
            <div class="misi-text">
                <div class="title">
                    <h5>Misi</h5>
                    <hr>  
                </div>
                <ul>
                    <li>Mewujudkan sekolah sebagai benteng moralitas bangsa</li>
                    <li>Mendidik anak bangsa dengan hati dan teknologi sehingga memenuhi kebutuhan mutu dunia kerja.</li>
                    <li>Membangun kebersamaan sosial, jiwa kewirausahaanm dan gerakan cinta tanah air dan lingkungan.</li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scoped>
.section1-container {
    margin-top: 5rem;
    padding: 42px 126px 38px 126px;
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
    line-height: 42px;
    width: 372px;
    padding-bottom: 5px;
    letter-spacing: auto;
}

.section1-container p {
    margin: 16px 0 24px 0;
    width: 660px;
    font-size: 20px;
    color: rgba(33, 56, 102, 0.80);
}

.text-flex {
    display: flex;
    justify-content:space-between;
}

.title {
    display: flex;
    margin-top: 4px;
}

.visi-text hr, .misi-text hr {
    margin-top: 13px;
    margin-left: 12px;
    width: 500px;
}
.visi-text h5, .misi-text h5{ 
    font-family: 'Poppins';
    font-weight: 500;
}

.visi-text ul, .misi-text ul {
    width: 500px;
    font-family: 'Raleway', sans-serif;
}

.misi-text {
    margin-right: 30px;
}

.visi-text ul, .misi-text ul {
    color: rgba(33, 56, 102, 0.80);
    font-size: 18px;
    padding-top: 16px;
    line-height: 32px;
    font-family: 'Raleway';
}

</style>