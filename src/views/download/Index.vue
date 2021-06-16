<template>
  <div class="post-index">
    <!-- header -->
    <Header />
    <!-- end header -->

    <!-- main content -->
    <header class="pt-5 border-bottom bg-light">
      <div class="container pt-md-1 pb-md-1">
        <h1 class="bd-title mt-4 font-weight-bold">
          <i class="fas fa-download" aria-hidden="true"></i> UNDUHAN
        </h1>
        <p class="bd-lead">Download File</p>
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
          <router-link :to="{ name: 'download' }" class="text-decoration-none"
            >Unduhan</router-link
          >
        </li>
      </ol>
    </nav>
    <!-- end breadcrumb -->

    <div class="container-fluid mt-5 mb-5">
      <div class="row">
        <div class="col-md-12">
          <div class="card border-0 shadow-sm rounded">
            <div class="card-body">
              <table class="table table-striped">
                <thead>
                  <tr>
                    <th scope="col">No.</th>
                    <th scope="col">Nama Data</th>
                    <th scope="col">Ukuran</th>
                    <th scope="col">Tanggal</th>
                    <th scope="col">Tindakan</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <th scope="row">1</th>
                    <td>Foto Bupati</td>
                    <td>947373 Kb</td>
                    <td>Jumat, 07 Juli 2021</td>
                    <td width="277">
                      <a class="btn btn-primary"> Download </a>
                    </td>
                  </tr>
                  <tr>
                    <th scope="row">2</th>
                    <td>Foto Wakil Bupati</td>
                    <td>947373 Kb</td>
                    <td>Jumat, 07 Juli 2021</td>
                    <td width="277">
                      <a class="btn btn-primary"> Download </a>
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>
          </div>
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
  name: "DownloadIndex",
  components: {
    Header,
    Footer,
  },
};
</script>