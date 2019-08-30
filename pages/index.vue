<template>
  <div class="container">
    <div class="content-intro">
      <div class="inside-content">
          <h1 class="quicksand">Tomas Girčius</h1>
          <h2>WEB DEVELOPER AND MORE</h2>
          <span> Currently looking for Full-Stack web developer position</span>
      </div>
    </div>
    <div class="content-work">
      <nuxt-link to="/example/1/" aria-label="Example 1" class="item" style="background-image:url('images/1.jpg');"></nuxt-link>
      <nuxt-link to="/example/2/" aria-label="Example 2" class="item" style="background-image:url('images/3.jpg');"></nuxt-link>
      <nuxt-link to="/example/3/" aria-label="Example 3" class="item" style="background-image:url('images/2.jpg');"></nuxt-link>
      <nuxt-link to="/example/4/" aria-label="Example 4" class="item" style="background-image:url('images/log/2.jpg');"></nuxt-link>
    </div>
    <div class="canvas-holder">
      <div class="item">
        <h3>Tech I'm comfortable working with</h3>
        <canvas width="540" height="360" id="canvas-skills">
            <ul class="quicksand">
              <li><a href="#">HTML</a></li>
              <li><a href="#">CSS</a></li>
              <li><a href="#">JAVASCRIPT</a></li>
              <li><a href="#">JQUERY</a></li>
              <li><a href="#">VUE</a></li>
              <li><a href="#">SCSS</a></li>
              <li><a href="#">AJAX</a></li>
              <li><a href="#">GIT</a></li>
              <li><a href="#">BOOTSTRAP</a></li>
              <li><a href="#">PHP</a></li>
              <li><a href="#">SYMFONY</a></li>
              <li><a href="#">MYSQL</a></li>
            </ul>
        </canvas>
      </div>
      <div class="item">
        <h3>Tech I'm trying to improve on</h3>
        <canvas width="540" height="360" id="canvas-skills-meh">
            <ul class="quicksand">
              <li><a href="#">LARAVEL</a></li>
              <li><a href="#">NODE</a></li>
            </ul>
        </canvas>
      </div>
    </div>
    <div class="about">
      <h3 class="quicksand">Experience</h3>
      <ul>
        <li>1 year full-stack (SYMFONY 3.4+)</li>
        <li class="plus">+</li>
        <li>1 year front-end (mostly CSS, HTML, JS)</li>
      </ul>
    </div>
    <div class="contact">
      <h3 class="quicksand">Contact me</h3>
      <div class="item">
        <client-only>
          <a href="tel:+37063884498">
            <svg height="60" width="320" xmlns="http://www.w3.org/2000/svg">
              <rect class="shape" height="60" width="320" />
            </svg>
            <div class="text">+370 638 84 498</div>

          </a>
        </client-only>
      </div>
      <div class="item">
        <client-only>
          <a href="mailto:girciustomas@gmail.com?Subject=Important%20message!">
            <svg height="60" width="380" xmlns="http://www.w3.org/2000/svg">
              <rect class="shape" height="60" width="380" />
            </svg>
            <div class="text">girciustomas@gmail.com</div>
          </a>
        </client-only>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  mounted () {
    let cloudOptions = {
      textFont: 'Quicksand, sans-serif',
      textColour: '#5D34CB',
      textHeight: 50,
      noSelect: true,
      lock: 'xy',
      wheelZoom: false,
      initial: [0.2, 0]
    }

    try {
      document.fonts.ready.then(() => {
        TagCanvas.Start('canvas-skills', '', cloudOptions);
        TagCanvas.Start('canvas-skills-meh', '', cloudOptions);
      })
    } catch(e) {
      TagCanvas.Start('canvas-skills', '', cloudOptions);
      TagCanvas.Start('canvas-skills-meh', '', cloudOptions);
    }

  }
}
</script>

<style>

</style>
