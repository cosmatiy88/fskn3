<template>


<div>


  <!-- banner section -->
  <section id="home" class="banner">
      <div id="banner-bg-effect" class="banner-effect"></div>
      <div class="container">
          <div class="row align-items-center">
              <div class="col-lg-7 col-md-12 col-sm-12 order-lg-first mt-lg-0 custom-margin">
                  <h1 class="mb-4 title title-size">

                    <strong>Межрегиональная общественная организация «Комитет по противодействию коррупции и содействию общественной безопасности»</strong>
                  </h1>
                  <div class="mt-5">
<!--             <nuxt-link class="btn btn-primary btn-style mr-2 text-white" to="/about">Read More </nuxt-link>-->
<!--          <nuxt-link class="btn btn-outline btn-outline-style text-white custom-hover" to="/services">Our Services </nuxt-link>-->
                  </div>
              </div>
              <div class="col-lg-5 col-md-12 col-sm-12 order-first text-lg-left text-center">
                  <div>




                  </div>
              </div>
          </div>
      </div>
  </section>
  <!-- //banner section -->

  <!-- home page about -->
  <section class="w3l-about section-bg-color text-white">
      <div class="container">
          <div class="row about-content">
              <div class="col-lg-6 info mb-lg-0 mb-sm-5 mb-4 align-center">
                  <h6 class="title">Межрегиональная общественная организация «Комитет по противодействию коррупции и содействию общественной безопасности» учреждена физическими лицами и зарегистрирована в Министерстве Юстиции РФ за основным государственным номером 1177700006098 от 11 апреля 2017 г.
                  </h6>
                  <h6>Центральный Совет является Высшим коллегиальным органом Комитета.</h6>
                  <p class="mt-md-4 mt-3 mb-0"> Председатель Центрального Совета — Марина Михайловна Галюченко.
                    Председатель организации — Малик Кадырович (Абдулзагир Абдулкадырович) Тавлуев. </strong>
                    У сотрудников организации накоплен большой опыт общественной деятельности и основной задачей своей работы члены МОО «Комитет по противодействию коррупции и содействию общественной безопасности» является противодействие коррупции, как опасному явлению, которое существенно замедляет экономический рост и негативно влияет на социальное развитие государства, поддержка инициатив гражданского общества, государственных и административный органов, направленных на созидание и оздоровление нашего общества; на продвижение идей гуманности и поддержку духовных ценностей нашего общества, на создание благоприятного межэтнического и межконфессионального фона для общения между обычными гражданами нашей страны.

                    В нашей организации ведется прием граждан и работает телефон горячей линии — 8-800-200-87-15</p>
              </div>
              <div class="col-lg-6">
                  <img src="@/assets/images/cohotek-web-search.png" class="img-fluid img-shadow"
                  alt="cohotek IT web development company">
              </div>
          </div>
      </div>
  </section>
  <!-- //home page about -->

  <!-- home page service grids -->
  <section id="services" class="bg-light">
    <div class="container">
<!--      <div class="row align-items-center">-->
<!--        <div class="col-lg-8 offset-lg-2 col-md-12 col-sm-12">-->
<!--          <h4 class="section-title">IT Problems Begone</h4>-->
<!--          <p class="text-center">We are a full-stack web development company offering a full-->
<!--            spectrum of services linked to the internet.-->
<!--              Hire us, and in a short period of time, you will notice a significant boost in your revenue and number of clients.</p>-->
<!--        </div>-->
<!--      </div>-->
<!--      <div class="row mt-lg-5">-->
<!--        <div class="col-lg-4 col-md-6 col-sm-12">-->
<!--          <div class="box-wrap">-->
<!--            <div class="icon">-->
<!--              <span class="fa fa-briefcase"></span>-->
<!--            </div>-->
<!--            <h4><a href="#url">Business Services</a></h4>-->
<!--            <p>We are a one-stop IT solutions company with a difference,-->
<!--              we want to change the world by the way we do business.</p>-->
<!--          </div>-->
<!--        </div>-->
<!--        <div class="col-lg-4 col-md-6 col-sm-12">-->
<!--          <div class="box-wrap">-->
<!--            <div class="icon">-->
<!--              <span class="fa fa-shield"></span>-->
<!--            </div>-->
<!--            <h4><a href="#url">Product Consulting</a></h4>-->
<!--            <p>A team of dedicated Product Consulting Services experts-->
<!--               provides solutions to meet your management challenges.</p>-->
<!--          </div>-->
<!--        </div>-->

<!--        <div class="col-lg-4 col-md-6 col-sm-12">-->
<!--          <div class="box-wrap">-->
<!--            <div class="icon">-->
<!--              <span class="fa fa-globe"></span>-->
<!--            </div>-->
<!--            <h4><a href="#url">Projects Worldwide</a></h4>-->
<!--            <p>We are opened to a market of vast populations that could be interested all around the world.</p>-->
<!--          </div>-->
<!--        </div>-->
<!--      </div>-->
    </div>
  </section>
  <!-- //home page service grids -->

  <!-- testimonials section -->

  <!--//testimonials section -->

  <!-- stats section -->

  <!-- //homepage blog grids -->


</div>



</template>

<script>
//import Logo from '~/components/Logo.vue'
//import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {

  head(){
    return {
      title: "Комитет по противодействию коррупции",
      meta:[

          { hid: 'description6', name: 'description', content: 'Cohotek IT company in Lagos Nigeria delivers innovative custom web designs, web development and digital marketing services.' },
          { name: 'keywords', content: 'web development in lagos, digital marketing, seo, cohotek, it company, it firm, website, web design, web application, web, web development, wordpress, php, html, web instructor, developer, porfolio, henry onyemaobi,website instructor, website teacher' },

      ]
    }
  },

  data () {

    return {
    projectCount: '-',
    posts:[],
    loading: true,
    err: false,
    }

  },

  methods: {

  getProjectCount(){
      fetch('https://cohotekapi.getfoods.ng/api/project-count', {
      method: 'GET',
      headers: {
        'Content-Type': 'application/json',
        'X-Authorization': 'w69D58JnTvtUCH3KHcfhSGNIO7NtLuJEAF7ixJDwSHCGiTpdLUWdhvROVWt8TaUf'
      }
    })
      .then(res => res.json())
      .then(res=>{
        this.projectCount = res;
        console.log(res)
      })
      .catch(error =>{
        console.log(error)
        this.projectCount = '-';
          })
  },
  //method end


  getPosts(){
      fetch('https://cohotekapi.getfoods.ng/api/posts', {
      method: 'GET',
      headers: {
        'Content-Type': 'application/json',
        'X-Authorization': 'w69D58JnTvtUCH3KHcfhSGNIO7NtLuJEAF7ixJDwSHCGiTpdLUWdhvROVWt8TaUf'
      }
    })
      .then(res => res.json())
      .then(res=>{
        this.posts = res.data;
        console.log(this.posts)
        this.loading = false
      })
      .catch(error =>{
        console.log(error)
        this.loading = false
        this.err = true
          })
  },
  //method end

  },

  mounted() {

  // get project count
  this.getProjectCount()

  //get blog posts
  this.getPosts()

      /*===================================*
	02. BACKGROUND ANIMATION JS
	*===================================*/

  var $particles_js = $("#banner-bg-effect");
  // if ($particles_js.length > 0) {
  //   particlesJS(
  //     "banner-bg-effect",
  //     // Update your personal code.
  //     {
  //       particles: {
  //         number: {
  //           value: 80,
  //           density: {
  //             enable: true,
  //             value_area: 800
  //           }
  //         },
  //         color: {
  //           value: "#ffffff"
  //         },
  //         shape: {
  //           type: "circle",
  //           stroke: {
  //             width: 0,
  //             color: "#ffffff"
  //           },
  //           polygon: {
  //             nb_sides: 5
  //           },
  //           image: {
  //             src: "img/github.svg",
  //             width: 100,
  //             height: 100
  //           }
  //         },
  //         opacity: {
  //           value: 0.4,
  //           random: false,
  //           anim: {
  //             enable: false,
  //             speed: 1,
  //             opacity_min: 0.5,
  //             sync: false
  //           }
  //         },
  //         size: {
  //           value: 3,
  //           random: true,
  //           anim: {
  //             enable: false,
  //             speed: 20,
  //             size_min: 0.2,
  //             sync: false
  //           }
  //         },
  //         line_linked: {
  //           enable: true,
  //           distance: 150,
  //           color: "#ffffff",
  //           opacity: 0.2,
  //           width: 1
  //         },
  //         move: {
  //           enable: true,
  //           speed: 6,
  //           direction: "none",
  //           random: false,
  //           straight: false,
  //           out_mode: "out",
  //           bounce: false,
  //           attract: {
  //             enable: false,
  //             rotateX: 600,
  //             rotateY: 1200
  //           }
  //         }
  //       },
  //       interactivity: {
  //         detect_on: "canvas",
  //         events: {
  //           onhover: {
  //             enable: false,
  //             mode: "repulse"
  //           },
  //           onclick: {
  //             enable: false,
  //             mode: "push"
  //           },
  //           resize: true
  //         },
  //         modes: {
  //           grab: {
  //             distance: 400,
  //             line_linked: {
  //               opacity: 1
  //             }
  //           },
  //           bubble: {
  //             distance: 400,
  //             size: 20,
  //             duration: 2,
  //             opacity: 1,
  //             speed: 3
  //           },
  //           repulse: {
  //             distance: 200,
  //             duration: 0.4
  //           },
  //           push: {
  //             particles_nb: 4
  //           },
  //           remove: {
  //             particles_nb: 2
  //           }
  //         }
  //       },
  //       retina_detect: true
  //     }
  //   );
  // }
    /*===================================*
	02. BACKGROUND ANIMATION JS
  *===================================*/

     /*===================================*
	Owl carousel
	*===================================*/

  $(document).ready(function () {
    var owl = $('.owl-carousel');
    owl.owlCarousel({
      margin: 10,
      nav: true,
      loop: false,
      responsive: {
        0: {
          items: 1
        },
        767: {
          items: 2
        },
        1000: {
          items: 3
        }
      }
    })
  })

   /*===================================*
	Owl carousel
  *===================================*/

  //collapse nav on component load
  $('#navbarNav').hide('fade');

},

  components: {
  //  Logo,
  //  VuetifyLogo
  }
}
</script>
