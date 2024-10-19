<template>
  <div>

    <div> 

      <div class="con-belt"></div>

      <div class="banner">
        <img src="~/assets/img/plants-banner.png" alt="PostCity Banner" />	
      </div>

      <h3 class="text-4xl uppercase mb-4 font-mono text-white-400">Transforming Infrastructure</h3>

      <h4 class="text-md text-gray-300 mt-0 mb-5">This website tells a story, in pictures, of a spectacular piece of <b>old infrastructure</b>, and <b>what it could become for the new university in Linz</b>.</h4>
      
      <div class="header-box">
        <div class="intro header">
          <h3>THE FACTS</h3>
          <div class="arrow-down"></div>
          <div class="arrow-down"></div>
          <div class="arrow-down"></div>
        </div>
      </div>
      
      <div class="highlighted-text-box-blue mb-4">
          <img src="~/assets/img/itu-spaceship.webp" alt="IT:U" width="120" style="float: right;"/>
          <h3>What is the Interdisciplinary Transformation University Austria?</h3>
          <p>
              The <a href="https://it-u.at/en/" target="_blank">Interdisciplinary Transformation University Austria (IT:U)</a> is Austria’s first interdisciplinary university, located in Linz, and dedicated to merging technology, hands-on learning, and global problem-solving. IT:U offers a project-based, inclusive approach to education, where students from diverse backgrounds apply technologies like AI and robotics to tackle real-world challenges.
          </p>
          <p>
              In some ways, because it was launched by politicians at both the state and federal levels, <b>it is like an alien space ship that has come to land in Linz: this is an opportunity</b>, for sure, and we are talking friendly aliens 👽 we think at least ❤️.
          </p>
          <h3 class="text-4xl uppercase mb-4 font-mono text-white-400 pt-12">From a City and Citizen's Perspective, so much Seems Clear: IT:U Needs to Be In the City-Center to Fulfill Its Mandate</h3>
          <p>
              As an institution centered on interdisciplinary research, <b>IT:U is determined to demonstrate that excellent science can be transformed into innovative products, services, and social advancements</b>. With its unique mission, IT:U <b>aims to empower students, scientists, and regional networks to drive transformative impact across Linz and beyond</b>.
          </p>

          <h3 class="text-4xl uppercase mb-4 font-mono text-white-400 pt-12">The University Is Called IT:U</h3>
          <h2 class="glossy-bold-black-h2">IT:U x PostCity Is <span class="neon-flicker">PostUni</span></h2>

      </div>

      <div class="full">
        <img src="~/assets/img/orange2_sonia_litwin_ccby.png" alt="Orange Wall" class="" />	
        <div class="con-belt"></div>
      </div>

      <h4 class="text-2xl uppercase mb-4 font-mono text-blue-300">Let's <b>go into</b> PostCity!</h4>

      <h3 class="text-3xl uppercase mb-4 font-mono text-blue-300">Why IT-U at PostCity <b>->NOW<-</b>? <b>IN DETAIL</b></h3>

      <div
        class="graphic sticky top-0 mt-20 flex items-center justify-center text-8xl"
      >
        <!--{{ activeStepIdSticky }}-->
        <img src="~/assets/img/cnv-blt-vrt.png" alt="Conveyor Belt" class="bg-img" />	
      </div>

      <Scrollama
        :offset="0.6"
        class="relative"
        @step-enter="stepEnterHandlerSticky"
      >
      <div
        v-for="step in stepsSticky"
        :key="step.id"
        :data-step-id="step.id"
        class="cnv-blt-1 step my-64 h-auto w-auto mx-auto flex items-center justify-between p-4 text-4xl uppercase mb-4 font-mono"
        @step-enter="stepEnterHandlerSticky"

      >
      <div class="hover-container">
          <img
            :src="step.image"
            alt="Main Image"
            class="main-image"
          />
          <div class="svg-glove">
            <!-- SVG of a glove/hand -->
            <svg viewBox="0 0 100 50" xmlns="http://www.w3.org/2000/svg" class="glove-shape">
              <!-- You can use a path or a shape resembling a glove or hand -->
              <path d="M10 10 L30 10 C40 10, 50 20, 50 30 C50 40, 40 50, 30 50 L10 50 Z" fill="#333" />
            </svg>
          </div>
          <div class="hover-box">
            <span class="text-9xl text-gray-600">{{ step.id }}</span>
            <p class="hover-description">{{ step.text }}</p>
          </div>
        </div>
      </div>

      </Scrollama>

    </div>

    <h3 class="text-3xl uppercase mb-4 font-mono text-blue-300 mt-2">So Why <b>->ARE<-</b> Decision Makers Like This About It?</h3>

    <!-- Ref. Once-In-A-Lifetime Oppt: Shrugging Guy Yellow Here, Also Pick Up Gloves Style -->
    <img src="~/assets/img/shrug.gif" alt="PostCity City Model" class="" />

    <h4>Where many people <b>across party-lines</b> are starting to see an opportunity, it sound like our politician-leaders see expensive private real estate development and a shopping mall thrown in, leading Linz down the road of <b>not just the ordinary and bland, but laying the groundwork for an undesirable urban social development in the century to come</b>.</h4>

    <h3 class="text-4xl uppercase mb-4 font-mono text-red-400">
      <i class="smaller-text text-red-400">We are convinced: <b>Linz can do better than business-as-usual here</b>.</i>
    </h3>

    <div class="header-box">
      <div class="info header">
        <h3>THE IDEA</h3>
        <div class="arrow-down"></div>
        <div class="arrow-down"></div>
        <div class="arrow-down"></div>
      </div>
    </div>
    
    <div class="highlighted-text-box mb-4">
      <h3>The Original Idea, Relevant Once Again</h3>
      <h4><a href="https://postuni.at/en/">postUNI - post:growth | post:operative | post:position</a></h4>
      <h5>by Lisa Ackerl, Daniel Schöngruber, Marco Thaller</h5>
      <p>Underused facilities and institutions in Linz like the postal distribution center PostCity, but also the slaughterhouse, or the Nestlé site are ready for new, versatile uses, which could be implemented in a climate- and environmentally-friendly manner within existing structures. Universities, along with their buildings and spaces, are essential, identity-shaping institutions within cities. Through students, educators, and infrastructure, they have the power to activate entire neighborhoods socially and economically as places to live and work. Over 26,000 people study in Linz, with around 3,000 more expected to join IT:U.
        To fulfill the societal mission of a university, its impact should not dissipate on the outskirts of the city but rather be integrated into the urban fabric, enhancing the city’s social and economic potential.</p>
      <img src="~/assets/img/city-model-no-bg.png" alt="PostCity City Model" class="" />
    </div>


    <div class="full">
      <img src="~/assets/img/RoboticsTopic_sonia_litwin_ccby.png" alt="Orange Wall" class="" />	
      <div class="con-belt"></div>
    </div>

    <div class="highlighted-text-box-yellow mb-4">
        <h3>What Is Special About PostCity?</h3>
        <h4>See Also: <a href="https://ars.electronica.art/aeblog/en/2023/04/20/once-again-in-postcity/">Ars Electronica Blog Article "Once Again In PostCity"</a></h4>
        <h5>by Katia Kreuzhuber</h5>
        <p>
          <i>With 80,000 square meters usable space spread over several levels, a 4,000-meter long parcel distribution facility, a storage unit for 10,000 packages, an entire battery of 12-meter high spiral chutes, and a rail track hall that is around 240 meters long made for both incoming and outgoing railways, the post distribution center that was abandoned in 2014 offers almost limitless opportunities for artistic stagings by Ars Electronica.</i>
        </p>
        <h3 class="text-3xl uppercase mb-4 font-mono text-blue-300 mt-2">PostCity Is Just <b>->AN INSPIRING PLACE<-</b>: <b>Most Visitors to the Ars Electronica Festivals 2023 and 2024 Agree</b></h3>
        <p><b>Endless open spaces, magical affordances like the postal slides, labarynthine corridors invite to play and to explore</b>: people do fall in love with this space itself and the fit for the insitution IT:U aims to be is apparent. More so, <b>we believe IT:U needs a space like PostCity to achieve its mission</b>.</p>
        <div style="position: relative; padding-bottom: 56.25%; height: 0; max-width: 100%; overflow: hidden;" class="mt-3">
            <iframe 
                src="https://www.youtube.com/embed/HmN03TQDCQo?start=14" 
                title="YouTube video player" 
                style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
                frameborder="0" 
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                allowfullscreen>
            </iframe>
        </div>
    </div>

    <h4 class="text-md text-gray-300 mt-0 mb-5">So now in <b>2024</b>, going into 2025, let us review ...</h4>

    <div class="header-box">
      <div class="info header">
        <h3>THE STORY SO FAR</h3>
        <div class="arrow-down"></div>
        <div class="arrow-down"></div>
        <div class="arrow-down"></div>
      </div>
    </div>

    <div class="flex mb-8"> 

      <div
        class="graphic flex-1 sticky top-0 bg-gray-300 border border-black mt-20 flex items-center justify-center text-8xl"
      >
        {{ activeStepIdSticky2 }}
      </div>
      <Scrollama
        :offset="0.6"
        class="flex-1"
        @step-enter="stepEnterHandlerSticky2"
      >
        <div
          v-for="step in stepsSticky2"
          :key="step.id"
          :data-step-id="step.id"
          class="my-64 h-48 w-48 mx-auto bg-yellow-300 border border-black flex justify-center items-center"
          @step-enter="stepEnterHandlerSticky2"
        >
          Discipline {{ step.id }}
        </div>
      </Scrollama>
    </div>

    <div class="header-box-yellow">
      <div class="intro header">
        <h3>THE VISION</h3>
        <div class="arrow-down"></div>
        <div class="arrow-down"></div>
        <div class="arrow-down"></div>
      </div>
    </div>

    <div class="text-box mb-4">
      <h3>Make It <span class="color-yellow">Yellow!</span></h3>
      <p class="color-black">You can take the yellow in the following designs to be the manifold spaces for creative transformation, aligned with the new Interdisciplinary Transformation University's mandate.</p> 
      <h3 class="text-3xl uppercase mb-4 font-mono text-blue-300 mt-2">Yes, <b>->don't<-</b> take this literally.</h3>
      <p class="mt-2">The university itself does not need to be yellow, we would agree.</p>
    </div>

    <Scrollama
        :offset="0.6"
        @step-enter="stepEnterHandler"
        @step-exit="stepExitHandler"
      >
        <div
          v-for="step in steps"
          :key="step.id"
          :data-step-id="step.id"
          class="my-32 flex justify-center items-center"
        >
          <img :src="step.image" :alt="step.id" class="topic-group-steps" />
        </div>
    </Scrollama>

    <div class="image-container">
      <h3 class="glossy-heading text-3xl uppercase mb-4 font-mono text-blue-300 mt-5 center">Some <b>->Q&A<-</b></h3>  

      <p class="text-box-inside">
        Are these designs final?
      </p>

      <p class="text-box-inside">
        No, they are one of <b>many options for a transformational opportunity in Linz</b>, where this transformation occurs in the dimensions Social Change, Ecology and Climate, Public Spaces and Transit, Global Communication, and City Politics.
      </p>

      <p class="text-box-inside">
        Why would this amazing location be used for anything but a truly transformational project, or this university be put at an ordinary location? (Not to say a green field.) In other words, what is the reasoning for not doing exactly this, which does somehow seem pretty obvious?
      </p>

      <p class="text-box-inside">
        A lot of people have been wondering this and now a collective of groups is taking action: fact is, the <b>decisions so far have been happening in the background</b>, probably driven by business-only (and business-as-usual) and certainly a non-participatory-democracy mindset. We want to change this and present a concept that is truly transformational and inclusive, in fact coming directly from students and concerned citizens of Linz.
      </p>

      <p class="text-box-inside">
        And since this has been in the news: What about Wels and Steyr?
      </p>

      <p class="text-box-inside">
        Apart from the fact that <b>Linz is the IT capital of Upper Austria</b>, aligning with the academic focus of this university, along with the fact that <b>Linz is the main university city of Upper Austria and the interdisciplinary orientation of this university would suggest an exchange with the other universities</b>, with the original decision to place the university in Linz <b>a whole cohort of staff, professors and now students have already started a new part of their life in Linz</b>, which makes a fundamental change of location like this very difficult and potentially damaging.
      </p>

      <p class="text-box-inside">
        So what <i>are</i> the people directly involved saying?
      </p>

      <p class="text-box-inside">
        It is important to note that the content of this website is not a statement from the IT:U, who have not issued a statement in any other venue so far, but does reflect the <b>voice of various groups in the vicinity of the project: starting with the very first students at the university</b>!
      </p>

      <div class="arrows-container">
        <div class="arrow-down-2"></div>
        <div class="arrow-down-2"></div>
        <div class="arrow-down-2"></div>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  data () {
    return {
      steps: [{ id: '1', image: require('../assets/img/postUNI@daniel_schöngruber_1.jpg') },
      { id: '2', image: require('../assets/img/plan_1.png') },
      { id: '3', image: require('../assets/img/plan_2.png') }
      ],
      imageReplacement: require('../assets/img/postUNI@daniel_schöngruber_2.png'),
      stepsSticky: [
        { id: '75', text: 'students founded the university here', image: require('../assets/img/spectacular.png') }, 
        { id: '7000+', text: 'signatures against closing the Green Belt' }, 
        { id: '7', text: 'Mayoral Candidates in 2024/25' }, 
        { id: '1', text: 'university/once-in-a-lifetime' }
      ],
      stepsSticky2: [{ id: 'I' }, { id: 'II' }, { id: 'III' }, { id: 'IV' }],
      activeStepId: null,
      activeStepIdSticky: 'A',
      activeStepIdSticky2: 'I'
    }
  },
  methods: {
    stepEnterHandler({ element }) {
      const stepId = element.dataset.stepId;
      this.activeStepId = stepId;
      if (stepId === '1') {
        const stepIndex = this.steps.findIndex(step => step.id === '1');
        if (stepIndex !== -1) {
          this.steps[stepIndex].image = this.imageReplacement;
        }
      }
    },
    stepEnterHandlerSticky ({ element, direction, index }) {
      console.log('step-enter', { element, direction, index })
      this.activeStepIdSticky = element.dataset.stepId
    },
    stepEnterHandlerSticky2 ({ element, direction, index }) {
      console.log('step-enter', { element, direction, index })
      this.activeStepIdSticky2 = element.dataset.stepId
    },
    stepExitHandler({ element }) {
      const stepId = element.dataset.stepId;
      if (stepId === '1') {
        // Optionally reset the image when the step exits
        const stepIndex = this.steps.findIndex(step => step.id === '1');
        if (stepIndex !== -1) {
          this.steps[stepIndex].image = require('../assets/img/postUNI@daniel_schöngruber_1.jpg');
        }
      }
      this.activeStepId = null;
    }
  }
}
</script>

<style>
.graphic {
  height: 80vh;
}

.full {
  display: block;
  width: 100%;
  height: 100%;
}

.bg-img {
  width: 245px;
}

.header {
  background-color: #fff;
  color: #000;
  font-weight: bold;
  font-size: 3em;
  padding: 10px;

  border: 10px solid #000
}

  .header-box {
    background-color: #fff;
    padding: 10px;
    margin-bottom: 20px;
  }

  .header-box-yellow {
    background: linear-gradient(135deg, #ff6b6b, #ffd93d, #1dd3b0, #0078d7); /* Neon gradient background */
    border: 5px solid #fde047; /* Keeps the yellow border */
    border-radius: 8px;
    padding: 20px;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2); /* Adds subtle shadow */
    transition: background 0.5s ease-in-out;
  }

.text-box {
  margin: 20px 0;
}

  .text-box h3 {
    font-size: 2em;
    margin-bottom: 10px;
    text-align: left;
    font-weight: bold;
    color: #ed820e;
  }

  .text-box p {
    font-size: 1.2em;
    text-align: left;
  }

.arrow-down {
  width: 0; 
  height: 0; 
  border-left: 20px solid transparent;
  border-right: 20px solid transparent;
  
  border-top: 20px solid #000;

  margin: 5px;
}


.banner {
  margin-bottom: 50px;
}

.intro {
  
}

.cnv-blt-1 {
  margin-bottom: 100px;
}

.summary {
  
}

.endnotes {
  margin-bottom: 200px;
}

.topic-group-steps {
  width: 100%;
  height: 100%;
}

.con-belt {
  width: 100%;
  height: 60px;
  margin-left: 60px;
  color: #f72585;
  background: linear-gradient(90deg, currentColor 50%, #0000 0) 0 0%,
    linear-gradient(-90deg, currentColor 50%, #0000 0) 50%,
    linear-gradient(90deg, currentColor 50%, #0000 0) 0 100%;
  background-size: 10px calc(100% / 3);
  background-repeat: repeat-x;
  animation: roll 50s infinite linear; /* Slowed down to 2 seconds */
}

.con-belt-v {
  width: 60px;
  height: 100%;
  margin-left: 60px;
  color: #f72585;
  background: linear-gradient(0deg, currentColor 50%, #0000 0) 0 0%,
    linear-gradient(0deg, currentColor 50%, #0000 0) 50%,
    linear-gradient(0deg, currentColor 50%, #0000 0) 0 100%;
  background-size: 10px calc(100% / 3);
  background-repeat: repeat-y;
  animation: roll 2.8s infinite linear; /* Slowed down to 1.8 seconds */
}

@keyframes roll {
  100% {
    background-position: -10px 0%, -20px 50%, -40px 100%;
  }
}

.highlighted-text-box {
  background-color: #f3f4f6; /* Light gray background */
  border: 2px solid #ed820e; /* Orange border for emphasis */
  border-radius: 8px;
  padding: 20px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  margin: 20px 0;
}

.highlighted-text-box h3 {
  font-size: 2em;
  margin-bottom: 10px;
  font-weight: bold;
  color: #ed820e;
  text-align: left;
}

.highlighted-text-box h4, .highlighted-text-box h5 {
  font-size: 1.1em;
  font-weight: bold;
  color: #333; /* Dark text color for contrast */
  margin-bottom: 10px;
  text-align: left;
}

.highlighted-text-box p {
  font-size: 1.1em;
  color: #555;
  line-height: 1.6;
  text-align: left;
}

.highlighted-text-box a {
  color: #ed820e; /* Matching orange color */
  text-decoration: none;
  font-weight: bold;
  border-bottom: 2px solid #ed820e; /* Adds an underline effect */
  transition: color 0.3s ease, border-color 0.3s ease;
}

.highlighted-text-box a:hover {
  color: #d46900; /* Darker orange on hover */
  border-color: #d46900; /* Matches hover color */
}

.highlighted-text-box-yellow {
  background-color: #fff9db; /* Light yellow background */
  border: 2px solid #ffcc00; /* Yellow border for emphasis */
  border-radius: 8px;
  padding: 20px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  margin: 20px 0;
}

.highlighted-text-box-yellow h3 {
  font-size: 2em;
  margin-bottom: 10px;
  font-weight: bold;
  color: #ffcc00;
  text-align: left;
}

.highlighted-text-box-yellow h4, .highlighted-text-box-yellow h5 {
  font-size: 1.1em;
  font-weight: bold;
  color: #333; /* Dark text color for contrast */
  margin-bottom: 10px;
  text-align: left;
}

.highlighted-text-box-yellow p {
  font-size: 1.1em;
  color: #555;
  line-height: 1.6;
  text-align: left;
}

.highlighted-text-box-yellow a {
  color: #ffcc00; /* Matching yellow color */
  text-decoration: none;
  font-weight: bold;
  border-bottom: 2px solid #ffcc00; /* Adds an underline effect */
  transition: color 0.3s ease, border-color 0.3s ease;
}

.highlighted-text-box-yellow a:hover {
  color: #e6b800; /* Darker yellow on hover */
  border-color: #e6b800; /* Matches hover color */
}

.highlighted-text-box-blue {
  background-color: #e0f2ff; /* Light blue background */
  border: 2px solid #00aaff; /* Blue border for emphasis */
  border-radius: 8px;
  padding: 20px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  margin: 20px 0;
}

.highlighted-text-box-blue h3 {
  font-size: 2em;
  margin-bottom: 10px;
  font-weight: bold;
  color: #0077cc; /* Darker blue for the header */
  text-align: left;
}

.highlighted-text-box-blue p {
  font-size: 1.1em;
  color: #555;
  line-height: 1.6;
  text-align: left;
}

/* Anchor styling for blue theme */
.highlighted-text-box-blue a {
  color: #0077cc; /* Matching blue color */
  text-decoration: none;
  font-weight: bold;
  border-bottom: 2px solid #0077cc; /* Underline effect */
  transition: color 0.3s ease, border-color 0.3s ease;
}

.highlighted-text-box-blue a:hover {
  color: #005a99; /* Darker blue on hover */
  border-color: #005a99; /* Matches hover color */
}

.bg-yellow-version {
  background-color: #fde047;
  border: 2px solid #fde047;
  border-radius: 8px;
  padding: 20px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  transition: background-image 0.5s ease-in-out;
}

.topic-group-steps {
  width: 100%;
  height: auto;
  object-fit: cover;
  transition: opacity 0.5s ease-in-out;
}

.img-hidden {
  opacity: 0;
}

.img-visible {
  opacity: 1;
}

.image-container {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  background-color: rgba(0, 0, 0, 0.6); /* Semi-transparent dark overlay */
  border: 1px solid rgba(255, 223, 47, 0.9); /* Border with slightly less transparency */
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.3); /* Subtle shadow for depth */
  backdrop-filter: blur(10px); /* Optional: adds a blur effect for a glossy look */
}

/* Glossy heading similar to highlight-text-intro */
.glossy-heading {
  background-color: rgba(0, 0, 0, 0.6); /* Semi-transparent dark background */
  padding: 1em 2em;
  border-radius: 8px;
  color: #e0e6ed;
  text-align: center;
  text-shadow: 1px 1px 4px rgba(0, 0, 0, 0.4); /* Adds depth to the text */
}

/* Arrow styles similar to THE VISION section */
.arrows-container {
  margin-top: 10px;
}

.arrow-down-2 {
  width: 0;
  height: 0;
  border-left: 20px solid transparent;
  border-right: 20px solid transparent;
  border-top: 20px solid #000;
  margin: 5px auto;
}

.text-box-inside {
  background-color: #e0e0e0;   /* Light gray for chat bubbles */
  color: black;
  padding: 15px;
  border-radius: 15px;         /* Rounded corners to look like chat bubbles */
  margin: 10px 0;
  max-width: 80%;              /* Limit the width of the chat bubbles */
  word-wrap: break-word;       /* Ensure long text breaks to new lines */
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Subtle shadow for the chat bubble effect */
  text-align: left;            /* Ensure text is left-aligned inside the bubble */
}

.text-box-inside:nth-child(odd) {
  align-self: flex-start;      /* Align odd messages to the left */
  background-color: #f1f1f1;   /* Light background for odd messages */
}

.text-box-inside:nth-child(even) {
  align-self: flex-end;        /* Align even messages to the right */
  background-color: #d1e7dd;   /* Light green background for even messages */
}

.color-yellow {
  color: #fde047;
}

.glossy-bold-black-h2 {
  font-size: 4em;               /* Large font size */
  text-transform: uppercase;     /* Make the text uppercase */
  font-weight: 800;              /* Extra bold font weight */
  color: #000;                   /* Black text color */
  background: linear-gradient(145deg, #1a1a1a, #4d4d4d); /* Subtle glossy gradient */
  padding: 10px 20px;            /* Padding for spacing */
  border-radius: 10px;           /* Rounded corners */
  box-shadow: 2px 4px 6px rgba(0, 0, 0, 0.3), /* Subtle shadow */
              inset 0px -2px 6px rgba(255, 255, 255, 0.4); /* Inner shadow for glossy effect */
  text-shadow: 1px 2px 4px rgba(0, 0, 0, 0.4); /* Text shadow for depth */
  letter-spacing: 1px;           /* Slightly increase letter spacing */
  text-align: center;            /* Center align text */
}

.hover-container {
  position: relative;
  display: inline-block;
  text-align: center;
  width: 100%;
  max-width: 400px; /* Slightly smaller for the main image */
  margin: 0 auto;
}

.main-image {
  width: 100%; /* The main image will adjust to container width */
  height: auto;
  display: block;
  transition: transform 0.3s ease-in-out; /* Add a subtle shrink effect */
}

.hover-box {
  position: absolute;
  top: 50%;
  left: -100%; /* Start outside of the container */
  transform: translateY(-50%);
  background-color: rgba(255, 255, 255, 0.8); /* Semi-transparent background for readability */
  padding: 20px;
  width: 200px; /* Adjust width of the hover box */
  transition: left 0.5s ease-in-out; /* Smooth slide-in transition */
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1); /* Subtle shadow for hover box */
}

.hover-container:hover .hover-box {
  left: 105%; /* Slide the hover box in from the left */
}

.hover-container:hover .main-image {
  transform: scale(0.9); /* Shrink the main image slightly on hover */
}

.hover-description {
  font-size: 1.2em;
  color: #333;
  line-height: 1.6;
  text-align: left;
}

/* New trailing arm style */
.trailing-arm {
  position: absolute;
  top: 50%;
  left: -100%;
  height: 20px; /* Height of the arm */
  width: 0; /* Initially hidden */
  background-color: #555; /* Dark industrial color */
  transform: translateY(-50%);
  transition: width 0.5s ease-in-out; /* Matches the hover-box transition */
}

.hover-container:hover .trailing-arm {
  width: calc(100% + 200px); /* Extends the arm to cover the image and text box width */
  left: 0; /* Moves the arm in with the hover box */
}

.svg-glove {
  position: absolute;
  top: 50%;
  left: -100%;
  transform: translateY(-50%);
  width: 50px; /* Adjust based on your SVG size */
  height: 50px;
  transition: left 0.5s ease-in-out; /* Same transition as the hover box */
}

.hover-container:hover .svg-glove {
  left: 0; /* Move into view when hovered */
}

.glove-shape {
  width: 100%; /* Adjust the width */
  height: auto;
  fill: #555; /* Industrial glove color */
}

.neon-flicker {
  color: #00ffcc; /* Neon color */
  text-shadow: 
    0 0 5px #00ffcc, 
    0 0 10px #00ffcc,
    0 0 20px #00ffcc, 
    0 0 40px #00ffcc, 
    0 0 80px #00ffcc, 
    0 0 120px #00ffcc; /* Glowing effect with multiple levels */
  animation: flicker 2.5s infinite alternate;
  font-weight: bold;
  text-transform: uppercase;
}

@keyframes flicker {
  0% {
    opacity: 0.1;
    text-shadow: 
      0 0 5px #00ffcc, 
      0 0 10px #00ffcc,
      0 0 20px #00ffcc, 
      0 0 40px #00ffcc, 
      0 0 80px #00ffcc, 
      0 0 120px #00ffcc;
  }
  10%, 70% {
    opacity: 1;
    text-shadow: 
      0 0 5px #00ffcc, 
      0 0 10px #00ffcc,
      0 0 20px #00ffcc, 
      0 0 40px #00ffcc, 
      0 0 80px #00ffcc, 
      0 0 120px #00ffcc;
  }
  80% {
    opacity: 0.2;
    text-shadow: 
      0 0 5px #00ffcc, 
      0 0 10px #00ffcc,
      0 0 20px #00ffcc, 
      0 0 40px #00ffcc;
  }
  90% {
    opacity: 1;
    text-shadow: 
      0 0 5px #00ffcc, 
      0 0 10px #00ffcc,
      0 0 20px #00ffcc, 
      0 0 40px #00ffcc, 
      0 0 80px #00ffcc, 
      0 0 120px #00ffcc;
  }
  100% {
    opacity: 0.9;
    text-shadow: 
      0 0 5px #00ffcc, 
      0 0 10px #00ffcc,
      0 0 20px #00ffcc, 
      0 0 40px #00ffcc;
  }
}


</style>