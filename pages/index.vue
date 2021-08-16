<template>
  <div>
    <div class="h-5 sm:h-12 md:h-20"></div>
    <!-- Landing Intro -->
    <div>
      <div class="flex flex-wrap justify-center">
        <p class="text-4xl md:text-5xl text-center font-body font-bold">
          UI/UX Designer and Full-Stack Web Developer
        </p>
      </div>
      <div class="flex flex-wrap justify-center">
        <p class="text-2xl font-body font-thin">
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
      <p class="text-center font-body text-white py-10 text-3xl font-bold pb-2">
        Hi, I am Bruck. Nice to Meet You!
      </p>
      <div class="flex flex-wrap justify-center">
        <div class="w-1/2">
          <p class="text-gray-500 text-center pt-6 text-lg leading-loose font-regular">
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
            <div class="font-body font-bold text-2xl my-6 text-center">
              {{ service.title }}
            </div>
            <p class="text-gray-700 text-base">
              {{ service.titleDescription }}
            </p>
          </div>
          <div class="mb-6">
            <p class="text-center text-blue-600 my-6 text-xl font-medium font-body">
              {{ service.subtitle }}
            </p>
            <p class="text-center text-lg mb-6 font-light font-body">
              {{ service.subtitleDescription }}
            </p>
            <p class="text-center text-blue-600 text-xl mb-6 font-body">
              {{ service.toolsTitle }}
            </p>
            <p
              v-for="(tool, index) in service.tools"
              :key="index"
              class="text-center text-lg mb-1 font-body font-light"
            >
              {{ tool }}
            </p>
          </div>
        </div>
      </div>
        <!-- Portifolio -->
       <div class="text-center font-body py-10 text-4xl font-bold pb-2">
      <p>My Portfolio</p>
    </div>
    </div>
  </div>

</template>

<script>
import bruck from "@/assets/bruck.svg";
export default {
  data() {
    return {
      bruck,
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

