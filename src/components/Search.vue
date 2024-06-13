<template>
  <div class="mobile-search">
    <div class="search-container">
      <div class="search-input">
        <input
            type="search"
            class="hppsearch"
            v-model="search"
            name="hppsearch"
            placeholder="Search"
            @keyup="handleSrach"
        />
        <img @click="navigateToSearch()" src="../assets/icons/search.svg" alt="search icon">
      </div>
      <div class="dropdown-content" v-if="showSearch">
        <ul class="sub sub-menu-block" >
          <li
              @click="showSearch = false;"
              v-for="(item, index) in allProducts"
              :key="index"
              class="child-1"
          >
            <nuxt-link v-if="item.item_type == 'category' && item.type == 0"
                       :to="{ name: 'industry-slug', params: { slug: item.slug } }"
            >
              <p class="mb-0">{{ item.title }}</p>
              <p   class="mb-0">({{ item.product_count }})</p>
            </nuxt-link>
            <nuxt-link v-else-if="item.item_type == 'category' && (item.type == 1 || item.type == 2)"
                       :to="'/' + item.slug"
            >
              <p class="mb-0">{{ item.title }}</p>
              <p   class="mb-0">({{ item.product_count }})</p>
            </nuxt-link>
            <nuxt-link v-else-if="item.item_type == 'blog'"
                       :to="'blog/' + item.slug"
            >{{ item.title }}</nuxt-link>
            <nuxt-link v-else
                       :to="{
                  name: 'industry-product',
                  params: {
                    industry: item.type,
                    product: item.slug,
                  },
                }"
            >{{ item.title }}</nuxt-link>
          </li>
          <li v-if="allProducts.length <= 0"><p>No search results found!</p></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Search",
  data:() =>{
    return {
      search:"",
      showSearch:false,
      allProducts:"",
    }
  },
  methods:{
    async handleSrach(){
      if(this.search.length >= 3){
        this.allProducts = await this.$axios.$get(`/search?q=${this.search}`);
        this.showSearch = true;
      }
    },
    navigateToSearch() {
      if(this.search.length >= 3){
        this.$router.push({ name: 'search', params: { query: this.search } });
      }else{
        this.$router.push({ name: 'catalogue', params: { id: null } });
      }

    },
    handleDocumentClick(){
      this.showSearch = false;
    }
  },
  mounted() {
    document.addEventListener("click", this.handleDocumentClick);
  },
  beforeDestroy() {
    document.removeEventListener("click", this.handleDocumentClick);
  },
};
</script>

<style lang="scss" scoped>
.hppsearch {
  all: unset;
  min-width: 270px;
  padding: 10px 20px;
  padding-right: 45px;
  background:  #f2f2f2;
  background-size: 20px;
  background-position: 96%;
}

.search-input{
  display: flex;
  gap: 5px;
  background: #f2f2f2;
  border-radius: 8px;
  width: 100%;

  img{
    padding: 3px 8px;
    cursor: pointer;
    width: 40px;
  }
}
.sub {
  background-color: #fff;
  border-bottom-right-radius: 4px;
  border-bottom-left-radius: 4px;
  position: absolute;
  display: grid;
  transition: all 0.3s ease;
  z-index: 11;
  // opacity: 0;
  -webkit-transition: all 0.4s ease 0s;
  transition: all 0.4s ease 0s;
  // -webkit-transform: rotateX(90deg);
  // transform: rotateX(90deg);
  -webkit-transform-origin: top center;
  transform-origin: top center;
  -webkit-box-shadow: 0 2px 4px 0 rgb(0 0 0 / 10%);
  box-shadow: 0 2px 4px 0 rgb(0 0 0 / 10%);
}
.sub-menu-block {
  list-style-type: none;
  border-bottom-right-radius: 4px;
  border-bottom-left-radius: 4px;
  min-width: 413px;
  max-height: 70vh;
  overflow-y: auto;
  top: 65%;
  padding-top: 12px !important;
}
.sub-menu-block::-webkit-scrollbar {
  width: 7px;
}

/* Style the scrollbar thumb */
.sub-menu-block::-webkit-scrollbar-thumb {
  background-color: #888;
  border-radius: 5px;
}

/* Style the scrollbar thumb when hovered */
.sub-menu-block::-webkit-scrollbar-thumb:hover {
  background-color: #555;
}
.sub-menu-block li {
  padding: 4px 8px;
  transition: 0.3s all ease;
  border-bottom: 1px solid #ddd;
  margin-right: 0 !important;
}
.sub-menu-block li a{
  display: flex;
  gap: 20px;

}
.sub-menu-block li:hover {
  background: #ef5f5b;
}
.sub-menu-block li:hover p {
  color: white !important;
}
.sub-menu-block li:hover a {
  text-decoration: none !important;
  color: white !important;
}
@media only screen and (max-width: 1199px){
  .hppsearch {
    min-width: 200px;
  }
  .sub-menu-block {
    min-width: 200px;
  }
}
@media (max-width: 640px) {
  .hppsearch {
    min-width: 100%;
  }
}
@media (max-width:480px) {
  .hppsearch {
    width: 100%;
  }
  .mobile-search{
    width: 80%;
    margin-top: 20px;
  }
  .search-container{
    width: 100%;
  }
}
</style>