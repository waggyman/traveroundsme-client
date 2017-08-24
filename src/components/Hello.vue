<template>
  <div class="hello">
    <section class="section-1">
      <div class="container is-fluid">
        <div class="tv-content" style="padding-top: 20px;">
          <div class="columns">
            <div class="column">
              <p class="tv-header mb-0">
                TraveroundsMe
              </p>
              <p style="font-size: 22px;" class="tv-text-center">
               Together travel everywhere, discover new place, new foods, new culture, and new experience
              </p>
            </div>
          </div>
          <div class="columns is-centered">
            <div class="column is-8">
              <div class="field">
                <div style="position: relative">
                  <input type="text" class="tv-form-control" placeholder="search location">
                  <span class="icon tv-form-inline-icon is-small is-left">
                    <i class="fa fa-search"></i>
                  </span>
                </div>
              </div>
            </div>
          </div>
          <div class="columns is-centered">
            <div class="column is-10">
              <div class="columns">
                <div class="column is-4">
                  <div class="card">
                    <div class="card-image">
                      <figure class="image is-4by3">
                        <img src="http://bulma.io/images/placeholders/1280x960.png" alt="Image">
                      </figure>
                    </div>
                    <div class="card-content">
                      <div class="media">
                        <div class="media-left">
                          <figure class="image is-48x48">
                            <img src="http://bulma.io/images/placeholders/96x96.png" alt="Image">
                          </figure>
                        </div>
                        <div class="media-content">
                          <p class="title is-4">John Smith</p>
                          <p class="subtitle is-6">@johnsmith</p>
                        </div>
                      </div>

                      <div class="content">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                        Phasellus nec iaculis mauris. <a>@bulmaio</a>.
                        <a>#css</a> <a>#responsive</a>
                        <br>
                        <small>11:09 PM - 1 Jan 2016</small>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="column is-4">
                  <div class="card">
                    <div class="card-image">
                      <figure class="image is-4by3">
                        <img src="http://bulma.io/images/placeholders/1280x960.png" alt="Image">
                      </figure>
                    </div>
                    <div class="card-content">
                      <div class="media">
                        <div class="media-left">
                          <figure class="image is-48x48">
                            <img src="http://bulma.io/images/placeholders/96x96.png" alt="Image">
                          </figure>
                        </div>
                        <div class="media-content">
                          <p class="title is-4">John Smith</p>
                          <p class="subtitle is-6">@johnsmith</p>
                        </div>
                      </div>

                      <div class="content">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                        Phasellus nec iaculis mauris. <a>@bulmaio</a>.
                        <a>#css</a> <a>#responsive</a>
                        <br>
                        <small>11:09 PM - 1 Jan 2016</small>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="column is-4">
                  <div class="card">
                    <div class="card-image">
                      <figure class="image is-4by3">
                        <img src="http://bulma.io/images/placeholders/1280x960.png" alt="Image">
                      </figure>
                    </div>
                    <div class="card-content">
                      <div class="media">
                        <div class="media-left">
                          <figure class="image is-48x48">
                            <img src="http://bulma.io/images/placeholders/96x96.png" alt="Image">
                          </figure>
                        </div>
                        <div class="media-content">
                          <p class="title is-4" style="font-size: 18px; margin-bottom: 10px;">Taman Musik Dipatiukur</p>
                          <p class="subtitle is-6" style="margin-top: 5px"><small style="font-size: 12px">Jl. Manukan Ranu 21C (4km) </small>
                            &nbsp;
                            <span class="icon" style="width: 15px; height: 20px;">
                              <i class="fa fa-star" style="font-size: 15px"></i>
                            </span>
                            <small>4.5</small>
                          </p>
                        </div>
                      </div>

                      <div class="content">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit.
                        Phasellus nec iaculis mauris. <a>@bulmaio</a>.
                        <a>#css</a> <a>#responsive</a>
                        <br>
                        <small>11:09 PM - 1 Jan 2016</small>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js PWA'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  .section-1 {
    padding-bottom: 72px;
    padding-top: 36px;
    /*background-image: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)), url('https://static.pexels.com/photos/266046/pexels-photo-266046.jpeg');*/
    background: linear-gradient(rgba(0,0,0,0.4),rgba(0,0,0,0.4)), url('https://static.pexels.com/photos/220444/pexels-photo-220444.jpeg') center center no-repeat;
    background-attachment: fixed;
  }
  .tv-content {
    color: white;
  }
  .tv-primary-outline {
    color: #40ffad;
    background-color: transparent;
    padding: 10px 20px;
    border: 2px solid #00B467;
    border-radius: 5px;
  }

  .tv-primary-outline:hover {
    background-color: #00B467;
    color: #f5f5f5;
    border: 2px solid #00B467;
  }
</style>
