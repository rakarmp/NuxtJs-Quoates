<template>
    <div>
  <Navbar />
  <b-container class="mt-4" v-for="kataKata in kataBijak" :key="kataKata.id">
    <b-card :header="kataKata.created">
      <blockquote class="blockquote mb-0">
        <p>{{ kataKata.katanya }}</p>
        <footer class="blockquote-footer">
          {{ kataKata.penulis }} in <cite title="Source Title">Quoates Anjay</cite>
        </footer>
      </blockquote>
    </b-card>
  </b-container>
</div>
</template>

<script>
export default {
    data() {
    return {
      kataBijak: []
    }
  },
  created() {
    this.kataBijak = [
    {
           id: 1,
           noUrut: "1",
           katanya: 'Semakin Lurus Niatnya, Semakin Kencang Cobaannya',
           penulis: 'Mamang@Racing',
           created: '19-10-2022'
         },
         {
           id: 2,
           noUrut: "2",
           katanya: 'Diperbaiki Bukan Diakhiri, Dibicarakan Bukan Ditinggalkan',
           penulis: 'Zidan - EnteKadang2X',
           created: '19-10-2022'
         },
         {
           id: 3,
           noUrut: "3",
           katanya: 'Jadilah Kuat Untuk Semua Hal Yang Membuatmu Patah',
           penulis: 'Djarum - Super`man',
           created: '19-10-2022'
         },
         {
           id: 4,
           noUrut: "4",
           katanya: 'Ada Lelah Yang Ditahan, Karena Ada Harapan Yang Harus Diwujudkan',
           penulis: 'The - Magnum Paralons',
           created: '19-10-2022'
         },
         {
           id: 5,
           noUrut: "5",
           katanya: 'Terwujud Atau Tak Terwujud, Tetaplah Bersujud',
           penulis: 'Samsudin X HoohTenan',
           created: '19-10-2022'
         },
         {
           id: 6,
           noUrut: "6",
           katanya: 'Sedang Meyakinkan Diri Bahwa Semuanya Bisa Dilewatin Sendirian',
           penulis: 'SHarapan Duls',
           created: '20-10-2022'
         },
         {
           id: 7,
           noUrut: "7",
           katanya: 'Kamu Terlalu Mengharapkan Dia, Sedangkan Dia Mengharapkan Orang Lain.',
           penulis: 'VueAnjayXSolorunXNetify',
           created: '20-10-2022'
         },
         {
          id: 8,
          noUrut: '8',
          katanya: 'Stay Strong, Stay Positive, Stay Happy',
          penulis: 'Sipaling Stay',
          created: '23-10-2022',
         },
         {
          id: 9,
          noUrut: '9',
          katanya: 'Stay Private, Belajar Dari Hari - Hari Kemarin, Terlalu Sering Dibanggakan Belum Tentu Tulus.',
          penulis: 'RakaTrust',
          created: '23-10-2022',
         },
         {
          id: 10,
          noUrut: '10',
          katanya: 'Terlalu Percaya, Hingga Lupa Bahwa Manusia Bisa Berubah Kapan Saja',
          penulis: 'AdliaFjaAgustin',
          created: '23-10-2022',
         },
         {
          id: 11,
          noUrut: '11',
          katanya: 'Kamu Bisa Mencintai Orang Lain, Tapi Tidak Bisa Mencintai Diri Sendiri',
          penulis: 'RakaTrust',
          created: '25-10-2022',
         },
         {
          id: 12,
          noUrut: '12',
          katanya: 'Semangat Bukan Untuk Mencari Yang Terbaik, Tapi Untuk Mencari Yang Terbaik Dari Yang Ada',
          penulis: 'Copilot',
          created: '25-10-2022',
         }
    ]
  },
  computed: {
    cariData(){
      return this.kataBijak.filter((kataKata) => {
        return kataKata.noUrut.match(this.cari);
      })
    }
  }
}
</script>

<style>
#card {
  position: absolute;
  top: 50px;
}
</style>
