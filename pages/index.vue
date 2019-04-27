<template>
    <main>
      <h1>What Dinner?</h1>
      <p>
          Can't decide what to have for dinner? Store your favorite meals in the app and let it decide for you!
      </p>
      <section class="badges">
          <div class="badge">
              <a href="https://itunes.apple.com/us/app/what-dinner/id1407394720">
                  <img src="/images/app-store-button.svg" alt="Download on the app store"></a>
              <a href="https://itunes.apple.com/us/app/what-dinner/id1407394720">
                  <p>Download for iOS</p>
              </a>
          </div>
          <div class="badge">
              <a href="https://play.google.com/store/apps/details?id=nl.joseewouters.dinner">
                  <img src="/images/google-play-badge.png" alt="Get it on Google Play"></a>
              <a href="https://play.google.com/store/apps/details?id=nl.joseewouters.dinner">
                  <p>Download for Android</p>
              </a>
          </div>
      </section>
    </main>
</template>

<script>

export default {

}
</script>

<style lang="scss">
main {
    padding: 1em;
    -webkit-backdrop-filter: blur(2px);
    backdrop-filter: blur(2px);
    background: rgba(255, 255, 255, 0.9);
    min-height: calc(100vh - 2em);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.badge {
    display: flex;
    align-items: center;
    margin-top: 2em;
    color: $secondary;
    img {
        margin-right: 1em;
        width: 120px;
    }
}

h1 {
    font-size: 3rem;
}
</style>
