<template>
  <div>
      <div class="">
        <slot></slot>
    <q-carousel
      v-model="slide"
      transition-prev="scale"
      transition-next="scale"
      swipeable
      animated
      control-color="white"
      navigation
      padding
      arrows
      height="600px"
      class="bg-primary text-white shadow-1 rounded-borders "
    >
      <template v-slot:navigation-icon="{ active, btnProps, onClick }">
        <q-btn v-if="active" size="lg" icon="home" color="yellow" flat round dense @click="onClick" />
        <q-btn v-else size="sm" :icon="btnProps.icon" color="white" flat round dense @click="onClick" />

      </template>

      <q-carousel-slide name="style" class="column no-wrap flex-center images-url">
        <div class="q-mt-md text-center">
           <div class="text-p">TESTIMONIALS</div><br>
             <div class="text-h4 text-center">Our Riders Said About Us</div><br><br>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;" /><br><br>
               <div class="text-h5">“Everything was as expected and agreed. They know their thing and also  <br> know the place very well.”</div><br>
               <div class="row flex-center">
                 <q-img height="70px" width="70px" class="q-mr-lg" src="	https://xtrm.foxthemes.me/wp-content/uploads/2018/09/Group-13.png" />
               <div>ANDRW GOSHO <br> <span class="q-mr-xl">Pro Rider</span></div>
               </div>
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="tv" class="column no-wrap flex-center images-url">
        <div class="q-mt-md text-center">
                  <div class="text-p">TESTIMONIALS</div><br>
             <div class="text-h4 text-center">Our Riders Said About Us</div><br><br>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;" /><br><br>
               <div class="text-h5">“Everything was as expected and agreed. They know their thing and also  <br> know the place very well.”</div><br>
               <div class="row flex-center">
                 <q-img height="70px" width="70px" class="q-mr-lg" src="	https://xtrm.foxthemes.me/wp-content/uploads/2018/09/Group-13.png" />
                  <div>ANDRW GOSHO <br> <span class="q-mr-xl">Pro Rider</span></div>
               </div>
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="layers" class="column no-wrap flex-center images-url">
        <div class="q-mt-md text-center">
          <div class="text-p">TESTIMONIALS</div><br>
          <div class="text-h4 text-center">Our Riders Said About Us</div><br><br>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;"/>
               <q-icon size="22px" name="star_border" style="color: yellow;" /><br><br>
          <div class="text-h5">“Everything was as expected and agreed. They know their thing and also  <br> know the place very well.”</div><br>
          <div class="row flex-center">
               <q-img height="70px" width="70px" class="q-mr-lg" src="	https://xtrm.foxthemes.me/wp-content/uploads/2018/09/Group-13.png" />
                  <div>ANDRW GOSHO <br> <span class="q-mr-xl">Pro Rider</span></div>
               </div>
        </div>
      </q-carousel-slide>
    </q-carousel>
  </div>
  </div>
</template>


<script>

export default {
    setup() {
        return {
            slide: ref("style"),
            lorem: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque voluptatem totam, architecto cupiditate officia rerum, error dignissimos praesentium libero ab nemo."
        };
    },
}
</script>

<style scoped>

</style>
