<template>
    <div>
        <div>
          <div class="bg-grey-3">
            <div class="text-center">
                <img src="images/divider.png" alt="" width="80%" >
            </div>
            <div class="text-center">
                <span class="ruban text-h4 text-weight-thin text-primary">Noro & Ker</span> <br>
                <span class="ruban text-h6 text-weight-light text-primary">#NK2020</span> <br>
                <span class="text-grey-7">We're getting married.</span>
            </div>
            <div class="text-center">
                <img src="images/divider.png" alt="" width="80%" >
            </div>   
          </div>
          <q-carousel
            v-model="slid"
            swipeable
            animated
            autoplay
            infinite
            control-color="secondary"
            :navigation="navigation"
            :navigation-position="navPos"
            height="400px"
            class="bg-grey-8 text-white"
            >

            <q-carousel-slide :name="carousel.name" class="q-pa-none" v-for="carousel in topCarousel" :key="carousel.id">
                <div>
                    <q-img :src="carousel.imageUrl" height="400px"/>
                    <div class="custom-caption absolute-bottom text-white text-h4 text-weight-light">
                    {{ carousel.title }}
                    </div>
                </div>
            </q-carousel-slide>
          </q-carousel>
        </div>

    <!-- Invitation C A R D -->
    <div class="row justify-center q-ma-md">
      <div class="text-center">
          <img src="images/divider.png" alt="" width="70%" >
      </div> 

      <q-card class="q-px-xl q-pt-xl text-white bg-secondary text-center" style="max-width: 350px">
        <span class="text-h4 text-weight-light text-accent align-center">Save The Date <br> </span>             
        <span class="text-h7 text-weight-light">WEDDING CEREMONY <br> </span>
        <span class="text-h7 text-weight-thin">5th December, 2020 <br> <br> </span>        
        <span class="text-h7 text-weight-thin">URCC  Church Anglo Jos , Channel seven, Yakubu Gowon Way, Plateau State Nigeria. <br> <br> </span>
        <span class="text-h8">We are excited to celebrate with you! <br> </span> 
        <q-card-actions align="right">
          <a href="https://forms.gle/gaStXvZNsfFCzK8J9" target="_blank"><q-btn no-caps outline color="white" text-color="white" label="RSVP Now" /></a>
        </q-card-actions>          
      </q-card>      
    </div>

    <div class="text-center">
        <img src="images/divider.png" alt="" width="70%" >
    </div>  

    <div class="text-h5 text-weight-light text-primary text-center">Wedding Colors <br> </div>        
    <div class="text-center">
      <q-chip clickable color="primary" text-color="white">
        Plum Purple
      </q-chip>
      <q-chip clickable color="secondary" text-color="white">
        Silver
      </q-chip>
      <q-chip clickable color="accent" text-color="white">
        Peach
      </q-chip>            
    </div>

    <div class="text-center">
        <img src="images/divider.png" alt="" width="70%" >
    </div> 

    <!-- Couple Toast-->
    <!-- Two Cards - Groom-->
    <div class="row items-start justify-center  q-pa-md bg-grey-4 ">
      <q-card class="bg-primary" style="max-width: 300px">
          <img src="images/ker.jpg" alt="">
      </q-card>

      <q-card class="q-pa-md text-grey-7 bg-grey-3" style="max-width: 300px; width: 100%"> 
          <span class="text-weight-light text-h5 text-black">Noro, baby</span>
          <p>Each passing day, I thank God I met you. <br>
            We were made for eachother. We blend well.<br> 
            Thank you for choosing and sticking by me. <br>
            Thanks for your unique friendship. <br>
            I will love you and cherish you always.<br> 
            Slowly our love will grow like a rose blooms. <br>
            I'll love you to the end of time</p>                
      </q-card>
    </div>

    <!-- Two Cards - Bride-->
    <div class="row items-start justify-center  q-pa-md bg-grey-4 ">
      <q-card class="q-pa-md text-grey-7 bg-grey-3" style="max-width: 300px; width: 100%"> 
          <span class="text-weight-light text-h5 text-black">Ker, love</span>
          <p>Ever since I met you my life has changed. <br>
            You've shown  me the true meaning of love. <br>
            I promise to love you over and over again <br>
            ...even until the very end. </p>                
      </q-card>

      <q-card class="bg-primary" style="max-width: 300px">
          <img src="images/noro1.jpg" alt="">
      </q-card>      
    </div> 

    <div class="bg-grey-8">
        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>          
        <div class="text-weight-light text-h4 text-white text-center">
          Our Love Story
        </div>
        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>
<!-- C H A T Love Story -->
        <div class="q-pr-md q-pl-md q-pb-md row justify-center">
            <div class="text-white" style="width: 100%; max-width: 500px">
              <q-chat-message
                label="Saturday, 19th"
              />

              <q-chat-message
                name="Noro"
                avatar="images/nor.jpg"
                :text="['Story, story...']"
                sent
                stamp="15 minutes ago"
              />
              <q-chat-message
                name="Ker"
                avatar="images/k.jpg"
                :text="['So we met each other on Facebook early 2020, I sent Noro a friend request and Noro accepted. I was glad that she responded to my first hello because I actually thought she would ignore my chat. ']"
                stamp="14 minutes ago"
              />
              <q-chat-message
                name="Noro"
                avatar="images/nor.jpg"
                :text="['Ignore keh... lol, We started chatting on the 5th of January 2020. Our calls and chats were long. We connected well and had good chemistry even now.']"
                sent
                stamp="12 minutes ago"
              />
              <q-chat-message
                name="Ker"
                avatar="images/k.jpg"
                :text="['We met each other on the 11th of February and I was amazed at how tall she was. I told her... you are long, lol. I cant forget in a hurry the fried potatoes, Jollof rice, salad and chicken she prepared for me that day. I ate to my satisfaction and I knew we were a match. She showed me unusual kindness.']"
                stamp="11 minutes ago"
              /> 
              <q-chat-message
                name="Ker"
                avatar="images/k.jpg"
                :text="['I kept on visiting Noro, traveling to Bauchi sometimes to Jos from Gboko to see my Cinderella. On May 23rd, I popped the question and she said YES!']"
                stamp="11 minutes ago"
              /> 
              <q-chat-message
                name="Noro"
                avatar="images/nor.jpg"
                :text="['Ker and I are best of friends, we love each other a lot and we can chat for Africa, my WhatsApp is filled with chats from our numerous conversations.  We cant wait to walk down the aisle together on December 5, 2020']"
                sent
                stamp="11 minutes ago"
              />                             
                                      
            </div>
          </div>                
    </div>

<!-- Pre-Wedding Photos -->
    <div class="bg-grey-8">
        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>

        <div class="text-weight-light text-h4 text-white text-center">
          Pre-wedding Photos
        </div>

        <div class="text-center q-mb-none q-pb-none">
          <img src="images/divider.png" alt="" width="80%" >
        </div>
<!-- Pictures Arrangements -->
        <div class="row q-mx-xl text-center"> 
<!-- Column One -->           
          <div class="col-xs-12 col-sm-6 col-md-6">
            <div class="q-pb-md">
                <q-img  class="radius" src="images/pic111.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic112.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic1.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic2.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic4.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic5.jpg" :ratio="4/3" />
            </div>    

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic6.jpg" :ratio="4/3" />
            </div> 
          </div>
<!-- Column Two -->
          <div class="col-xs-12 col-sm-6 col-md-6">
            <div class="q-pb-md">
                <q-img  class="radius" src="images/pic7.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic8.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic9.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic10.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic11.jpg" :ratio="4/3" />
            </div>

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic12.jpg" :ratio="4/3" />
            </div>    

            <div class="q-pb-md">
                <q-img class="radius"  src="images/pic13.jpg" :ratio="4/3" />
            </div> 
          </div>                    
        </div>


        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>          
    </div>

<!-- Gift Registry -->
    <div class="bg-grey-4">
        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>          
        <div class="text-weight-light text-h4 text-grey-8 text-center">
          Gift Registry
        </div>
        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>

        <div class="text-grey-9 text-center q-mb-sm q-px-md">
          We are grateful in advance for all the pleasant gifts you have planned 
          to gift us with. You may wish to gift any of the items below or gift cash. 
          Again, thank you very plenty.
        </div>         
<!-- Gift Cards -->
        <div class="row justify-center q-gutter-md">
          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/cash.jpg">
            <q-card-section>
              <div class="text-grey-8">
                Cash Gift
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <a href="https://paystack.com/pay/gimkfaci50" target="_blank"><q-btn no-caps glossy rounded color="primary" icon="favorite" label="Gift This" /></a>
            </q-card-actions>
          </q-card>

          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/microwave.jpg">
            <q-card-section>
              <div class="text-grey-8">
                #50,000 - Hisense Microwave
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <a href="https://paystack.com/pay/gimkfaci50" target="_blank"><q-btn no-caps glossy rounded color="primary" icon="favorite" label="Gift This" /></a>
            </q-card-actions>
          </q-card>  

          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/gascooker.png">
            <q-card-section>
              <div class="text-grey-8">
                #130,000 - Gascooker
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <a href="https://paystack.com/pay/gimkfaci50" target="_blank"><q-btn no-caps glossy rounded color="primary" icon="favorite" label="Gift This" /></a>
            </q-card-actions>
          </q-card>  

          <q-card class="bg-grey-3" style="width: 100%; max-width: 300px;">
            <img src="images/washing.jpg">
            <q-card-section>
              <div class="text-grey-8">
                #100,000 - Washing Machine
              </div>              
            </q-card-section>
            <q-card-actions align="right">
              <a href="https://paystack.com/pay/gimkfaci50" target="_blank"><q-btn no-caps glossy rounded color="primary" icon="favorite" label="Gift This" /></a>
            </q-card-actions>
          </q-card>                      
        </div>

<!-- Appreciation -->
        <div class="text-center q-pa-md">
          Thank's for your love <br>
          We are excited to celebrate with you! <br>  
          Watch this space for our post-wedding Photo Gallery!       
        </div>

        <div class="text-center">
          <img src="images/divider.png" alt="" width="80%" >
        </div>          

<!-- Floating Button -->
      <q-page-sticky position="bottom-right" :offset="[18, 18]">
        <q-fab
          v-model="fabRight"
          autoplay
          animated
          transition-prev="slide-right"
          transition-next="slide-left"    
          swipeable
          vertical-actions-align="right"
          color="primary"
          glossy
          icon="add"
          direction="up"
        >
          <q-fab-action label-position="left" color="primary" to="/giftregistry" icon="card_giftcard" label="Gift Registry" />
          <q-fab-action label-position="left" color="primary" @click="contactus=true" icon="phone" label="Contact Us" />
        </q-fab>  
      </q-page-sticky> 

    <!-- Dialogs -->
    <q-dialog v-model="contactus">
      <ContactUs/>
    </q-dialog> 

    </div>  
  </div>
</template>

<script>
import ContactUs from '../components/Dialogs/ContactUs'

export default {

    components:{
    ContactUs
  },

  data () {
    return {    
      fabRight: false,
      contactus: false,
    // for Carousel
      slid: 'moonlove',
      navigation: true,
      navPos: 'bottom',
      slide: 1,

      topCarousel: [
        {
          id: '1',
          name: 'moonlove',
          imageUrl: '/images/pic112.jpg',
          title: '5th December, 2020',
        },
        {
          id: '2',
          name: 'lovecircle',
          imageUrl: '/images/pic2.jpg',
          title: '#NK2020',
        },
        {
          id: '3',
          name: 'lovelove',
          imageUrl: '/images/pic1.jpg',
          title: '#Soulmates',
        },
        {
          id: '4',
          name: 'loveRing',
          imageUrl: '/images/pic7.jpg',
          title: '#Forever',
        },                         
      ],      
    }
  }

}
</script>

<style scoped>

.custom-caption{
    bottom: 50px;
    text-align: center;
    padding: 12px;
    background-color: rgba(0, 0, 0, .3);
}

.radius{
  border-radius: 15px 0px 15px 0px;
  max-width: 350px;
}


/* .ruban{
    font-family:'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
} */
</style>
