<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradsy Download</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css"
    />
    <style>
      body {
        font-family: "Poppins", sans-serif;
      }
    </style>
  </head>
  <body class="bg-[url('/icon/opacity_graduate.png')] bg-no-repeat bg-cover">
    <!-- Main downloading section -->
    <div class="flex flex-col mt-[8vh] lg:mt-[12vh] justify-around">
      <!-- Title and Description -->
      <div
        class="flex flex-wrap items-center justify-around mx-auto text-center lg:text-left"
      >
        <img
          src="/icon/About.png"
          alt=""
          class="w-3/4 lg:w-auto mx-auto lg:mx-0"
        />
        <div class="text-lg lg:text-xl font-bold mb-4">
          <pre><b>   For a more seamless experience,</b></pre>
          <pre><b>  Download Gradsy on your device now!</b></pre>
        </div>
      </div>

      <!-- Download Cards -->
      <div
        class="flex flex-wrap justify-center gap-6 lg:gap-10 mt-8 lg:mt-16 px-4 lg:px-0"
      >
        <!-- Windows Card -->
        <div
          class="flex flex-col w-[15rem] lg:w-[20rem] h-[20rem] lg:h-[22rem] gap-4 lg:gap-6 justify-center items-center text-lg lg:text-xl font-bold rounded-2xl bg-gray-200"
          style="box-shadow: 10px 10px 20px gray;"
        >
          <img
            src="/icon/window.png"
            class="h-[7rem] lg:h-[9rem] rounded-lg mx-auto"
            alt="Windows Icon"
          />
          <p>Download for Windows</p>
          <button
            class="px-6 py-2 rounded-2xl border-2 bg-[#49b6c5] text-white"
          >
            Download
          </button>
        </div>

        <!-- Android Card -->
        <div
          class="flex flex-col w-[15rem] lg:w-[20rem] h-[20rem] lg:h-[22rem] gap-4 lg:gap-6 justify-center items-center text-lg lg:text-xl font-bold rounded-2xl bg-[#2E2E30] text-white"
          style="box-shadow: 10px 10px 20px gray;"
        >
          <img
            src="/icon/playstore.png"
            class="h-[7rem] lg:h-[9rem] mx-auto"
            alt="Play Store Icon"
          />
          <p>Download for Android</p>
          <button
            class="px-6 py-2 rounded-2xl border-2 bg-white text-[#49b6c5]"
          >
            Download
          </button>
        </div>

        <!-- IOS Card -->
        <div
          class="flex flex-col w-[15rem] lg:w-[20rem] h-[20rem] lg:h-[22rem] gap-4 lg:gap-6 justify-center items-center text-lg lg:text-xl font-bold rounded-2xl bg-gray-200"
          style="box-shadow: 10px 10px 20px gray;"
        >
          <img
            src="/icon/apple.png"
            class="h-[7rem] lg:h-[9rem] mx-auto"
            alt="Apple Icon"
          />
          <p>Download for IOS</p>
          <button
            class="px-6 py-2 rounded-2xl border-2 bg-[#49b6c5] text-white"
          >
            Download
          </button>
        </div>
      </div>
    </div>

    <!-- Floating Message Icon -->
    <img
      src="/icon/msg.png"
      class="fixed bottom-4 right-4 w-12 lg:w-auto"
      alt="Message Icon"
    />

    <script></script>
  </body>
</html>
