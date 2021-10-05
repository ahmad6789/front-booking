<template>
  <div class="home">
    <!-- Button trigger modal -->
    <Sidebar></Sidebar>
    <div class="content" id="content">
      <div
        class="container-fluid overflow-auto"
        v-for="(item, i) in items"
        :key="i"
      >
        <h2 class="text-right">{{ item.name }}</h2>
        <div class="row d-flex flex-row flex-nowrap">
          <div
            class="col-12 col-md-4 col-sm-6"
            v-for="(cteg, i) in item['ctegories']"
            :key="i"
          >
            <div class="card mb-4 shadow-sm">
              <img :src="cteg.photo_center" height="225" class="img-card" />
              <div class="card-body">
                <h5 class="text-success">
                  {{ cteg.name }}
                </h5>
                <p class="card-text">
                  قبل الحسم: <del>{{ cteg.price }}</del
                  ><br />
                  السعر بعد الحسم:{{ cteg.price_discount }}
                </p>
                <div class="d-flex justify-content-between align-items-center">
                  <div class="">
                    <span style="font-size: 12px; color: #9e9e9e"
                      >تم النشر :{{ cteg.created_at }}</span
                    >
                    <button type="button" class="btn btn-sm btn-success mx-1">
                      التفاصيل
                    </button>
                    <button type="button" class="btn btn-sm btn-primary mx-1">
                      الحجز
                    </button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import axios from "axios";
import Sidebar from "@/components/sidebar.vue";
export default {
  name: "Home",
  components: {
    Sidebar,
  },
  data() {
    return {
      items: [],
    };
  },

  created() {
    this.getItem();
  },

  methods: {
    getItem() {
      axios
        .get("http://localhost:8000/api/Show-item")
        .then((response) => {
          console.log(response.data);
          this.items = response.data;
        })
        .catch((error) => {
          console.log(error);
        });
    },
  },
};
</script>
<style scoped>
.card {
  border-radius: 1.25rem;
}

.img-card {
  border-top-left-radius: 1.25rem;
  border-top-right-radius: 1.25rem;
}
@media (min-width: 768px) {
  .bd-placeholder-img-lg {
    font-size: 3.5rem;
  }
}
.content {
  background-color: #f5faf8;
  margin-right: 16px;
  margin-left: 16px;
}
@media screen and (min-width: 992px) {
  .content {
    margin-right: 250px;
    margin-left: 250px;
  }
}

.text-right{
  text-align: right;
}
</style>
