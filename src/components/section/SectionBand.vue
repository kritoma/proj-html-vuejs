<template>
  <section>
    <div class="container">
        <TitleSection  class="py-5" title="Latest Band News"/>
        <div class="bands">
          <div class="band">
            <img src="../../assets/img/blog_music_techo-400x200.jpg" alt="blog-music-techo">
            <div class="content_band">
              <h4>Technology and music</h4>
              <p>Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum.</p>
            </div>
          </div>
          <div class="band">
            <img src="../../assets/img/blog-post1-200x300.jpg" alt="blog-post1">
            <div class="content_band">
              <h4>Taking it back to the old school</h4>
              <p>Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum.</p>
            </div>
          </div>
          <div class="band">
            <img src="../../assets/img/blog-post3-200x300.jpg" alt="blog-post1">
            <div class="content_band">
              <h4>While my guitar gently weeps</h4>
              <p>Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum.</p>
            </div>
          </div>
          <div class="band">
            <img src="../../assets/img/blog-post4-200x300.jpg" alt="blog-post1">
            <div class="content_band">
              <h4>It just sounds better</h4>
              <p>Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum.</p>
            </div>
          </div>
          <div class="band">
            <img src="../../assets/img/blog-post2-200x300.jpg" alt="blog-post1">
            <div class="content_band">
              <h4>Sharing the stage with a legend</h4>
              <p>Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum.</p>
            </div>
          </div>
          <div class="band">
            <img src="../../assets/img/blog_flavor_rock-400x200.jpg" alt="blog-post1">
            <div class="content_band">
              <h4>The flavor of rock</h4>
              <p>Sed sit amet sem turpis. Curabitur cursus lacinia est at interdum risus id condimentum.</p>
            </div>
          </div>
        </div>
    </div>
    <DisplayBar text="VIEW ALL LATEST NEWS"/>
  </section>
</template>

<script>
import DisplayBar from '../common/DisplayBar.vue';
import TitleSection from '../common/TitleSection.vue';

export default {
  components: { TitleSection, DisplayBar },
    name: "SectionBand"
}
</script>

<style lang="scss" scoped>
section{
    background-color: #252a33;
    
}

.bands {
  margin: 3.75rem 0;
  display: grid;
  gap: .625rem;
  grid-auto-columns: 1fr;
  grid-template-areas: 
    "uno uno due"
    "tre quattro due"
    "tre quattro cinque"
    "sei sei cinque" 
  ;

  .band {
    background-color: #323844;


    img {
    width: 100%;
    }

    .content_band {
      padding: 20px;
    }

    h4 {
      color: var(--color-primary);
    }

    p {
      color: #7d7b8d;
    }
  }
  
  
}

.band:nth-child(1) {
  grid-area: uno;
}
.band:nth-child(2) {
  grid-area: due;
}
.band:nth-child(3) {
  grid-area: tre;
}
.band:nth-child(4) {
  grid-area: quattro;
}
.band:nth-child(5) {
  grid-area: cinque;
}
.band:nth-child(6) {
  grid-area: sei;
}
</style>