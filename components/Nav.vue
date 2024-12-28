<template>
   <div class="navbar bg-base-100">
  <div class="flex-none relative left-[900px]">
    <ul class="menu menu-horizontal px-1">
      <li>
        <details>
          <summary>Profil</summary>
          <ul class="bg-base-100 rounded-t-none p-2">
            <li><a>Identitas Sekolah</a></li>
            <li><a>Sejarah</a></li>
            <li><a>Visi & Misi</a></li>
            <li><a>Kepala Sekolah</a></li>
            <li><a>Struktur Organisasi</a></li>
            <li> <NuxtLink to="/guru"><a>Guru & Staf</a> </NuxtLink></li>
          </ul>
        </details>
      </li>
      <li>
        <details>
          <summary>Konsentrasi Keahlian</summary>
          <ul class="bg-base-100 rounded-t-none p-2">
            <li><a>Link 1</a></li>
            <li><a>Link 2</a></li>
          </ul>
        </details>
      </li>
      <li>
        <details>
          <summary>Ekstrakulikuler</summary>
          <ul class="bg-base-100 rounded-t-none p-2">
            <li><a>Link 1</a></li>
            <li><a>Link 2</a></li>
          </ul>
        </details>
      </li>
      <li>
        <details>
          <summary>Sapras</summary>
          <ul class="bg-base-100 rounded-t-none p-2">
            <li><a>Link 1</a></li>
            <li><a>Link 2</a></li>
          </ul>
        </details>
      </li>
      <li>
        <details>
          <summary>Galeri</summary>
          <ul class="bg-base-100 rounded-t-none p-2">
            <li><a>Link 1</a></li>
            <li><a>Link 2</a></li>
          </ul>
        </details>
      </li>
    </ul>
  </div>
</div>
</template>