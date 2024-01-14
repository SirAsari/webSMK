<template>
    <div class="footer-container">
        <div class="footer-row-1">
            <div class="top">
                <h4 class="footer-title">Alamat</h4>
                <p>Jl. Raya Wangun Kelurahan<br> Sindangsari Bogor Timur 16720</p>
            </div>
            <div class="bottom">
                <h4 class="footer-title">Telepon</h4>
                <p>0251-8242411 / 082221718035</p>
            </div>
        </div>
        <!-- This one is like a hr but vertical -->
        <div class="footer-row-2"></div>
        <div class="footer-row-3">
            <h5 class="footer-title-first">Tentang Wikrama</h5>
            <ol>
                <li>Sejarah</li>
                <li>Peraturan Sekolah</li>
                <li>Pencapaian</li>
                <li>Kerjasama</li>
            </ol>
        </div>
        <div class="footer-row-4">
            <h5 class="footer-title">Layanan</h5>
            <ol>
                <li>FAQ</li>
                <li>Pembelajaran</li>
                <li>PPDB</li>
                <li>Hubungi Kami</li>
            </ol>
        </div>
        <div class="footer-row-5">
            <h5 class="footer-title">Cabang</h5>
            <ol>
                <li>Wikrama Garut</li>
                <li>Wikrama Jepara</li>
                <li>Wikrama Bekasi</li>
                <li>Wikrama Semarang</li>
            </ol>
        </div>
    </div>
</template>

<style scoped>
* {
    margin: 0;
    padding: 0;
}

.footer-container {
    padding-top: 2.3rem;
    padding-bottom: 2.3rem;
    background: #2D928C;
    margin-top: 30rem;
    display: flex;
    justify-content: center;
}

.footer-row-2 {
    width: 2.3px;
    height: 160px;
    background: #277B76;
}

.footer-row-3 {
    margin-left: 4rem;
}
.footer-title {
    color: #FFF;

font-family: Poppins;
font-size: 18px;
font-style: normal;
font-weight: 600;
line-height: normal;
}

h5.footer-title-first {
    margin-bottom: 18px;
    margin-right: 42px;
    color: #FFF;

font-family: Poppins;
font-size: 18px;
font-style: normal;
font-weight: 600;
line-height: normal;
}
h5.footer-title {
    margin-bottom: 18px;
    padding-right: 65px;
}

li {
    list-style-type: none;
    color: #FFF;
    font-family: 'Poppins';
    font-weight: lighter;
    opacity: 0.7;
    margin-bottom: 4px;
}

.footer-row-1 {
    padding-right: 2.7rem;
}
.top h4 {
    margin-bottom: 8px;
}
.top p, .bottom p {
    color: #FFF;

font-family: Poppins;
font-size: 16px;
font-style: normal;
font-weight: 400;
line-height: normal;
text-decoration-line: underline;
}
.bottom h4 {
    margin-top: 16px;
}
</style>