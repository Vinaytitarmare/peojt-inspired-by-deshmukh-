<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Support Page with Sidebar</title>
    <script src="https://cdn.tailwindcss.com"></script>
  </head>

  <body class="bg-gray-100">
    <!-- Sidebar -->
    <div class="flex">
      <!-- Sidebar hidden on small screens -->
      <aside class="w-64 h-screen bg-gray-800 text-white fixed hidden md:block">
        <div class="p-6">
          <h1 class="text-2xl font-bold mb-8">Navigation</h1>
          <ul class="space-y-6">
            <li>
              <a
                href="#"
                class="flex items-center p-2 text-lg hover:bg-gray-700 rounded-lg"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6 mr-3"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M3 12l9-9 9 9M4 10v10a1 1 0 001 1h3m10-11l-9 9m9-9v10a1 1 0 01-1 1h-3m-10 0h.01"
                  />
                </svg>
                Home
              </a>
            </li>
            <!-- Additional Links -->
            <li>
              <a
                href="#"
                class="flex items-center p-2 text-lg hover:bg-gray-700 rounded-lg"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="h-6 w-6 mr-3"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M17 20h5V4a1 1 0 00-1-1h-4m-5 0h-6a1 1 0 00-1 1v16h5M12 9v3m-6 3h6m4 0h6m-6 3h2m-2-4h2"
                  />
                </svg>
                Alumni
              </a>
            </li>
            <!-- More list items -->
          </ul>
        </div>
      </aside>

      <!-- Main content with responsive margin -->
      <div class="md:ml-64 w-full">
        <!-- Mobile menu button -->
        <div class="bg-gray-800 text-white p-4 md:hidden">
          <button id="menu-toggle" class="focus:outline-none">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              />
            </svg>
          </button>
        </div>

        <!-- Header -->
        <header class="bg-white shadow">
          <div class="container mx-auto px-4 py-6">
            <h1 class="text-3xl font-bold text-gray-800">Support Center</h1>
          </div>
        </header>

        <!-- Main content section -->
        <main class="container mx-auto px-4 py-10">
          <!-- Search Bar -->
          <div class="mb-8">
            <input
              type="text"
              placeholder="Search support articles..."
              class="w-full p-3 rounded-lg border border-gray-300 focus:ring focus:ring-indigo-200"
            />
          </div>

          <!-- FAQ Section -->
          <section class="bg-white p-6 rounded-lg shadow-md mb-8">
            <h2 class="text-xl font-bold mb-4">Frequently Asked Questions</h2>
            <ul class="space-y-4">
              <li>
                <h3 class="font-semibold">How can I reset my password?</h3>
                <p class="text-gray-600">
                  To reset your password, go to the login page and click 'Forgot
                  password?'. You’ll receive an email with further instructions.
                </p>
              </li>
              <!-- Other FAQs -->
            </ul>
          </section>

          <!-- Help Articles Section -->
          <section class="bg-white p-6 rounded-lg shadow-md mb-8">
            <h2 class="text-xl font-bold mb-4">Help Articles</h2>
            <!-- Responsive grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
              <article class="border p-4 rounded-lg">
                <h3 class="font-bold">Getting Started with Our Platform</h3>
                <p class="text-gray-600">
                  Learn how to set up your profile and get the most out of our
                  services.
                </p>
                <a href="#" class="text-indigo-500 hover:underline">Read more</a
                >
              </article>
              <!-- More articles -->
            </div>
          </section>

          <!-- Contact Form Section -->
          <section class="bg-white p-6 rounded-lg shadow-md mb-8">
            <h2 class="text-xl font-bold mb-4">Contact Us</h2>
            <form class="space-y-4">
              <div>
                <label for="name" class="block font-medium text-gray-700"
                  >Name</label
                >
                <input
                  type="text"
                  id="name"
                  class="w-full p-3 rounded-lg border border-gray-300 focus:ring focus:ring-indigo-200"
                />
              </div>
              <div>
                <label for="email" class="block font-medium text-gray-700"
                  >Email</label
                >
                <input
                  type="email"
                  id="email"
                  class="w-full p-3 rounded-lg border border-gray-300 focus:ring focus:ring-indigo-200"
                />
              </div>
              <div>
                <label for="message" class="block font-medium text-gray-700"
                  >Message</label
                >
                <textarea
                  id="message"
                  class="w-full p-3 rounded-lg border border-gray-300 focus:ring focus:ring-indigo-200"
                ></textarea>
              </div>
              <button
                type="submit"
                class="w-full bg-indigo-500 text-white p-3 rounded-lg hover:bg-indigo-600"
              >
                Send Message
              </button>
            </form>
          </section>
        </main>

        <!-- Footer Section -->
        <footer class="bg-gray-800 text-white py-6">
          <div class="container mx-auto text-center">
            <p>&copy; 2024 Your Company. All rights reserved.</p>
            <div class="flex justify-center space-x-6 mt-4">
              <a href="#" class="text-gray-400 hover:text-white"
                >Privacy Policy</a
              >
              <a href="#" class="text-gray-400 hover:text-white"
                >Terms of Service</a
              >
              <a href="#" class="text-gray-400 hover:text-white">Contact Us</a>
            </div>
          </div>
        </footer>
      </div>
    </div>

    <!-- Toggle Sidebar Script -->
    <script>
      const menuToggle = document.getElementById("menu-toggle");
      const sidebar = document.querySelector("aside");

      menuToggle.addEventListener("click", () => {
        sidebar.classList.toggle("hidden");
      });
    </script>
  </body>
</html>
