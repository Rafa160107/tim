<script setup>
import { onMounted } from 'vue';
import modal from '../components/modal.vue'
let myModal;
onMounted(()=>{
  myModal = new bootstrap.Modal(document.getElementById("alert"))
})
const popupShow = ()=>{
  myModal.show();
}
</script>
<template>
<button @click="popupShow">tampil modal</button>
<modal title="hello">ini adalah konten modal</modal>
</template>