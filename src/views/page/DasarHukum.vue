<template>
  <div class="post-index">
    <!-- header -->
    <Header />
    <!-- end header -->

    <!-- main content -->
    <header class="pt-5 border-bottom bg-light">
      <div class="container pt-md-1 pb-md-1">
        <h1 class="bd-title mt-4 font-weight-bold">
          <i class="fas fa-download" aria-hidden="true"></i> Dasar Hukum
        </h1>
        <p class="bd-lead">Dasar Hukum Dinas Perumahan dan Kawasan Permukiman Kabupaten Bolaang Mongondow</p>
      </div>
    </header>

    <!-- breadcrumb -->
    <nav aria-label="breadcrumb">
      <ol class="breadcrumb">
        <li class="breadcrumb-item">
          <router-link :to="{ name: 'home' }" class="text-decoration-none"
            ><i class="fa fa-home"></i> Beranda</router-link
          >
        </li>
        <li class="breadcrumb-item">
          <router-link :to="{ name: 'dasarhukum' }" class="text-decoration-none"
            >Dasar Hukum</router-link
          >
        </li>
      </ol>
    </nav>
    <!-- end breadcrumb -->

        <div class="container-fluid mt-5 mb-5">

            <div class="row">

                <div class="row">

                </div>

                <div>
                    <div class="alert alert-danger">
                        DATA BERITA BELUM TERSEDIA !
                    </div>
                </div>

                <div class="text-center" v-show="moreExists">
                    <button type="button" class="btn btn-primary btn-md" v-on:click="loadMore"><span class="fa fa-arrow-down"></span> LIHAT LEBIH BANYAK</button>
                </div>

            </div>
        </div>
    <!-- main content -->

    <!-- footer -->
    <Footer />
    <!-- end footer -->
  </div>
</template>

<script>
//import component
import Header from "@/components/Header";
import Footer from "@/components/Footer";

export default {
  name: "DasarHukumIndex",
  components: {
    Header,
    Footer,
  },
};
</script>
