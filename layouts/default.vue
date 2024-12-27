  <template>
    <div>
      <!-- Header with Banner/Intro -->
      <div :class="{'bg-white text-gray-900 pt-0 mt-0 pb-0': !isDarkMode, 'bg-gray-500 text-gray-100 pt-0 mt-0 pb-0': isDarkMode}" class="text-center pb-2">
        <div :style="isAnimationsEnabled ? { animation: 'gradientAnimation 8s ease infinite' } : {}" class="w-full flashy-banner-text pt-0 mt-0">

          <div class="logo-container">
            <img src="~/assets/img/postitu-logo2.png" alt="Post IT-U" class="logo-title" />
          </div>
          

          <h2 class="text-5xl uppercase mb-0 font-mono pt-5"><span class="text-yellow-300">PostIT</span>:U</h2>

          <h3 class="text-3xl uppercase mb-4 font-mono text-red-300 pt-2">PostCity x IT:U - Linz, You Saved the Grüngürtel,</h3>

          <h3 class="text-4xl uppercase mb-4 font-mono text-red-300 pt-2">
            <b class="highlight-background">NOW Let's Make PostCity Work for All of Us</b>
          </h3> 


          <div class="bg-gray-500 text-gray-100 text-center">
            <div :style="isAnimationsEnabled ? { animation: 'zoomEffect 30s infinite alternate' } : {}" class="w-full background-banner">
            </div>
          </div>

        </div>

        <!-- Intro -->
        <div class="max-w-3xl w-full mx-auto px-8 pt-10">
          <div class="highlight-text-intro pb-64 text-center">
          <h3 class="text-4xl uppercase mb-4 font-mono text-white-400 pt-12">What is this about/why now?</h3>
          <h5 class="text-md text-white-400">
            Now that the city <a href="https://www.nachrichten.at/politik/landespolitik/stadt-linz-zieht-bei-der-umwidmung-fuer-die-itu-die-notbremse;art383,3989606?utm_source=browser&utm_medium=push-notification&utm_campaign=cleverpush-1728293690" target="_blank">has backtracked</a> on the planned Dornach "Grüngürtel" extension, here is <b>another chance for the PostCity location, the place where the university began</b>.
          </h5>
        <!--<h3 class="text-4xl uppercase mb-4 font-mono text-red-400 pt-12">
            <i class="smaller-text text-red-400"><b>Thank you</b> to those officials involved, for listening to the people, and stopping the ecologically disastrous old plan in October 2024. </i></h3>--> 
          <h3 class="text-4xl uppercase mb-4 font-mono text-red-400 pt-12">
            <b>this initiative aims to continue the colaborative dialog</b> since we all stand to profit from doing this long-term project right</i>.
          </h3>

          <h4>Based on the original <a href="https://postuni.at">PostUni</a> idea by post:collective, this website aims to collect <b>mayoral candidate statements about Linz's PostCity as a possible location for IT:U</b>, in the run-up to the 2025 election, as well as related facts and the (political) story so far, as understdood by students IT:U's own Founding Lab.</h4>

          <p class="mb-5 text-gray-400">Art Credit (Background Banner): <b>post:collective</b> (<a href="https://postuni.at">PostUni</a>)</p>

          <h3 class="text-4xl uppercase mb-4 font-mono text-white-400 pt-12">Who are we?</h3>

          <h4>We are an unlikely grouping iterested in a sutainable, smart, relevant and promising development of the university sector in Linz that still goes together with economic prowess: we are the KHJ, the Catholic University Youth in Upper Austria, as well as IT:U Founding Lab and the 2024 Summer School cohort. <b>But above all, we are Linzer.</b> And we are students!</h4>

          <h4>Read on for more background.
          </h4>

          <!-- Box to hold toggle switches -->
          <div class="max-w-3xl w-full mx-auto px-8 pt-10">
            <h4><b>Options</b> for reading this page:</h4>
            <!-- Dark Mode Toggle Switch -->
            <div class="toggle-container">
              <label class="toggle-label">
                <input type="checkbox" v-model="isDarkMode" class="toggle-input">
                <span class="toggle-slider"></span>
              </label>
              <span>Switch to <b>Dark Mode</b></span>
            </div>

            <!-- Animations Toggle Switch -->
            <div class="toggle-container">
              <label class="toggle-label">
                <input type="checkbox" v-model="isAnimationsEnabled" class="toggle-input">
                <span class="toggle-slider"></span>
              </label>
              <span>Enable <b>(Horizontal) Animations</b></span>
            </div>

            <!-- Politics Toggle Switch -->
            <div class="toggle-container">
              <label class="toggle-label">
                <input type="checkbox" v-model="isPoliticsEnabled" class="toggle-input">
                <span class="toggle-slider"></span>
              </label>
              <span>Show <b>(Political) Information About Mayoral Candidates</b></span>
              <p>Recommended.</p>
            </div>
          </div> 
        </div> 

        <!-- Main Content -->
        <Nuxt :isDarkMode="isDarkMode" :isAnimationsEnabled="isAnimationsEnabled" :isPoliticsEnabled="isPoliticsEnabled" /> <!-- Main App/Content: Pagination Could Grab This -->

        <!--<div class="pb-64 text-center">
          <NuxtLink v-for="page in pages" :key="page" :to="page" class="underline mx-4">
            <span class="main-link" v-if="page == '/'">PostCity</span>
            <span class="secondary-link" v-else>+ {{ page }}</span>
          </NuxtLink>
        </div>-->

        <div :style="isAnimationsEnabled ? { animation: 'roll 50s infinite linear' } : {}" class="con-belt"></div>

        </div>
      </div>

      <!-- Voices  -->

      <!-- A Message from the Found Lab -->
      <!--<div class="bg-yellow text-gray-100 text-center pb-2">
        <div class="max-w-3xl w-full mx-auto px-8 pt-10">
        <h3 class="text-3xl uppercase mb-4 font-mono text-blue-300 mt-5">Now a <b>->MESSAGE<-</b> from <b>IT:U'S FIRST STUDENTS</b></h3>  

        <div class="header-box">
          <div class="info header">
            <h3>FOUNDING LAB</h3>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
          </div>
        </div>

        <div class="highlighted-text-box mb-4">
          <h3>Individual Voices from The Founding Lab</h3>
          <h4><a href="https://postuni.at/en/">Book Link Perhaps</a></h4>
          <h5>by Open!</h5>
          <p>Voice 1: TODO! JACK KONTAKT FOUNDING LAB MEMBERS</p>
          <h5>by Open!</h5>
          <p>Voice 2: TODO! JACK KONTAKT FOUNDING LAB MEMBERS</p>
        </div>

        </div>
      </div>-->

      <!-- About Us Part -->
      <div class="bg-blue text-gray-100 text-center pb-2">
        <div class="max-w-3xl w-full mx-auto px-8 pt-10">
        <h3 class="text-3xl uppercase mb-4 font-mono text-blue-300 mt-5">So <b>->WHO<-</b> are we? <b>IN DETAIL</b></h3>  

        <img src="~/assets/img/machine.jpg" alt="From the Collective:Detention Model Makers" class="w-full mb-4" />

        <p class="mb-5">Art Credit: Ars Electronica/IT:U <b>Founding Lab 2024</b></p>

        <!--<div class="header-box">
          <div class="info header">
            <h3>FOUNDING LAB</h3>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
          </div>
        </div>

        <div class="highlighted-text-box mb-4">
          <h3>Starting a University: 2023 Ars Electronica Festival Recap and the 2024/25 Perspective</h3>
          <h4><a href="https://postuni.at/en/">Book Link Perhaps</a></h4>
          <h5>by Open! Letta?</h5>
          <p>TODO! JACK KONTAKT FOUNDING LAB ODER EIGENER TEXT</p>
          <p>Group Photo?</p>
        </div>-->

        <img src="~/assets/img/Firefly-1.jpg" alt="From the Collective:Detention Model Makers" class="w-full mb-4" />

        <div class="header-box mt-5">
          <div class="info header">
            <h3>CATHOLIC UNIV. YOUTH</h3>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
          </div>
        </div>

        <div class="highlighted-text-box mb-4">
          <h3>(Re-)Thinking University-Impact - Socially, Ecologically - in Linz</h3>
          <img src="~/assets/img/profile-jack.jpg" alt="Profile Picture of Jack Heseltine" class="float-right ml-3 mb-2" />
          <h4><a href="https://www.dioezese-linz.at/institution/8228/ueberuns/khjlvorstand201617">KHJ Leadership 2024/25</a></h4>
          <h5>by Jack Heseltine</h5>
          <p class="mb-3"><strong>First and foremost, PostCity is an inspiring and unique location in Linz: whether you consider the underground train hall, the vast open spaces with the famous blue package slides, or the baffling amount of backoffices slightly frozen in time, from when there was post being processed here.</strong> Anyone who has attended the Ars Electronica Festival here, particularly the last two editions in 2023 and 2024, knows this well. Exhibits, talks, workshops — PostCity is not just a prime venue for the activities that define a university too, all conveniently situated in the heart of Linz and seamlessly connected to the outside world via the central train station — it is, in fact, a place perfectly matched with this sort of use, even in its current state, as proven by the festival’s success. That is not to say it should stay exactly as it is!</p>
          <p class="mb-3"><strong>Yet, there is another story at play here, one that recent festival visitors may have forgotten or even chosen to overlook: the homelessness and visible drug-related activities just outside the train station have long marked this area as a problem hotspot for the city.</strong> I, too, have at times felt uneasy crossing the square in front of the main entrance, positioned between the train station and PostCity. This isn't the exaggerated concern of supposedly pampered, disconnected festival-goers — it’s a very real issue, reflected in crime reports that can easily be found online.</p>
          <p class="mb-3">The Catholic University Youth believes in the power of transformative dialog within the university, striving for social and cultural relevance at every opportunity. At the same time, a <strong>core Catholic social principle is the prevention of further displacement of marginalized individuals and communities</strong> — an all-too-common consequence when high-rises filled with luxury apartments and over-priced ground-floor cafés spring up, as has been seen in the mechanics of gentrification across cities worldwide.</p>
          <p class="mb-3">Here, however, we have the chance to do something different, something more inclusive and open-ended. <strong>Motivated by the potential for social progress, the Catholic University Youth advocates for a thoughtful and socially relevant use of PostCity</strong> — one that includes housing IT-U and related educational facilities at this key location, provided the IT-U and its partners are prepared to engage with the surrounding (social) environment in a meaningful way.</p>
          <p><em>We believe that the people of IT-U are up to this challenge and express our support at this critical juncture, in the lead-up to the mayoral elections — though we do not, however, align ourselves with any established or emerging political parties.</em></p>
        </div>

        </div>
      </div>

      <!-- Our Supporters Part -->
      <!--<div class="bg-green text-gray-100 text-center pb-2">
        <div class="max-w-3xl w-full mx-auto px-8 pt-10">
        <h3 class="text-3xl uppercase mb-4 font-mono text-blue-300 mt-5"><b>->OUR SUPPORTERS<-</b></h3>  
        <div class="header-box">
          <div class="info header">
            <h3>RETTET DEN GRÜNGÜRTEL</h3>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
          </div>
        </div>

        <div class="highlighted-text-box mb-4">
          <h3>(Re-)Thinking University-Impact - Socially, Ecologically - in Linz</h3>
          <h4><a href="https://www.dioezese-linz.at/institution/8228/ueberuns/khjlvorstand201617">KHJ Leadership 2024/25</a></h4>
          <h5>by ?</h5>
          <p>2024 Fall Perspective? TODO JACK KONTAKT GRÜNGÜRTEL FÜR TEXT</p>
          <p>Group Photo? Logo?</p>
        </div>

        <h3 class="text-3xl uppercase mb-4 font-mono text-blue-300 mt-1"><b>->YOUR LOGO<- Here?</b></h3> 
        <h3 class="text-md text-white mt-3">If you would like to appear as a supporter on this website, please write to: <b>contact@postuni.at</b></h3>-->

        <!--<h3 class="text-3xl uppercase mb-4 font-mono text-blue-300 mt-4"><b>->SHARING IS CARING<-!</b></h3> 
        <h3 class="text-md text-white mt-3">Would you like to <b>bring attention to this initative</b> on your channels?</h3>

        <h3 class="text-md text-white mt-4"><a href="">Copy the still image</a> or this code for the animated version:</h3>-->

        <!--</div>
      </div>-->

      <!-- Footer (1) End-Notes Section -->
      <div class="bg-black text-gray-100 text-center pb-2">
        <div class="max-w-3xl w-full mx-auto px-8 pt-10">

        <div class="header-box">
          <div class="summary header">
            <h3>THE NEXT STEPS</h3>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
          </div>
        </div>

        <div class="text-box mb-2 endnotes">
          <h3>Thank You for Reading This Far!</h3>
          <p>You see, we care about this stuff. Are you getting this idea? If yes, <b>we hope to count on your support: make your voice heard at January 12th Mayoral election</b> by voting for a candidate prioritizing this important project at this excellent location.</p>
          <p class="mt-4">For our part, <b>we will continue to publicize the story and related efforts, exercising a democratic, soft counter-power to the politics- and business-as-usual leading to bad decisions like closing the Green Belt (Grüngürtel)</b>.</p>
          
          <h2 class="text-5xl uppercase font-mono text-red-400 mt-10"><b>Next stop: Linz, PostIT:U!</b></h2>

          <img src="~/assets/img/linienplan.jpg" alt="From the Collective:Detention Model Makers" class="w-full mb-0 mt-10" />
        </div>

        <div :style="isAnimationsEnabled ? { animation: 'roll 50s infinite linear' } : {}" class="con-belt"></div>

        <img src="~/assets/img/post-city-no-bg.png" alt="PostUni Logo" width="100" class="mb-5 mt-5 center logo" />

        </div>

        <p style="display: inline-flex; align-items: center;">
          <a href="https://heseltime.github.io/"><img src="~/assets/img/heseltime-favicon-32x32.png" alt="heseltime Logo" width="16" style="margin-right: 5px;" /></a>
          <span><a href="https://heseltime.github.io/"><b>heseltime</b></a>: website design, deployment and content except where indicated. <b style="text-decoration: underline;">Based on the original <a href="https://postuni.at">postuni.at</a>-concept by Collective:Detention</b></span>
        </p>

      </div>

      <!-- <div class="bg-white-footer text-gray-100 text-center pb-2">
        <div class="max-w-3xl w-full mx-auto px-8 pt-2 flex justify-between items-center">
          <div class="logo-container-2  ">
            <img src="~/assets/img/postuni-old-logo.jpg" alt="Logo Original Postuni" width="100" class="logo-left">
          </div>

          <div class="footer-links">
            <a href="#project" class="footer-link">Project</a>
            <a href="#planning" class="footer-link">Planning</a>
            <a href="#research" class="footer-link">Research</a>
            <a href="#component-scavenger-hunt" class="footer-link">Component Scavenger Hunt</a>
            <a href="#contact" class="footer-link">Contact</a>
          </div>
        </div>-->
      </div>

    </div>
  </template>

  <script>
  import Nuxt from '~/pages/index.vue';
  export default {
    components: {
      Nuxt
    },
    data () {
      return {
        isDarkMode: false, // Default is light mode
        isAnimationsEnabled: true,   // State to toggle animations
        isPoliticsEnabled: true, // State to toggle political content
      };
    },
    mounted () {
      window.addEventListener('resize', this.handleResize)
      this.handleResize()
    },
    methods: {
      toggleDarkMode() {
        this.isDarkMode = !this.isDarkMode;
      },
      handleResize () {
        this.triggerTop = this.offset * window.innerHeight
      }
    }
  }
  </script>

  <style>
  body {
    min-height: 100vh;
  }

  .logo-container {
    display: flex;
    justify-content: center; /* Center horizontally */
    align-items: center;     /* Center vertically */
    height: 200px;           /* Adjust height to create enough space */
  }

  .logo-title {
    width: 200px;             /* Set the width of the image */
    display: block;           /* Ensure the image is treated as a block-level element */
    margin: 0 auto;           /* Center the image horizontally */
  }

  .background-banner {
    background-image: url('@/assets/img/postuni.jpg');
    background-size: cover;
    background-position: center;
    height: 650px;
    width: 100vw; /* Ensures the background covers the full viewport width */
    position: relative; /* Set to relative */
    overflow: hidden;
    z-index: 0; /* Ensure the background is behind */
  }

  /* Zoom effect keyframes (horizontal only) */
  @keyframes zoomEffect {
    0% {
      transform: scaleX(1); /* Initial size */
    }
    100% {
      transform: scaleX(1.1); /* Zoom in horizontally only */
    }
  }

  .text-center {
    text-align: center;
  }

  .main-link {
    font-size: 2em;
  }

  .secondary-link {
    color: #bbb;
    text-decoration: none;
  }

  .highlight-text-intro {
    background-color: rgba(0, 0, 0, 0.6); /* Semi-transparent dark overlay */
    padding: 3em 2em;
    border-radius: 8px;
    max-width: 800px;
    margin: 0 auto;
    color: #e0e6ed;
    text-align: left;
    position: relative;
    z-index: 10; /* Ensure the text is in front of the background */
  }

  .highlight-text-intro h3 {
    color: #ffffff;
    text-shadow: 1px 1px 4px rgba(0, 0, 0, 0.4);
    margin-bottom: 1.5em; /* Additional bottom margin for spacing */
  }

  .highlight-text-intro h4,
  .highlight-text-intro h5 {
    font-weight: 300;
    color: #e0e6ed;
    margin-bottom: 1.2em; /* Additional spacing between elements */
  }

  .highlight-text-intro a {
    color: #00bcd4;
    font-weight: bold;
    text-decoration: underline;
    transition: color 0.3s ease;
  }

  .highlight-text-intro a:hover {
    color: #0097a7;
  }

  .highlight-text-intro b {
    font-weight: bold;
    color: #ffffff;
  }

  .flashy-banner-text {
    text-align: center;
    background: linear-gradient(135deg, #ff6b6b, #ffd93d, #1dd3b0, #0078d7); /* Gradient background */
    background-size: 300% 300%;
    height: 600px;
  }

  .flashy-banner-text h3, .flashy-banner-text h2 {
    color: #ffffff;
    font-weight: bold;
    text-transform: uppercase;
    text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.4); /* Shadow for depth */
  }

  .flashy-banner-text h3 {
    font-size: 3rem;
    margin-bottom: 0.5em;
  }

  .flashy-banner-text h2 {
      font-size: 4.5rem;
      font-weight: 900;
      margin-bottom: 1em;
    }

    /* Gradient animation */
    @keyframes gradientAnimation {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

  .highlight-background {
    background-color: rgba(255, 255, 0, 0.5); /* Yellow semi-transparent background */
    padding: 0.2em 0.4em;
    border-radius: 4px;
  }

  .smaller-text {
    font-size: 0.75em; /* Adjust as needed */
    vertical-align: middle;
  }

  .cta-button {
    display: inline-flex; /* Ensure text and SVG are flex items */
    align-items: center; /* Align text and logo vertically */
    justify-content: center; /* Center both the text and the logo horizontally */
    background: linear-gradient(45deg, #32e0f4, #29b0cc); /* Gradient for a glossy look */
    color: #ffffff !important; /* Force the text color to white */
    padding: 1em; /* Padding around the button */
    font-size: 1.5rem;
    font-weight: bold;
    text-transform: uppercase;
    border: none;
    border-radius: 8px;
    cursor: pointer;
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3), inset 0px 2px 4px rgba(255, 255, 255, 0.3); /* 3D effect */
    width: 100%; /* Full width of container */
    max-width: 800px; /* Limits width on larger screens */
    margin: 1.5em auto 0; /* Center-align and space from other elements */
    text-decoration: none !important;
    transition: background 0.3s ease, transform 0.2s ease;
    gap: 0.2em; /* Adds space between the logo and the text */
    position: relative; /* Required for the :before pseudo-element */
  }

  .cta-button:hover {
    color: #fff !important; /* Ensure text stays white on hover */
    background: linear-gradient(45deg, #32e0f4, #2cb4cc); /* Darker gradient on hover */
    transform: translateY(-3px); /* Lift effect on hover */
  }

  .cta-button:active {
    transform: translateY(1px); /* Slightly press down on click */
  }

  .cta-button:before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    border-radius: 8px;
    background: rgba(255, 255, 255, 0.2);
    z-index: 1;
    opacity: 0;
    transition: opacity 0.3s ease;
  }

  .cta-button:hover:before {
    opacity: 1; /* Adds an extra layer for a glossier effect on hover */
  }

  .cta-button svg {
    vertical-align: middle;
    right: 0;
  }

  .bg-blue {
    background-color: #2596be;
  }

  .bg-yellow {
    background-color: #f8dc6c;
  }

  .bg-green {
    background-color: #d0d410;
  }

  .info-box {
    display: flex;
    align-items: flex-start;
    background-color: #655c5c; /* Dark gray background */
    border: 2px solid #ddd; /* Subtle border */
    border-radius: 8px;
    padding: 20px;
    margin-top: 20px;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1); /* Subtle shadow for depth */
  }

  .info-symbol {
    font-size: 2rem; /* Size of the info symbol */
    margin-right: 15px;
    color: #2596be; /* Optional: Info color (blue) */
  }

  .info-text {
    flex-grow: 1;
  }

  .info-box a {
    color: #2596be; /* Matching color for links */
    text-decoration: underline;
  }

  .info-box a:hover {
    color: #0077a8; /* Darker blue on hover */
  }

  .logo {
      display: block;
      margin-left: auto;
      margin-right: auto;
  }

  .bg-white-footer {
    background-color: #fff;
    color: #333;
    padding: 1.5em 0;
  }

  .logo-container-2 {
    flex-shrink: 0; /* Prevents the logo from shrinking */
  }

  .logo-left {
    display: block;
    margin-right: 15px; /* Adds spacing to the right of the logo */
  }

  .footer-links {
    display: flex;
    justify-content: center;
    gap: 1.5em; /* Spacing between links */
  }

  .footer-link {
    text-decoration: none;
    color: #333; /* Link color */
    font-weight: bold;
    font-size: 1rem;
    transition: color 0.3s ease;
  }

  .footer-link:hover {
    color: #0077a8; /* Hover color */
  }

  /* Base styles */
  .light-mode {
    background-color: white;
    color: black;
  }

  .dark-mode {
    background-color: black;
    color: white;
  }

  /* Container for the toggles */
  .toggle-container {
    display: flex;
    align-items: center;
    justify-content: flex-start; /* Align to the left */
    margin-bottom: 1rem;
  }

  .toggle-label {
    position: relative;
    display: inline-block;
    width: 50px;
    height: 26px;
    margin-right: 0.5rem;
  }

  .toggle-input {
    opacity: 0;
    width: 0;
    height: 0;
  }

  .toggle-slider {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: #ccc;
    border-radius: 34px;
    cursor: pointer;
    transition: 0.4s;
  }

  .toggle-slider:before {
    position: absolute;
    content: "";
    height: 20px;
    width: 20px;
    left: 4px;
    bottom: 3px;
    background-color: white;
    border-radius: 50%;
    transition: 0.4s;
  }

  .toggle-input:checked + .toggle-slider {
    background-color: #2196F3;
  }

  .toggle-input:checked + .toggle-slider:before {
    transform: translateX(24px);
  }



  </style>