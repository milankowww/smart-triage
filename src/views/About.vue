<template>
  <div class="main-container">
    <NavBar :back-btn="true"></NavBar>
    <h1 class="mb-6">{{ $t('ABOUT.ABOUT_THIS_APP') }}</h1>
    <div class="main-content">
      <img class="m-6" src="@/assets/img/home-page-welcome-img.png" alt="" />
      <div class="card">
        <p>
          <strong>
            {{ $t('ABOUT.APP_SHORT_DESCRIPTION') }}
          </strong>
        </p>

        <p>
          {{ $t('ABOUT.TRIAGE_DESCRIPTION') }}
        </p>

        <p>
          {{ $t('ABOUT.CREATED_ON_HACKATHON') }}
        </p>
      </div>

      <div class="mb-6 mt-2">
        <h2>{{ $t('ABOUT.AUTHORS') }}</h2>
        <ul>
          <li>Vasil Kostin</li>
          <li>Tom Kuna</li>
          <li>Ľuboš Repka</li>
          <li>Tomáš Trejdl</li>
        </ul>
      </div>
    </div>
    <div class="bottom-link text-xs">
      {{ $store.state.app.appTitle }} {{ $t('ABOUT.VERSION') }}
      {{ $store.getters.appVersion }}
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped></style>
