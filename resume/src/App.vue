<template>
  <div class="media">
        <div class="container">
            <div class="row">
                <div class="col-sm-6">
                    <div class="media__info">
                        <a href="mailto:zackneron@gmail.com">zackneron@gmail.com</a>
                        <a href="tel:+27624129173">0624129173</a>
                    </div>
                </div>
                <div class="col-sm-6">
                    <a href="">
                        <i class="fa fa-info"></i>
                    </a>
                        <a href="tel:+27624129173">0624129173</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import TopContactBar from './components/TopContactBar.vue'

export default {
  name: 'App',
  components: {
    TopContactBar, 
  }
}
</script>

<style lang="scss">
.media {
  background: #080808;
  padding: 5px 0;
  position: relative;
  z-index: 1;

    &::after {
      background: #df0a0a;
      content: '';
      position: absolute;
      top: 0;
      left: -12px;
      width: 51%;
      height: 100%;
      z-index: -1;
      transform: skew(25deg);
      padding-left: 20px;
  }

  a {
    color: white;
  }
}
</style>