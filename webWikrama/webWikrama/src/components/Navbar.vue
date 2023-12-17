<template>
    <nav class="navbar navbar-expand-lg">
    <div class="container-fluid">
      <img class="navbar-brand" src="/img/Nav-logo.png" alt="Nav Logo">
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-center" id="navbarSupportedContent">
        <ul class="navbar-nav">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Beranda</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Program Keahlian
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">PPLG</a></li>
            <li><a class="dropdown-item" href="#">TKJT</a></li>
            <!-- <li><hr class="dropdown-divider"></li> -->
            <li><a class="dropdown-item" href="#">KLN</a></li>
            <li><a class="dropdown-item" href="#">HTL</a></li>
            <li><a class="dropdown-item" href="#">PMN</a></li>
            <li><a class="dropdown-item" href="#">BDP</a></li>
            <li><a class="dropdown-item" href="#">DKV</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">PPDB 2024-2025</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Kurikulum</a>
        </li>
      </ul>
    </div>
    <div class="d-flex flex-row-reverse">
      <button class="btn btn-primary">Daftar</button>
    </div>
  </div>
</nav>
</template>

<script>
export default {
    name: 'Navbar',
}
</script>

<style>

</style>