<script setup lang="ts">
import {ref, onMounted, watch} from 'vue'

const jumlah = ref(1)
const disabledTambah = ref(false)
const disabledKurang = ref(false)

function tambah() {
  jumlah.value++
}

function kurang() {
  jumlah.value--
}

onMounted(() => {
  console.log('Ini pemanis aja'); // karena belum tau jalaninnya kek mana
})

watch(jumlah, () => {
  if (jumlah.value <= 0){
    disabledKurang.value = true
  } else if (jumlah.value >= 10) {
    disabledTambah.value = true
  }
  else {
    disabledTambah.value = false
    disabledKurang.value = false
  }
})
</script>

<template>
<title>alkdjkleajdlkajwedlkajwed</title>
  <button @click="tambah" :disabled="disabledTambah">tambahin</button>
  <br>
  {{ jumlah }}
  <br>
  <button @click="kurang" :disabled="disabledKurang">kurangin</button>
</template>