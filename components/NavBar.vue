<template>
  <div class="h-20">
    <nav class="flex justify-between mx-5 md:mx-20">
      <div class="mt-5">
        <a href="/">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="43.281"
            height="33.168"
            viewBox="0 0 43.281 33.168"
          >
            <path
              d="M673,489.974h13.634s9.784,4.745,5,9.744S673,502.252,673,502.252v14.89h27.446s16.163-11.663,7.015-14.89c-4.363-1.539-11.682-2.247-14.447-2.534h0"
              transform="translate(-670 -486.974)"
              fill="none"
              stroke="#1e3a8a"
              stroke-width="6"
            />
          </svg>
        </a>
        <!-- #123D90 -->
      </div>
      <div class="flex mt-6 invisible md:visible">
        <!-- Github -->
        <a href="https://www.github.com/bruck-3" target="_blank">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="30"
            height="30"
            viewBox="0 0 511.996 512"
          >
            <path
              id="github"
              d="M256,0C115.391,0,0,115.391,0,256,0,375.988,84.2,484.984,196,512V427.3c-11.078,2.426-21.273,2.5-32.551-.828-15.129-4.465-27.422-14.543-36.547-29.91-5.816-9.812-16.125-20.453-26.879-19.672l-2.637-29.883c23.254-1.992,43.371,14.168,55.313,34.23,5.3,8.922,11.41,14.152,19.246,16.465,7.574,2.23,15.707,1.16,25.184-2.187,2.379-18.973,11.07-26.074,17.637-36.074v-.016c-66.68-9.945-93.254-45.32-103.8-73.242-13.977-37.074-6.477-83.391,18.238-112.66.48-.57,1.348-2.062,1.012-3.105-11.332-34.23,2.477-62.547,2.984-65.551,13.078,3.867,15.2-3.891,56.809,21.387l7.191,4.32c3.008,1.793,2.063.77,5.07.543A217.253,217.253,0,0,1,256,123.563a218.192,218.192,0,0,1,54.465,7.75l2.328.234c-.2-.031.633-.148,2.035-.984,51.973-31.48,50.105-21.191,64.043-25.723.5,3.008,14.129,31.785,2.918,65.582-1.512,4.656,45.059,47.3,19.246,115.754-10.547,27.934-37.117,63.309-103.8,73.254v.016c8.547,13.027,18.816,19.957,18.762,46.832V512C427.8,484.984,512,375.988,512,256,512,115.391,396.609,0,256,0Zm0,0"
              fill="#2f4262"
            />
          </svg>
        </a>
        <a href="https://www.linkedin.com/in/bruck25/" target="_blank">
          <svg
            class="ml-4"
            id="linkedin_1_"
            data-name="linkedin (1)"
            xmlns="http://www.w3.org/2000/svg"
            width="30"
            height="30"
            viewBox="0 0 291.319 291.319"
          >
            <path
              id="Path_273"
              data-name="Path 273"
              d="M145.659,0A145.66,145.66,0,1,1,0,145.66,145.66,145.66,0,0,1,145.659,0Z"
              fill="#2f4262"
            />
            <path
              id="Path_274"
              data-name="Path 274"
              d="M82.079,200.136h27.275v-90.91H82.079Zm106.259-94.059c-13.237,0-25.081,4.834-33.483,15.5V108.927H127.48v91.21h27.375V150.813c0-10.424,9.55-20.593,21.512-20.593s14.912,10.169,14.912,20.338v49.57h27.275v-51.6C218.553,112.686,201.584,106.077,188.338,106.077Zm-92.749-5.936A13.655,13.655,0,1,0,81.933,86.486,13.661,13.661,0,0,0,95.589,100.141Z"
              fill="#fff"
            />
          </svg>
        </a>
      </div>
      <div class="mt-4">
        <button
          class="rounded-full font-exo border-2 border-blue-900 px-5 py-3 hover:bg-blue-900 hover:text-white font-body font-bold"
        >
          Say Hello!
        </button>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'NavBar'
};
</script>

<style lang="scss" scoped></style>
