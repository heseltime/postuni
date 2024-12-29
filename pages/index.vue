<template>
  <div>

    <div> 

      <div :style="isAnimationsEnabled ? { animation: 'roll 50s infinite linear' } : {}" class="con-belt"></div>

      <div class="banner">
        <img src="~/assets/img/plants-banner.png" alt="PostCity Banner" />	
        <p class="text-gray-300">Photo Credit: Founding Lab member <a href="https://www.sonialitwin.com">@sonialitwin</a></p>
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
          <h2 class="glossy-bold-black-h2">IT:U x PostCity Is <span class="neon-flicker">PostIT:U</span></h2>

      </div>

      <div class="full">
        <img src="~/assets/img/orange2_sonia_litwin_ccby.png" alt="Orange Wall" class="" />	
        <div :style="isAnimationsEnabled ? { animation: 'roll 50s infinite linear' } : {}" class="con-belt"></div>
        <p class="text-gray-300">Photo Credit: Founding Lab member <a href="https://www.sonialitwin.com">@sonialitwin</a></p>
      </div>

      <h4 class="text-2xl uppercase mb-4 pt-10 font-mono text-blue-300">Let's <b>go into</b> PostCity!</h4>

      <h3 class="text-3xl uppercase mb-10 pb-10 font-mono text-blue-300">Some Lucky Numbers for PostCity <b>->NOW<-</b>?</h3>

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
            <img :src="step.image" alt="Main Image" class="main-image" />
            <div class="image-glove">
                <img src="~/assets/img/hand-1.png" alt="Hand Pushing" class="glove-image" />
            </div>
            <div class="hover-box">
                <span class="text-9xl text-gray-600">{{ step.id }}</span>
                <p class="hover-description">{{ step.text }}</p>
            </div>
        </div>
      </div>

      </Scrollama>

    </div>

    <h3 class="text-3xl uppercase mb-4 font-mono text-blue-300 mt-2">So Why <b>->ARE<-</b> Decision Makers Like <b>This</b> About It?</h3>

    <!-- Ref. Once-In-A-Lifetime Oppt: Shrugging Guy Yellow Here, Also Pick Up Gloves Style -->
    <img src="~/assets/img/shrug.gif" alt="PostCity City Model" class="" width="200px" />

    <h4>Where many people <b>across party-lines</b> are starting to see an opportunity, it sounds like our politician-leaders see expensive private real estate development and a shopping mall thrown in, leading Linz down the road of <b>not just the ordinary and bland, but laying the groundwork for an undesirable urban social development in the century to come</b>.</h4>

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
      <p class="mb-5 text-gray-400">Art Credit: <b>post:collective</b> (<a href="https://postuni.at">PostUni</a>)</p>
    </div>


    <div class="full">
      <img src="~/assets/img/RoboticsTopic_sonia_litwin_ccby.png" alt="Orange Wall" class="" />	
      <div :style="isAnimationsEnabled ? { animation: 'roll 50s infinite linear' } : {}" class="con-belt"></div>
      <p class="text-gray-300">Photo Credit: Founding Lab member <a href="https://www.sonialitwin.com">@sonialitwin</a></p>
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
        class="graphic flex-1 sticky top-0 mt-20 flex flex-col items-center justify-center"
      >
        <img
          v-if="activeStepIdSticky2Image"
          :src="activeStepIdSticky2Image"
          :alt="activeStepIdSticky2"
          class="full-height-image"
        />
        <p v-if="activeStepIdSticky2Credit" class="text-xs text-gray-500 mt-2">{{ activeStepIdSticky2Credit }}</p>
      </div>
      <Scrollama
        :offset="0.6"
        class="flex-1"
        @step-enter="stepEnterHandlerSticky2"
        @step-exit="stepExitHandlerSticky2"
      >
        <div
          v-for="step in stepsSticky2"
          :key="step.id"
          :data-step-id="step.id"
          :class="[
            'my-64 h-auto w-64 mx-auto flex flex-col justify-center items-center p-4 transition-transform duration-300 transition-background',
            activeStepIdSticky2 === step.id ? 'active-step' : 'bg-yellow-300'
          ]"
        >
          <p v-if="step.timeline" class="timeline-text mb-4">{{ step.timeline }}</p>
          <img :src="step.image2" :alt="`Event ${step.id} - Alt`" class="scroll-image w-full h-auto object-cover mb-2 transition-transform duration-300" />
          <p class="text-sm text-gray-700 mt-2">{{ step.text }}</p>
          <a v-if="step.link" :href="step.link" target="_blank" class="text-blue-600 underline text-sm mt-1">Read more</a>
          <p v-if="step.credit2" class="text-xs text-gray-500 mt-1">{{ step.credit2 }}</p>
          <p v-if="step.comment" class="comment-text mt-2">{{ step.comment }}</p>
          <a v-if="step.link2" :href="step.link2" target="_blank" class="text-blue-600 underline text-xs mt-1">Related link</a>
        </div>
      </Scrollama>
    </div>

    <h3 class="text-4xl uppercase mb-4 font-mono text-red-300 mt-2">This Leaves the <b>->MAYOR OF LINZ<-</b> as a <b>central figure in this story</b></h3>

    <p>IT:U was <b>supposed to be built near Johannes Kepler University</b>. However, <b>acting mayor</b> <a class="text-red-300 text-underline" href="https://www.derstandard.at/story/3000000239720/linzer-digital-uni-itu-wird-nicht-am-areal-in-auhof-nahe-der-jku-gebaut">Dietmar Prammer <b>halted the rezoning to building land</b> due to a negative ecologocial assessment</a> (Link in DE). So <b>how will the next Mayor of Linz shape the project?</b></p>

    <!-- Political Part (Conditional Display) -->
    <div v-if="isPoliticsEnabled" class="bg-red text-gray-100 text-center pb-2">
      <div class="max-w-3xl w-full mx-auto px-8 pt-10">
        <h3 id="the-politics" class="text-3xl uppercase mb-4 font-mono text-blue-300 mt-5">
          <b>->LET'S TAKE A LOOK AT MAYORAL CANDIDATES<-</b>
        </h3>  

        <div class="header-box">
          <div class="info header">
            <h3>MAYORAL CANDIDATES 2024/25</h3>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
            <div class="arrow-down"></div>
          </div>
        </div>

        <div class="highlighted-text-box-red mb-4">
          <h3>The Current Political Options in the Upcoming Mayoral Election for Linz</h3>
          <h4>The election is an important political moment for Linz with regards to the question of IT:U's location - where we strongly believe Linz is the appropriate location in Upper Austria.</h4>

          <p>We collect this information from official campagin materials and direct inquiry only: <b>we are looking for a firm statement for use of PostCity for the IT:U and related educational facilities</b> instead of alternate projects.</p>

          <h2>Let's Vote for Linz</h2>

          <p>The following list is in alphabetic order and gives an overview of the relevant information about candidates and their stance as well as history with the location selection.</p>

          <table class="candidates-table">
            <thead>
              <tr>
                <th>Image</th>
                <th>Candidate</th>
                <th>Position</th>
                <th>Supports IT:U @ PostCity (PostUni)</th>
                <th>Connection to Original Grüngürtel Plan</th>
              </tr>
            </thead>
            <tbody>
              <tr v-for="candidate in candidates" :key="candidate.id" :data-support="candidate.support ? 'yes' : ''">
                <td><img :src="candidate.image" :alt="candidate.name" class="candidate-img" /></td>
                <td 
                  :style="{ 
                    color: candidate.partyColor, 
                    backgroundColor: '#ffffff', /* White background */ 
                    fontWeight: 'bold' /* Bold font */
                  }"
                >
                  <span @click="showPopup(candidate)" class="cursor-pointer hover:underline">
                    {{ candidate.name }}
                  </span>
                </td>
                <td>{{ candidate.description }}</td>
                <td class="support-icon" :data-support="candidate.support ? 'yes' : ''"></td>
                <td class="support-icon" :data-support="candidate.greenbelt ? 'yes' : ''">
                  <template v-if="!candidate.greenbelt">
                    <p class="text-xs text-gray-900">*see <b>Note</b> below: voted FOR the problematic original greenbelt plan</p>
                  </template>
                </td>
              </tr>
            </tbody>
          </table>

        </div>

        <popup v-if="selectedCandidate" @close="selectedCandidate = null">
          <template v-slot:header>
            <h2>{{ selectedCandidate.name }}</h2>
          </template>
          <template v-slot:content>
            <p>{{ selectedCandidate.fullStatement }}</p>
          </template>
        </popup>
      </div>
    </div>

    <h4 class="mb-4"><b>Note</b>: The two representatives of the larger parties, SPÖ and ÖVP in Linz, are notable because they voted <b>for</b> the original Grüngürtel plan (in line with their parties) under then SPÖ Mayor Luger before backtracking under Deputy Mayor Prammer, under some pressure from the county government. The original idea for this location came from a questionable process without any significant transpareny or inclusion of stakeholders beyond politics and business, not to mention the public.</h4>

    <img alt="Gemeinderat Distribution Vote for Grüngürtel: SPÖ and ÖVP vote for the decision" src="~/assets/img/gemeinderat.jpg.webp" />

    <h4 class="mb-10">Courtesy of <a href="https://www.linzplus.at/post/stadtpolitik-verkauft-gruenguertel">Linz+</a></h4>

    <h3 class="text-3xl uppercase mb-10 font-mono text-blue-300 mt-5">
      <b>With this ->NEW INTEREST IN THE IT:U LOCATION QUESTION<- we are hopeful a sensible decision will be made and voted for under the new mayor</b>
    </h3>  

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

        <p class="mb-10 text-gray-400">Art Credit: <b>post:collective</b> (<a href="https://postuni.at">PostUni</a>)</p>
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
      steps: [
        { id: '1', image: require('../assets/img/postUNI@daniel_schöngruber_1.jpg') },
        { id: '2', image: require('../assets/img/plan1b3x.png') },
      ],
      imageReplacement: require('../assets/img/postUNI@daniel_schöngruber_2.png'),
      imageReplacement2: require('../assets/img/plan1a3x.png'),
      stepsSticky: [
        { id: '75', text: 'students founded the university here', image: require('../assets/img/spectacular.png') }, 
        { id: '4000+', text: 'signatures against closing the Green Belt', image: require('../assets/img/no-field.png') }, 
        { id: '7', text: 'Mayoral Candidates in 2024/25', image: require('../assets/img/mhwbg.png') }, 
        { id: '1', text: 'Owner: NOW Open to Negotiation', image: require('../assets/img/post-delivers.png') }
      ],
      stepsSticky2: [
        { id: '1', 
          timeline: 'October 2024',
          text: 'The new Digital University will not be built near Johannes Kepler University after all.',
          comment: 'This kicks of the current story and this initiative.', 
          link: 'https://www.meinbezirk.at/linz/c-politik/neue-digital-uni-wird-doch-nicht-bei-johannes-kepler-universitaet-gebaut_a6937880?ref=curate#gallery=null', 
          image: require('../assets/img/sticky2-1a.png'), 
          image2: require('../assets/img/sticky2-1b.jpg'),
          credit: 'Rendering: Kronaus Mitterer Architekten ZT GmbH',
          credit2: 'Photo: IT:U and Fotokerschi/Kerschbaum' }, 
        { id: '2', 
          timeline: 'Throughout 2024',
          text: 'The "Post City Gardens" project in Linz, planned on the PostCity site, has faced significant delays due to challenges in securing investors.',
          comment: 'With this location available, will an open-minded, inspired Post AG remain open and push for intelligent transformation as part of its OEBAG (who majority-owns the Post) mandate?',
          link: 'https://www.nachrichten.at/oberoesterreich/linzer-post-city-gardens-investorensuche-ist-gescheitert;art4,3911556#:~:text=Seitens%20der%20Post%20wird%20nun%20mit%20einem%20Baubeginn%20frühestens%202026%20gerechnet.',
          link2: 'https://oebag.gv.at',
          image: require('../assets/img/sticky2-2a.png'), 
          image2: require('../assets/img/sticky2-2b.png'),
          credit: 'Rendering: Nussmüller Architekten ZT GmbH / Expressiv GmbH',
          credit2: 'Logo: Post AG' }, 
        { id: '3', 
          timeline: 'October 2024',
          text: 'Governor Thomas Stelzer has stated that the search for a location for the "Digital University" will be handled at the highest level.', 
          comment: 'And so, as the governor considers all of Upper Austria in his own search, will Hallstatt also be shortlisted, we wonder?',
          link: 'https://www.meinbezirk.at/linz/c-politik/lh-stelzer-erklaert-standortsuche-fuer-digital-uni-zur-chefsache_a6940181',
          image: require('../assets/img/sticky2-3a.png'), 
          image2: require('../assets/img/sticky2-3b.png'),
          credit: 'Photo: State of Upper Austria/Peter May',
          credit2: 'Photo: austriavienna.info' }, 
        { id: '4', 
          timeline: 'October 2024',
          text: 'Despite other applicants: Linz is the IT:U location.',
          comment: 'The national government (Federal Ministry of Education, Science and Research) sees the university in Linz, however, where it belongs - we agree.',
          link: 'https://www.nachrichten.at/politik/innenpolitik/trotz-anderer-bewerber-linz-ist-der-itu-standort;art385,3992118', 
          image: require('../assets/img/sticky2-4a.png'), 
          image2: require('../assets/img/sticky2-4b.png'),
          credit: 'Photo: Antonio Bayer',
          credit2: 'Photo: 1000things.at' }
      ],
      activeStepId: null,
      activeStepIdSticky: 'A',
      activeStepIdSticky2: '75',
      activeStepIdSticky2Image: require('../assets/img/spectacular.png'),
      selectedCandidate: null,
      candidates: [
        {
          id: 1,
          name: "Martin Hajart",
          partyColor: "#796190",
          partyName: "ÖVP",
          description: "supports establishing IT:U in Linz, considers PostCity one of further options (however) - *see note below, voted for the original Grüngürtel plan.",
          fullStatement: "Mr Hajart wrote (December 26th, 2024): Fundamentally, I would have supported the establishment of IT:U next to JKU but want to emphasize that, during discussions, I consistently opposed the construction of corporate headquarters in recreational areas. Additionally, any project should be environmentally sustainable. My focus (and it remains so) has been to establish small, business-oriented research units alongside IT:U to create a biotope that bridges basic research to applied research. \
          The planning for IT:U has been underway for years. That the project has now been scrapped after this long preparation period without any concrete alternative locations sets IT:U back by years. I deeply regret this.\
          Nevertheless, given the significance of this century-defining project, it is crucial to look forward. PostCity is a good alternative as a location. I have also proposed the current site of Raiffeisenlandesbank OÖ (which will soon relocate to a nearby plot) as a potential location that, in my view, would be suitable. However, there are other possible sites worth considering. It is essential that the location remains in Linz and that ultimately the best possible site is chosen.",
          image: require('../assets/img/hajart.png'),
          support: true,
          greenbelt: false,
        },
        {
          id: 2,
          name: "Michael Raml",
          partyColor: "#31579F", 
          partyName: "FPÖ",
          description: "sees PostCity as the ideal location for IT:U due to its excellent transport links, avoidance of environmental impact, and potential to transform the area around the main train station",
          fullStatement: "Mr Raml wrote (December 19th, 2024): I consider PostCity the ideal location for IT:U, and for several reasons. The transport connections for an internationally active university (which is the goal) are excellent, as it is located right next to the train station. The connection to the A7 motorway would also make the university accessible for drivers, and there would be sufficient space for a large parking garage on-site (which, incidentally, should also be used as a general Park & Ride facility). Unlike the original plan in Auhof, no green spaces need to be paved over for PostCity. It also offers a great opportunity to enhance the area around the main train station into a vibrant student district for all of Linz – extending up to Volksgarten and the southern Landstraße.",
          image: require('../assets/img/raml.png'),
          support: true,
          greenbelt: true,
        },
        {
          id: 3,
          name: "Eva Schobesberger",
          partyColor: "#91B338", 
          partyName: "Greens",
          description: "strong supporter of the Grüngürtel aktion, considers PostCity the main alternative due to public transport links",
          fullStatement: "Ms Schobesberger said on the phone (December 20th, 2024): She was one of the first and loudest supporters of the Grüngürtel Aktion to stop building the first IT:U location proposal. She further supported permanently banning this option in the city government. Now she sees PostCity as the main alternate site, considering IT:U to belong to Linz as well, and at PostCity especially also because of ease of access from public transport (train station).",
          image: require('../assets/img/schobesberger.png'),
          support: true,
          greenbelt: true,
        },
        {
          id: 4,
          name: "Lorenz Potocnik",
          partyColor: "#F9EC37", 
          partyName: "LINZ+",
          description: "supports IT:U location in PostCity or another city location, after a proper location selection process, which has been absent so far",
          fullStatement: "This candidate made himself available by phone, referencing extensive background writings on the topic, e.g. https://www.linzplus.at/post/itu-und-flaechenverbrauch and https://www.linzplus.at/post/auhof-sieg-der-zivilgesellschaft - all taking a clear stance against the original IT:U location plan and for due process.",
          image: require('../assets/img/potocnik.png'),
          support: true,
          greenbelt: true,
        },
        {
          id: 5,
          name: "Dietmar Prammer",
          partyColor: "#A6131F", 
          partyName: "SPÖ",
          description: "supports IT:U location in PostCity as well as others in the city, according to media outlets (no direct statement as of yet) - *see note below, voted for the original Grüngürtel plan.",
          fullStatement: "Not (yet) available",
          image: require('../assets/img/prammer.jpg'),
          support: true,
          greenbelt: false,
        }
      ],
    }
  },
  props: {
    isDarkMode: {
        type: Boolean,
        default: false,
    },
    isAnimationsEnabled: {
        type: Boolean,
        default: true,
    },
    isPoliticsEnabled: {
      type: Boolean,
      default: true,
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
      } else if (stepId === '2') {
        const stepIndex = this.steps.findIndex(step => step.id === '2');
        if (stepIndex !== -1) {
          this.steps[stepIndex].image = this.imageReplacement2;
        }
      }
    },
    stepEnterHandlerSticky ({ element, direction, index }) {
      //console.log('step-enter', { element, direction, index })
      this.activeStepIdSticky = element.dataset.stepId
    },
    stepEnterHandlerSticky2 ({ element, direction, index }) {
      //console.log('step-enter', { element, direction, index })
      this.activeStepIdSticky2 = element.dataset.stepId;
      const currentStep = this.stepsSticky2.find(step => step.id === this.activeStepIdSticky2);
      if (currentStep) {
        this.activeStepIdSticky2Image = currentStep.image;
        this.activeStepIdSticky2Credit = currentStep.credit;
      }
    },
    stepExitHandler({ element }) {
      const stepId = element.dataset.stepId;
      if (stepId === '1') {
        const stepIndex = this.steps.findIndex(step => step.id === '1');
        if (stepIndex !== -1) {
          this.steps[stepIndex].image = require('../assets/img/postUNI@daniel_schöngruber_1.jpg');
        }
      } else if (stepId === '2') {
        const stepIndex = this.steps.findIndex(step => step.id === '2'); // Find index for stepId '2'
        if (stepIndex !== -1) {
          this.steps[stepIndex].image = require('../assets/img/plan1b3x.png');
        }
      }
      this.activeStepId = null;
    },
    stepExitHandlerSticky2({ element }) {
      // Reset active step when it exits
      if (this.activeStepIdSticky2 === element.dataset.stepId) {
        this.activeStepIdSticky2 = null;
      }
    },
    showPopup(candidate) {
      this.selectedCandidate = candidate;
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
  /*border: 2px solid #ed820e;  Orange border for emphasis */
  border: 2px solid #555; 
  border-radius: 8px;
  padding: 20px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  margin: 20px 0;
}

.highlighted-text-box h3 {
  font-size: 2em;
  margin-bottom: 10px;
  font-weight: bold;
  /*color: #ed820e;*/
  color: #888;
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
  /*background-color: #fff9db;*/ /* Light yellow background */
  background-color: #bbb;
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
  /*color: #ffcc00;*/
  color: #666;
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
  /*background-color: #e0f2ff;*/ /* Light blue background */
  background-color: #ddd;
  /*border: 2px solid #00aaff;*/ /* Blue border for emphasis */
  border: 2px solid #000;
  border-radius: 8px;
  padding: 20px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  margin: 20px 0;
}

.highlighted-text-box-blue h3 {
  font-size: 2em;
  margin-bottom: 10px;
  font-weight: bold;
  /*color: #0077cc;*/ /* Darker blue for the header */
  color: #777;
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

.highlighted-text-box-red {
  background-color: #4a1a1a; /* Dark red background */
  /*border: 2px solid #b30000;*/ /* Darker red border */
  border-radius: 8px;
  padding: 20px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.3); /* Slightly darker shadow for emphasis */
  margin: 20px 0;
  color: #f3f3f3; /* Light text color for contrast */
}

.highlighted-text-box-red h3 {
  font-size: 2em;
  margin-bottom: 10px;
  font-weight: bold;
  color: #ff4d4d; /* Light red for the header */
  text-align: left;
}

.highlighted-text-box-red h4, .highlighted-text-box-red h5 {
  font-size: 1.1em;
  font-weight: bold;
  color: #f3f3f3; /* Light text color for contrast */
  margin-bottom: 10px;
  text-align: left;
}

.highlighted-text-box-red p {
  font-size: 1.1em;
  color: #e0e0e0; /* Light gray for paragraph text */
  line-height: 1.6;
  text-align: left;
}

.highlighted-text-box-red a {
  color: #ff4d4d; /* Light red for links */
  text-decoration: none;
  font-weight: bold;
  border-bottom: 2px solid #ff4d4d;
  transition: color 0.3s ease, border-color 0.3s ease;
}

.highlighted-text-box-red a:hover {
  color: #e60000; /* Darker red on hover */
  border-color: #e60000;
}
.candidates-table {
  width: 100%;
  margin-top: 20px;
  border-collapse: collapse;
  font-size: 1em;
  color: #e0e0e0;
}

.candidates-table th,
.candidates-table td {
  padding: 12px;
  text-align: center;
  border-bottom: 1px solid #b30000;
}

.candidates-table td p {
  color: #000;
  font-size: x-small;
}

.candidates-table th {
  background-color: #5c1d1d; /* Dark red header background */
  color: #f3f3f3; /* Light text color */
  font-weight: bold;
}

.candidates-table tbody tr:nth-child(even) {
  background-color: #4a1a1a; /* Alternate row color */
}

.candidate-img {
  width: 50px;
  height: 50px;
  object-fit: cover;
  border-radius: 50%; /* Circular image */
}

/* Style for support icons */
.support-icon {
  font-size: 1.8em; /* Increased size for visibility */
  font-weight: bold;
  color: #e60000; /* Default red color for X */
}

.support-icon:before {
  content: "✗"; /* Default X for no support */
}

/* Highlight checkmark in green */
.support-icon[data-support="yes"] {
  color: #4caf50; /* Green for support */
}

.support-icon[data-support="yes"]:before {
  content: "✓"; /* Checkmark icon */
}

.candidates-table tbody tr[data-support="yes"] {
  background-color: #e6f4e8; /* Light green background for supporters */
  color: #2c3e50; /* Dark text color for readability */
  border-radius: 8px;
  overflow: hidden; /* Prevents content overflow on rounded corners */
  margin: 5px;
}

/* Make the first and last cell in each row rounded */
.candidates-table tbody tr[data-support="yes"] td:first-child {
  border-top-left-radius: 8px;
  border-bottom-left-radius: 8px;
}

.candidates-table tbody tr[data-support="yes"] td:last-child {
  border-top-right-radius: 8px;
  border-bottom-right-radius: 8px;
}

.candidates-table tbody tr:nth-child(even):not([data-support="yes"]) {
  background-color: #4a1a1a; /* Alternate row color for non-supporters */
  color: #f3f3f3; /* Light text color for dark background */
}

.candidates-table th {
  background-color: #5c1d1d; /* Dark red header background */
  color: #f3f3f3; /* Light text color */
  font-weight: bold;
}

/* Style support icons */
.support-icon[data-support="yes"] {
  color: #4caf50; /* Green color for checkmark */
}

.support-icon:not([data-support="yes"]) {
  color: #e60000; /* Red color for X */
}

.highlighted-text-box-red h2 {
  font-size: 2.5em; /* Larger font size */
  font-weight: bold;
  color: #ffcccc; /* Light red color */
  text-align: center;
  background: linear-gradient(135deg, #b30000, #ff4d4d); /* Red gradient */
  padding: 10px 20px;
  border-radius: 10px;
  display: inline-block;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.3); /* Shadow for depth */
  margin: 20px 0;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3); /* Adds depth to text */
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

.image-glove {
  position: absolute;
  top: 50%;
  left: -100%; /* Start outside the container */
  transform: translateY(-50%);
  width: 80px; 
  height: auto;
  transition: left 0.5s ease-in-out; /* Matches the hover-box transition */
}

.hover-container:hover .image-glove {
  left: 0; /* Move the image-glove into view */
}

.glove-image {
  width: 100%;
  height: auto;
  object-fit: contain; /* Ensure the glove image scales properly */
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

.full-height-image {
  height: 100%; /* Make the image fill the container height */
  width: auto;  /* Maintain aspect ratio */
  object-fit: cover; /* Ensures the image covers the container */
}

.scroll-image {
  transform: scale(1); /* Default size */
  transition: transform 0.3s ease-in-out; /* Smooth transition */
}

.active-step .scroll-image {
  transform: scale(1.1); /* Increase size when active */
}

.transition-background {
  /* Darker gray background with light gray border */
  background-color: #555; 
  border: 2px solid #e5e7eb; 
  border-radius: 8px; 
  padding: 20px;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.15); 
  transition: background-color 0.3s ease-in-out, border-color 0.3s ease-in-out;
}

.transition-background:hover {
  background-color: #fde047; /* Yellow background on hover */
  border-color: #facc15; /* Slightly darker yellow border on hover */
}

.transition-background h3, 
.transition-background h4, 
.transition-background p {
  color: #b7b799; /* Light gray text color */
}

.transition-background:hover h3,
.transition-background:hover h4,
.transition-background:hover p {
  color: #333; /* Dark text color for better contrast on yellow background */
}

.transition-background a {
  color: #9ca3af; 
  text-decoration: none;
  font-weight: bold;
  border-bottom: 2px solid #9ca3af;
  transition: color 0.3s ease, border-color 0.3s ease;
}

.transition-background:hover a {
  color: #333; /* Darker text for better contrast on yellow */
  border-color: #333;
}

.active-step {
  background-color: #888; /* No background when active */
}

.transition-text {
  transition: font-weight 0.3s ease-in-out; /* Smooth transition for font weight */
}

.active-step-text {
  font-weight: bold; /* Bold text when active */
}

.timeline-text {
  font-weight: bold;
  text-transform: uppercase;
  font-size: 1rem; /* Adjust size as needed */
  margin-bottom: 0.5rem;
}

.comment-text {
  color: #6b7280; /* Gray-500 color */
  font-style: italic;
  font-size: 0.875rem; /* Adjust size as needed */
}


</style>