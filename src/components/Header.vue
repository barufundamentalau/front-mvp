<template>
  <nav
    class="navbar navbar-expand-md navbar-dark fixed-top bg-dark"
    style="border-top: 2px solid rgb(54, 60, 228)"
  >
    <div class="container-fluid">
      <router-link :to="{ name: 'home' }" class="navbar-brand">
        Disperkim Bolmong
      </router-link>
      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarCollapse"
        aria-controls="navbarCollapse"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarCollapse">
        <ul class="navbar-nav mr-auto mb-2 mb-md-0">
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdown"
              role="button"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
              PROFIL
            </a>
            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
              <router-link :to="{ name: 'dasarhukum' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/puzzle.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Dasar Hukum</router-link
              >
              <router-link :to="{ name: 'dasarhukum' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/work.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Tugas Pokok dan Fungsi</router-link
              >
              <router-link :to="{ name: '404' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/user.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Struktur Organisasi</router-link
              >
              <router-link :to="{ name: '404' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/team.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Sumber Daya Manusia</router-link
              >
            </div>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdown"
              role="button"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
              BIDANG
            </a>
            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
              <router-link :to="{ name: 'post' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/newspaper.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Sekretariat</router-link
              >
              <router-link :to="{ name: 'event' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/calendar.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Bidang Perumahan Rakyat</router-link
              >
              <router-link :to="{ name: 'event' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/calendar.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Bidang Kawasan Permukiman</router-link
              >
              <router-link :to="{ name: 'event' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/calendar.svg"
                  class="rounded"
                  style="width: 20px"
                />
                UPTD</router-link
              >
            </div>
                      <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdown"
              role="button"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
              LAYANAN
            </a>
            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
              <router-link :to="{ name: '404' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/newspaper.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Pengajuan SOP RTLH</router-link
              >
              <router-link :to="{ name: '404' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/calendar.svg"
                  class="rounded"
                  style="width: 20px"
                />
                SOP Bedah Rumah</router-link
              >
              <router-link :to="{ name: '404' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/calendar.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Layanan Rusunawa</router-link
              >
            </div>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdown"
              role="button"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
              INFORMASI
            </a>
            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
              <router-link :to="{ name: 'post' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/newspaper.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Berita</router-link
              >
              <router-link :to="{ name: 'event' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/calendar.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Agenda</router-link
              >
            </div>
          </li>
          <li class="nav-item dropdown">
            <a
              class="nav-link dropdown-toggle"
              href="#"
              id="navbarDropdown"
              role="button"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            >
              GALERI
            </a>
            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
              <router-link :to="{ name: 'photo' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/photo.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Foto</router-link
              >
              <router-link :to="{ name: 'video' }" class="dropdown-item"
                ><img
                  src="assets/images/svg/video-camera.svg"
                  class="rounded"
                  style="width: 20px"
                />
                Video</router-link
              >
            </div>
          </li>
          <li class="nav-item">
            <router-link :to="{ name: 'download' }" class="nav-link">
              UNDUHAN</router-link
            >
          </li>
          <li class="nav-item">
            <router-link :to="{ name: 'contact' }" class="nav-link">
              KONTAK</router-link
            >
          </li>
        </ul>
        <form action="/search" method="get" class="d-none d-lg-block">
          <div class="input-group">
            <input
              name="q"
              type="text"
              class="form-control"
              placeholder="Kata kunci.."
            />
            <div class="input-group-append">
              <button class="btn btn-light">
                <svg
                  width="1em"
                  height="1em"
                  viewBox="0 0 16 16"
                  class="bi bi-search"
                  fill="currentcolor"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    fill-rule="evenodd"
                    d="M10.442 10.442a1 1 0 011.415.0l3.85 3.85a1 1 0 01-1.414 1.415l-3.85-3.85a1 1 0 010-1.415z"
                  ></path>
                  <path
                    fill-rule="evenodd"
                    d="M6.5 12a5.5 5.5.0 100-11 5.5 5.5.0 000 11zM13 6.5a6.5 6.5.0 11-13 0 6.5 6.5.0 0113 0z"
                  ></path>
                </svg>
              </button>
            </div>
          </div>
        </form>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Header",
};
</script>