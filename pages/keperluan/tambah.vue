<template> 
    <div class="container-fluid"> 
      <div class="row"> 
        <div class="col-lg-12"> 
          <h2 class="text-center my-4">Keperluan Kas PPLG 4</h2>
          <form @submit.prevent="kirimData">
            <div class="row d-flex justify-content-center">
            <div class="mb-3 col-lg-6"> 
                  <select v-model="form.nama" class="form-control form-control-lg form-select rounded-3 mb-2"> 
                    <option value="">Nama...</option>
                    <option value="Agistina">Agistina</option>
                    <option value="Agni Anjelita">Agni</option>
                    <option value="Ardiansyah Maulana">Ardiansyah Maulana</option>
                    <option value="Ega Suzana">Ega Suzana</option>
                    <option value="Erina Nazwa S">Erina Nazwa S</option>
                    <option value="Gilang Ardiansyah">Gilang Ardiansyah</option>
                    <option value="Husni Hadiani R">Husni Hadiani R</option>
                    <option value="Ilham Septihadi">Ilham Septihadi</option>
                    <option value="Irgi Cahya">Irgi Cahya</option>
                    <option value="Jian Kamil">Jian Kamil</option>
                    <option value="Melani Siti N">Melani Siti N</option>
                    <option value="Muhammad Riqi">Muhammad Riqi</option>
                    <option value="Neng Wafi N">Neng Wafi N</option>
                    <option value="Rafi Ahmad A">Rafi Ahmad A</option>
                    <option value="Raras Ramadhani">Raras Ramadhani</option>
                    <option value="Resti Oktaviani">Resti Oktaviani</option>
                    <option value="Risti Nur A">Risti Nur A</option>
                    <option value="Rizni Razbia">Rizni Rajbia</option>
                    <option value="Sani Sahrul M">Sani Sahrul M</option>
                    <option value="Tiara Andriyani">Tiara Andriyani</option>
                    <option value="Wijdan Fathu R">Wijdan Fathu R</option>
                    <option value="Wulan Maulina">Wulan Maulina</option>
                    <option value="Wulan Tri A">Wulan Tri a</option>
                    <option value="Zaskia Nurul H">Zaskia Nurul H</option>
                    <option value="Ziankha Islamiranda">Ziankha Islamiranda</option>
                    <option value="Zulpa Agustin">Zulpa Agustin</option>
                  </select> 
                </div>
              </div>
              <div class="row d-flex justify-content-center">
                <div class="mb-3 col-lg-6 ">
                  <input type="date" class="form-control form-control-lg form-select rounded-3 mb-2" placeholder="Tanggal">
                </div>
              </div>
              <div class="row d-flex justify-content-center">
                <div class="mb-3 col-lg-6 d-flex justify-content-center">
                  <select name="" id="" class="form-control form-control-lg form-select rounded-3 mb-2">
                    <option value="">Keperluan</option>
                    <option value="Membayar Uang Kas">Membayar Uang Kas</option>
                    <option value="Pengeluaran">Pengeluaran</option>
                    <option value="Pemasukan">Pemasukan</option>
                  </select>
                </div>
              </div>
              <div class="row d-flex justify-content-center">
                <div class="mb-3 col-lg-6">
                  <input type="text" class="form-control form-control-lg form-select rounded-3 mb-2" placeholder="Nominal Bayar:">
                </div>
                </div>
          </form>
        </div>
      </div>
      <nuxt-link to="/keperluan">
      <button type="submit" class="btn btn-success btn-lg rounded-3 px-3"> Kirim </button>
      </nuxt-link>
    </div>
    </template>
  
    
    <style scoped>
    
    .btn-success{
      background-color: #000000;
    }
    input{
      background: #D9D9D9;
    }
    select{
      background: #D9D9D9;
    }
    </style>
    
    <script setup>
    const supabase = useSupabaseClient()
    
    const members = ref([])
    
    const objectives = ref([])
    
    const form = ref ({
    nama: "",
    Waktu: "",
    Keperluan: "",
    })
    
    </script>