<template>
  <div>
    <div class="h-5 sm:h-12 md:h-20"></div>
    <!-- Landing Intro -->
    <div>
      <div class="flex flex-wrap justify-center">
        <p class="text-2xl px-10 md:pl-0 md:text-5xl text-center font-exo font-bold">
          UI/UX Designer and Full-Stack Web Developer
        </p>
      </div>
      <div class="flex flex-wrap justify-center">
        <p class="text-xl md:text-2xl px-10 md:pl-0 font-exo font-thin text-center">
          UI/UX Designer and Full-Stack Web Developer
        </p>
      </div>
    </div>
    <!-- Avatar -->
    <div class="flex flex-wrap justify-center mt-20">
      <img :src="bruck" alt="" />
    </div>

    <!-- Intro and Services -->
    <div class="bg-blue-900 mt-8">
      <!-- Intro -->
      <p class="text-center font-exo text-white py-10 text-3xl font-bold pb-2">
        Hi, I am Bruck. Nice to Meet You!
      </p>
      <div class="flex flex-wrap justify-center">
        <div class="w-1/2">
          <p
            class="text-gray-500 text-center pt-2 text-lg leading-loose font-regular mb-6"
          >
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores minus esse
            quidem sapiente odio, earum optio nobis, natus deleniti atque dolorem debitis
            repellat molestiae laboriosam quo sequi.
          </p>
        </div>
      </div>
    </div>
    <!-- Services -->
    <div class="mb-10">
      <div class="bg-blue-900 h-40"></div>
      <div class="p-2 md:p-10 grid grid-cols-1 lg:grid-cols-3 gap-4 -mt-40 md:-mt-48">
        <!--Card-->
        <div
          v-for="(service, index) in services"
          :key="index"
          class="bg-gray-100 rounded overflow-hidden shadow-lg"
        >
          <div class="flex flex-wrap justify-center mt-4">
            <img :src="require('../assets/' + service.iconName)" />
          </div>
          <div class="px-6 py-4">
            <div class="font-exo font-bold text-2xl my-6 text-center">
              {{ service.title }}
            </div>
            <p class="text-gray-700 text-base">
              {{ service.titleDescription }}
            </p>
          </div>
          <div class="mb-6">
            <p class="text-center text-blue-600 my-6 text-xl font-medium font-exo">
              {{ service.subtitle }}
            </p>
            <p class="text-center text-lg mb-6 font-light font-body">
              {{ service.subtitleDescription }}
            </p>
          </div>
        </div>
      </div>
      <div class="grid grid-cols-1 mt-6 md:grid-cols-2">
        <div class="mx-2">
          <p class="md:px-10 text-3xl md:text-4xl font-bold font-exo">
            Working to Bring Ideas To Life &#38;
          </p>
          <p class="md:px-10 -mt-2 text-3xl md:text-4xl font-bold font-exo">
            get Projects Rolling.
          </p>
          <p class="md:px-10 text-lg mt-2 font-regular font-exo">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Id asperiores
            exercitationem maxime fuga saepe quibusdam nostrum facere nisi eius possimus,
            quam iusto earum repellat sequi odit eum, deserunt rerum quaerat?
          </p>
          <div class="flex justify-end md:mr-20 mr-6">
            <button
              class="rounded-full font-exo border-4 mt-4 border-blue-900 px-5 py-3 hover:bg-blue-900 hover:text-white font-body font-bold"
            >
              Hire Me
            </button>
          </div>
        </div>
        <div class="mt-10 sm:mt-0 flex justify-center">
          <img :src="techStack" alt="" />
        </div>
      </div>
      <!-- Recent Works -->
      <div>
        <p class="text-center font-exo py-10 text-3xl md:text-4xl font-bold pb-2">
          Recent Works
        </p>
        <p class="text-gray-900 text-center pt-2 text-lg font-regular mb-6">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores minus esse.
        </p>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-10 mx-10">
          <div class="rounded-2xl bg-blue-200 relative hover:opacity-75">
            <img src="~/assets/wabey.png" class="mx-auto rounded-3xl" alt="Text" />
            <div
              class="opacity-0 hover:opacity-100 rounded-3xl bg-blue-900 duration-500 absolute inset-0 z-10 flex justify-center"
            >
              <div class="w-64">
                <p class="text-xl text-center text-white font-exo mt-10 font-bold">
                  A Start Up Project I am a Part Of and Currently Working On.
                </p>
                <div class="flex justify-center">
                  <button
                    class="flex justify-center rounded-full text-white font-exo border-2 mt-4 border-white px-5 py-3 hover:bg-blue-600 hover:border-blue-600 hover:text-white font-body font-bold"
                  >
                    Visit Website
                    <img class="ml-2 mt-1" :src="next" alt="" />
                  </button>
                </div>
              </div>
            </div>
          </div>
          <div class="bg-black rounded-3xl relative hover:opacity-75">
            <img src="~/assets/tough.webp" class="mx-auto rounded-3xl" alt="Text" />
            <div
              class="opacity-0 hover:opacity-100 rounded-3xl bg-blue-900 duration-500 absolute inset-0 z-10 flex justify-center"
            >
              <div class="w-64">
                <p class="text-xl text-center text-white font-exo mt-10 font-bold">
                  A Start Up Project I am a Part Of and Currently Working On.
                </p>
                <div class="flex justify-center">
                  <button
                    class="flex justify-center rounded-full text-white font-exo border-2 mt-4 border-white px-5 py-3 hover:bg-blue-600 hover:border-blue-600 hover:text-white font-body font-bold"
                  >
                    Visit Website
                    <img class="ml-2 mt-1" :src="next" alt="" />
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import bruck from "@/assets/bruck.svg";
import techStack from "@/assets/techStack.svg";
import next from "@/assets/next.svg";

export default {
  name: "HomePage",
  data() {
    return {
      bruck,
      techStack,
      next,
      services: [
        {
          iconName: "web-design.svg",
          title: "UI/UX Design",
          titleDescription:
            "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptas, tenetur odio harum facere.adipisicing elit. Voluptas, tenetur odio. ",
          subtitle: "Designs For:",
          subtitleDescription: "Web, Mobile, Apps",
          toolsTitle: "Design Tools:",
          tools: ["Adobe XD", "Figma", "Material Design", "Bootstrap"],
        },
        {
          iconName: "front-end.svg",
          title: "Front-End Web Development",
          titleDescription:
            "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptas, tenetur odio. adipisicing elit. Voluptas, tenetur odio.",
          subtitle: "Designs For:",
          subtitleDescription: "Web, Mobile, Apps",
          toolsTitle: "Design Tools:",
          tools: [
            "Adobe XD",
            "Figma",
            "Material Design",
            "Bootstrap",
            "Figma",
            "Material Design",
            "Bootstrap",
            "Vue",
          ],
        },
        {
          iconName: "back-end.svg",
          title: "Back-End Development",
          titleDescription:
            "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptas, tenetur odio adipisicing elit. Voluptas, tenetur odio.",
          subtitle: "Designs For:",
          subtitleDescription: "Web, Mobile, Apps",
          toolsTitle: "Design Tools:",
          tools: [
            "Adobe XD",
            "Figma",
            "Material Design",
            "Bootstrap",
            "Vue",
            "Nuxt",
            "Php",
          ],
        },
      ],
    };
  },
};
</script>

<style>
/* Sample `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
</style>
