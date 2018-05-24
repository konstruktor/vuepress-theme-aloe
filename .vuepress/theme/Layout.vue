<template>
  <div class="container my-5">
    <div id="header" class="row mb-4">
      <div class="col">
        <div class="d-flex flex-row">
          <div class="p-2 bd-highlight">Flex item 1</div>
          <div class="p-2 bd-highlight">
            <span class="d-block p-2">
              <h1>Aloe Classic</h1>
            </span>
            <span class="d-block p-2">
              <ul class="nav">
                <li class="nav-item" v-for="item in this.$site.themeConfig.nav">
                  <a class="nav-link active" href="#">
                    {{ item.text }}
                  </a>
                </li>
              </ul>
            </span>
          </div>
        </div>
      </div>
    </div>

    <div id="about" class="row">
      <div class="col">
        {{ this.$site }}
      </div>
    </div>

    <div id="writing" class="row">
      <div class="col">
        <h2>Writing</h2>
        <dl class="row">
          <dt class="col-sm-3">Description lists</dt>
          <dd class="col-sm-9">A description list is perfect for defining terms.</dd>
        </dl>
      </div>
    </div>

    <div id="projects" class="row">
      <div class="col">
        <h2>Projects</h2>
        <ul class="list-unstyled">
          <li>Description lists</li>
          <li>A description list is perfect for defining terms.</li>
        </ul>
      </div>
    </div>

    <div id="footer" class="row">
      <div class="col">
        Copyright © 2018 Madis Väin
      </div>
    </div>
  </div>
</template>

<style lang="scss">
  @import '~bootstrap/scss/bootstrap.scss';
  @import url('https://fonts.googleapis.com/css?family=Inconsolata:400,700&subset=latin-ext');

  html, body, #app {
    height: 100%;
    font-family: 'Inconsolata', monospace;
  }
  #app {
    border-top: 2px solid #22272a;
  }
</style>
