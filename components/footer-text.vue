<template>
    <div class="space-row">
        <span>{{ contect }}</span>
        <div class="link-space">
            <a :href="link"><span>Baca selanjutnya</span></a>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        contect: String,
        test: String,
        link: String,
    },
    data() {
        return {
            text: 'Selamat datang di situs Sukabet situs dermainan online terlenakap dan terpercava. Pada halaman in anda dapat memilih kategori permainan vang anda inqin mainkan saat In. Bag andd yang Delum au, Dartar Can dapatkan DOnus pemain Daru di SituS Kami. Rasakan keservan yang relan dirasakan oleh pemain lainnya., Jangan ketingqalan permainan terbaru yanq seru di situs kami, Kami hanya memiliki permainan-permainan terbaik agar anda tidak binqund',
        }
    },
}
</script>