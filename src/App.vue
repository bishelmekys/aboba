<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
    <div class="container-fluid">
      <RouterLink class="navbar-brand" to="/">Home</RouterLink>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <RouterLink class="nav-link active" aria-current="page" to="/about"
              >ОГЭ</RouterLink
            >
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link" to="/ege">ЕГЭ</RouterLink>
          </li>
          <li class="nav-item">
            <a
              class="nav-link"
              target="_blank"
              href="https://synergy.ru/assets/upload/news/articles_oge/oge/fizika/демоверсии/fi_9_oge_2023_kodif.pdf"
              >Кодификатор ОГЭ</a
            >
          </li>
          <li class="nav-item">
            <a
              class="nav-link"
              target="_blank"
              href="https://synergy.ru/assets/upload/news/articles_ege/ege/fizika/демоверсии/fi_11_ege_2024_kodif.pdf"
              >Кодификатор EГЭ</a
            >
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <RouterView />
</template>

<style scoped></style>
