<template>
      <div class="container">
          <h1 class="title">What Dinner?</h1>
          <p>
              Can't decide what to have for dinner? 
          </p>
          <p>
              Store your favorite meals in the app and let it decide for you!
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
                      <img src="/images/google-play-badge.png" alt="Get it on Google Play">
                  </a>
              </div>
          </section>
      </div>
</template>

<script>

export default {

}
</script>

<style lang="scss">

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

.title {
    font-size: 3rem;
}
</style>
