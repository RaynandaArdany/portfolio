<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
import { ref } from 'vue'
import { TheCard } from 'flowbite-vue'
const activeTab = ref('first')
import { Carousel } from 'flowbite-vue'
import { Timeline, TimelineItem, TimelinePoint, TimelineTime, TimelineContent, TimelineTitle } from 'flowbite-vue'
import { Footer } from 'flowbite-vue'
import { Progress } from 'flowbite-vue'
import { ListGroup, ListGroupItem } from 'flowbite-vue'
const pictures = [
  {
    'src': '/img/HD.jpeg',
    'alt': 'Picture 1',
  },
  {
    'src': '/img/one.jpeg',
    'alt': 'Picture 2',
  },
  {
    'src': '/img/kapal.jpeg',
    'alt': 'Picture 3',
  },
]


</script>


<template>
    <Navbar>
      <template #logo>
        <NavbarLogo link="#" alt="Flowbite logo" image-url="/img/zoro.png">
          TheExplorer
        </NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink is-active>Beranda</NavbarLink>
          <NavbarLink>Tentang</NavbarLink>
          <NavbarLink>Kontak</NavbarLink>
        </NavbarCollapse>
      </template>
      <template #menu-icon>
        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4"></path></svg>
      </template>
    </Navbar>

    <Carousel :pictures="pictures"></Carousel>

    <hr>

  <div style="margin: 25px;" class="flex">
<the-card class="mr-20" variant="image" img-src="/img/7d4d39f5-5643-4273-9ac5-2dced1d071ff.jpeg" img-alt="Desk">
<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">BioData</h5>
<h5 class="font-normal text-gray-700 dark:text-gray-400">
  NAMA   : RIAN JUAN RAYNANDA A
  <br>
  ALAMAT : Kp.Cilisung Rt04 Rw05
  <br>
  TANGGAL LAHIR : 13/05/2006
  <br>
  JENIS KELAMIN : Laki-laki
  <br>
  AGAMA : Islam

</h5>
</the-card>


<the-card class="mr-20" variant="image" img-src="/img/Saya.jpeg" img-alt="Desk">
<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Tentang</h5>
<p class="font-normal text-gray-700 dark:text-gray-400">
  Rian adalah Pemburu E-Rank yang terkenal lemah, dia mendapat kesempatan seumur hidup ketika dia terpilih sebagai Pemain Sistem , memperoleh kemampuan unik untuk tumbuh dalam kekuatan tanpa hambatan. Akibatnya, dengan memanfaatkan peluang yang ditawarkan oleh Sistem, Rian akhirnya naik ke tampuk kekuatan sebagai pemburu terhebat umat manusia dan Raja Bayangan kedua.
</p>
</the-card>

<Timeline>
    <timeline-item>
      <timeline-point>
      </timeline-point>
      <timeline-content>
        <timeline-time>
          
        </timeline-time>
        <timeline-title>
          Hobi
        </timeline-title>
        <timeline-body>
          Hobi Saya Bermain Game, Membaca Komik, dan Ngoding
        </timeline-body>
      </timeline-content>
    </timeline-item>
    <timeline-item>
      <timeline-point>
      </timeline-point>
      <timeline-content>
        <timeline-time>
          
        </timeline-time>
        <timeline-title>
        Cita-cita
        </timeline-title>
        <timeline-body>
          Cita-tata Saya Menjadi Konten Creator
        </timeline-body>
      </timeline-content>
    </timeline-item>
    <timeline-item>
      <timeline-point>
      </timeline-point>
      <timeline-content>
        <timeline-time>
          
        </timeline-time>
        <timeline-title>
          Kata-kata
        </timeline-title>
        <timeline-body>
          Bahkan orang tanpa bakat pun Suatu hari nanti pasti berguna.
        </timeline-body>
      </timeline-content>
    </timeline-item>
  </Timeline>

</div>

<hr>

<div style="margin: 50px;" class="flex">
<Timeline>
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time>
          Mei 2006
        </timeline-time>
        <timeline-title>
          Kelahiran
        </timeline-title>
        <timeline-body>
          lahir Bandung Dibesarkan Di Bandung Dan Ingin 
          <br>
          Kerja Di luar Negeri asik.
        </timeline-body>
      </timeline-content>
    </timeline-item>
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time>
         2007
        </timeline-time>
        <timeline-title>
          Pendidikan
        </timeline-title>
        <timeline-body>
          Jenjang Pendidikan PAUD Sangat amat seru Bisa belajar Sedikit 
        </timeline-body>
      </timeline-content>
    </timeline-item>
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time>
          2017
        </timeline-time>
        <timeline-title>
          Awal Mula SMP
        </timeline-title>
        <timeline-body>
          SMP saya di Yudhistira Jarak Dari Rumah Sampai SMP Lumayan Jauh
        </timeline-body>
      </timeline-content>
    </timeline-item>
  </Timeline>

  <Timeline>
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time>
          2020
        </timeline-time>
        <timeline-title>
          Awal Mula SMK
        </timeline-title>
        <timeline-body>
          SMK saya Di Assalaam Jarak Dengan rumah juga tidak terlalu jauh
        </timeline-body>
      </timeline-content>
    </timeline-item>
    <timeline-item>
      <timeline-point>
        <svg aria-hidden="true" class="w-3 h-3 text-blue-600 dark:text-blue-400" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M6 2a1 1 0 00-1 1v1H4a2 2 0 00-2 2v10a2 2 0 002 2h12a2 2 0 002-2V6a2 2 0 00-2-2h-1V3a1 1 0 10-2 0v1H7V3a1 1 0 00-1-1zm0 5a1 1 0 000 2h8a1 1 0 100-2H6z" clip-rule="evenodd"></path></svg>
      </timeline-point>
      <timeline-content>
        <timeline-time>
        2024
        </timeline-time>
        <timeline-title>
          Melanjutkan Dimana?
        </timeline-title>
        <timeline-body>
          Selanjutny Saya Antara Memilih Kuliah Atau Memilih Langsung Kerja
        </timeline-body>
      </timeline-content>
    </timeline-item>
  </Timeline>
</div>

<hr>

<div style="margin: 25px;">
  <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Keterampilan</h5>
  <Progress labelProgress="true" labelPosition="outside" label="HTML" progress="50"></Progress>
  <Progress labelProgress="true" labelPosition="outside" label="CSS" progress="50"></Progress>
  <Progress labelProgress="true" labelPosition="outside" label="JAVASCRIPT" progress="50"></Progress>
  <Progress labelProgress="true" labelPosition="outside" label="VUE.JS" progress="50"></Progress>
  <Progress labelProgress="true" labelPosition="outside" label="UI/UX" progress="50"></Progress>
</div>

<hr>

<hr>
</template>
