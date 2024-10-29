<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradsy Platform</title>
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
    <!-- Main Section -->
    <div class="flex flex-col items-center justify-center h-screen p-6 lg:p-0">
      <!-- Content Wrapper -->
      <div
        class="flex flex-col lg:flex-row justify-between items-center w-full max-w-7xl mt-[10vh] lg:mt-[20vh]"
      >
        <!-- Left Column: Text and Buttons -->
        <div
          class="flex flex-col items-center lg:items-start text-center lg:text-left"
        >
          <img
            src="/icon/About.png"
            alt="Gradsy About"
            class="w-[60%] lg:w-auto mx-auto lg:mx-0"
          />

          <p class="text-lg lg:text-xl w-[80%] lg:w-[60%] mt-4 lg:mt-6 m-auto">
            Gradsy is a platform that makes alumni tracking, donations, and
            management easier.
          </p>

          <!-- Buttons -->
          <div class="flex justify-around mt-10 lg:mt-16 gap-4">
            <button
              class="px-6 py-2 lg:px-8 lg:py-2.5 rounded-2xl bg-[#49b6c5] text-white"
            >
              <a href="download">Download Gradsy</a>
            </button>
            <button
              class="px-6 py-2 lg:px-8 lg:py-2.5 rounded-2xl border-2 text-[#49b6c5] bg-gray-200"
            >
              <a href="signup">Continue on Browser</a>
            </button>
          </div>
        </div>

        <!-- Right Column: Image -->
        <div class="mt-8 lg:mt-0">
          <img
            src="/icon/couple.png"
            alt="Couple using Gradsy"
            class="w-[80%] lg:w-auto mx-auto lg:mx-0"
          />
        </div>
      </div>
    </div>

    <!-- Floating Message Icon -->
    <img
      src="/icon/msg.png"
      class="fixed bottom-4 right-4 w-10 lg:w-12"
      alt="Message Icon"
    />

    <script></script>
  </body>
</html>
