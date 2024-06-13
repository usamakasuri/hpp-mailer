<template>
  <section id="desktop-menu">
    <div class="header-top-bar text-center">
      <a href="#">
        <img src="../assets/images/bulk-order-deal.7f2832d.jpg" alt="bul order" width="700" />
      </a>
    </div>

    <div class="container-fluid">
      <div class="row pt-4 pb-4">
        <div class="col-md-2">
          <img src="../assets/images/logo.svg" width="200" alt="logo" />
        </div>
        <div class="col-md-4">
          <div class="header-search">
            <div class="input-group mb-3">
              <input type="text" class="form-control" placeholder="Search"
                aria-label="Recipient's username" aria-describedby="button-addon2">
              <button class="btn btn-outline-secondary" type="button" id="button-addon2">
                <img src="../assets/images/search_icon.svg" alt="search" width="30" />
              </button>
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="talk-to-expert text-center">
            <p class="m-0">Talk to our packaging experts</p>
            <a href="tel:866-225-2112">866-225-2112</a>
          </div>
        </div>
        <div class="col-md-3">
          <div class="talk-to-expert-email text-center">
            <p class="m-0 invisible">Talk to our packaging experts</p>
            <a href="mailto:orders@halfpricepackaging.com">orders@halfpricepackaging.com</a>
          </div>
        </div>
      </div>
    </div>


    <!-- navbar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Navbar</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link" href="#">Industries <span></span></a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
            </li>
          </ul>
<!--          <form class="d-flex">-->
<!--            <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">-->
<!--            <button class="btn btn-outline-success" type="submit">Search</button>-->
<!--          </form>-->
        </div>
      </div>
    </nav>
    <!-- end navbar -->

   

  </section>
</template>
<script setup lang="ts">
</script>

<style scoped>
.header-top-bar {
  border-bottom: 1px solid rgba(0, 0, 0, .1);
  padding: 20px 0px;
}

.header-search {
  font-family: var(--fontFamily);
  button {
    border: none;
    background: transparent;
  }
  input {
    box-shadow: none;
    border: none;
    background-color: #F2F2F2;
  }
  .input-group {
    border: 1px solid #F2F2F2;
    background-color: #F2F2F2;
    padding: 5px;
    border-radius: 10px;
  }
}

.talk-to-expert {
  font-family: var(--fontFamily);
  p {
    font-size: 16px;
  }
  a {
    color: #007bff;
    font-size: 20px;
    font-weight: 600;
    text-decoration: none;
  }
  a:hover {
    color: #EF4B59;
    text-decoration: underline;
  }
}

</style>