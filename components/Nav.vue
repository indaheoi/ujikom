<template>
   <div class="navbar group relative ms-4 cursor-pointer items-end justify-end m-0">
  <div class="flex-none">
    <ul class="menu-hover menu relative menu-horizontal px-1 gap-4">
      <li>
        <details>
          <summary><NuxtLink to="/">Beranda</NuxtLink></summary>
        </details>
      </li>
      <li>
        <details>
          <summary>Profil</summary>
          <ul class="bg-base-100 rounded-t-none p-2">
            <li> <NuxtLink to="/profil/identitas"><a>Identitas Sekolah</a> </NuxtLink></li>
            <li> <NuxtLink to="/profil/sejarah"><a>Sejarah</a> </NuxtLink></li>
            <li> <NuxtLink to="/profil/visimisi"><a>Visi & Misi</a> </NuxtLink></li>
            <li> <NuxtLink to="/profil/kepsek"><a>Kepala Sekolah</a> </NuxtLink></li>
            <li> <NuxtLink to="/profil/guru"><a>Guru & Staf</a> </NuxtLink></li>
   
          </ul>
        </details>
      </li>
      <li>
        <details>
         
          <summary> <NuxtLink to="/jurusan">Konsentrasi Keahlian</NuxtLink></summary>
          <ul class="bg-base-100 rounded-t-none p-2">
            <li><a>TJKT</a></li>
            <li><a>PPLG</a></li>
            <li><a>TSM</a></li>
            <li><a>DKV</a></li>
            <li><a>TOI</a></li>
          </ul>
        </details>
      </li>
      <li>
        <details>
          <summary> <NuxtLink to="/ekskul">Ekstrakulikuler</NuxtLink></summary>
          <ul class="bg-base-100 rounded-t-none p-2">
            <li><a>Link 1</a></li>
            <li><a>Link 2</a></li>
          </ul>
        </details>
      </li>
      <li>
        <details>
          <summary> <NuxtLink to="/galeri">Galeri</NuxtLink></summary>
        </details>
      </li>
      <li>
        <details>
          <summary><NuxtLink to="/berita">Berita</NuxtLink></summary>
        </details>
      </li>
    </ul>
  </div>
</div>
</template>