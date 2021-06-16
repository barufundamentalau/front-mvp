<template>
  <footer>
    <div class="container-fluid" style="background: white">
      <div class="row p-4">
        <div class="col-md-4">
          <h5>TENTANG</h5>
          <hr />
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorum
            necessitatibus nemo facere tenetur iste molestiae natus eaque.
            Aliquam enim modi id repellendus, temporibus odio sequi, vitae
            laudantium, dolorum ea nam!
          </p>
          <div class="social mt-4" style="margin-bottom: 30px">
            <a href="https://www.facebook.com"
              ><img
                src="assets/images/svg/facebook.svg"
                style="width: 25px"
                class="icon-footer"
            /></a>
            <a href="https://www.instagram.com"
              ><img
                src="assets/images/svg/instagram.svg"
                style="width: 25px"
                class="icon-footer"
            /></a>
            <a href="https://www.twitter.com"
              ><img
                src="assets/images/svg/twitter.svg"
                style="width: 25px"
                class="icon-footer"
            /></a>
            <a href="https://www.youtube.com"
              ><img
                src="assets/images/svg/youtube.svg"
                style="width: 25px"
                class="icon-footer"
            /></a>
          </div>
        </div>
        <div class="col-md-4">
          <h5>KATEGORI</h5>
          <hr />
          <div v-if="tags.length > 0">
            <router-link
              :to="{ name: 'detail_tag', params: { slug: tag.slug } }"
              v-for="tag in tags"
              :key="tag.id"
              class="btn btn-sm btn-outline-secondary mb-2 mr-2"
              >{{ tag.name.toUpperCase() }}</router-link
            >
          </div>
          <div v-else class="text-center">
            <ListLoader />
          </div>
        </div>
        <div class="col-md-4">
          <h5>ALAMAT</h5>
          <hr />
          <p>
            <i class="fa fa-map-marker" aria-hidden="true"></i> Jl. XXX
            <br />
            <br />
            <i class="fas fa-phone-alt"></i> +62852-1234-5678
          </p>
        </div>
      </div>
    </div>
    <div class="container-fluid bg-dark">
      <div class="row p-3">
        <div class="text-center text-white">
          © Pemerintah Kabupaten Bolaang Mongondow 2021 Dinas Pariwisata
          <br />Dikembangkan oleh e-Gov Diskominfo Bolmong
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
//import content loader
import { ListLoader } from "vue-content-loader";

//import axios
import axios from "axios";

export default {
  name: "Footer",
  components: {
    //loader component
    ListLoader,
  },
  data() {
    return {
      tags: [],
    };
  },
  created() {
    axios.get("/api/tag").then((response) => {
      this.tags = response.data.data.data;
    });
  },
};
</script>