<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Gradsy Register</title>
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"
    />

    <!-- Import Poppins Font -->
    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600&display=swap"
      rel="stylesheet"
    />

    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- Apply Poppins font in Tailwind -->
    <style>
      body {
        font-family: "Poppins", sans-serif;
      }
    </style>
  </head>
  <body class="bg-gray-100 flex items-center justify-center min-h-screen">
    <!-- Container -->
    <div class="w-full max-w-lg bg-white shadow-md rounded-lg p-8">
      <!-- Logo -->
      <div class="flex justify-center mb-6">
        <img src="/icon/About.png" alt="Gradsy Logo" class="h-16" />
      </div>

      <!-- Registration Form -->
      <form action="#" method="POST">
        <!-- Name Fields -->
        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
          <!-- First Name -->
          <div>
            <label for="first_name" class="block text-gray-700"
              >First Name</label
            >
            <input
              type="text"
              id="first_name"
              name="first_name"
              placeholder="First Name"
              class="w-full p-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-400"
            />
          </div>
          <!-- Last Name -->
          <div>
            <label for="last_name" class="block text-gray-700">Last Name</label>
            <input
              type="text"
              id="last_name"
              name="last_name"
              placeholder="Last Name"
              class="w-full p-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-400"
            />
          </div>
        </div>

        <!-- Username -->
        <div class="mt-4">
          <label for="username" class="block text-gray-700"
            >Create Username</label
          >
          <input
            type="text"
            id="username"
            name="username"
            placeholder="Username"
            class="w-full p-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-400"
          />
        </div>

        <!-- Email -->
        <div class="mt-4">
          <label for="email" class="block text-gray-700">Email</label>
          <input
            type="email"
            id="email"
            name="email"
            placeholder="Enter Your Email"
            class="w-full p-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-400"
          />
        </div>

        <!-- Password -->
        <div class="mt-4 relative">
          <label for="password" class="block text-gray-700"
            >Create Password</label
          >
          <input
            type="password"
            id="password"
            name="password"
            placeholder="Create Password"
            class="w-full p-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-400"
          />
          <span
            class="absolute right-3 top-8 cursor-pointer"
            id="password-toggle"
          >
            <i class="fas fa-eye opacity-50" id="password-eye"></i>
          </span>
        </div>

        <!-- Terms & Conditions -->
        <div class="flex items-start mt-6">
          <input
            id="terms"
            name="terms"
            type="checkbox"
            required
            class="focus:ring-indigo-500 h-4 w-4 text-indigo-600 border-gray-300 rounded"
          />
          <label for="terms" class="ml-2 text-sm text-gray-700"
            >I agree to the <a
              href="#"
              class="text-indigo-600 hover:text-indigo-500"
              >Terms & Conditions</a
            >
            and
            <a href="#" class="text-indigo-600 hover:text-indigo-500"
              >Privacy Policy</a
            ></label
          >
        </div>

        <!-- Register Button -->
        <button
          type="submit"
          class="w-full bg-blue-500 text-white p-2 mt-6 rounded-lg hover:bg-blue-600"
          >Register</button
        >
      </form>

      <!-- Login Link -->
      <p class="text-center text-gray-600 mt-4">
        Already have an account? <a
          href="login"
          class="text-blue-500 hover:underline">Log In</a
        >
      </p>

      <!-- OR Sign In With -->
      <div class="flex items-center justify-between mt-6">
        <div class="border-t flex-grow mr-3"></div>
        <span class="text-gray-500">Or Sign In With</span>
        <div class="border-t flex-grow ml-3"></div>
      </div>

      <!-- Social Buttons -->
      <div class="flex justify-center mt-4 space-x-4">
        <a
          href="#"
          class="bg-white border p-2 rounded-lg hover:bg-gray-100 flex items-center"
        >
          <img src="/icon/google.png" alt="Google" class="h-6 w-6" />
        </a>
        <a
          href="#"
          class="bg-white border p-2 rounded-lg hover:bg-gray-100 flex items-center"
        >
          <img src="/icon/github.png" alt="GitHub" class="h-6 w-6" />
        </a>
        <a
          href="#"
          class="bg-white border p-2 rounded-lg hover:bg-gray-100 flex items-center"
        >
          <img src="/icon/linkedin.png" alt="LinkedIn" class="h-6 w-6" />
        </a>
      </div>
    </div>

    <script>
      let passwordInput = document.getElementById("password");
      let passwordToggle = document.getElementById("password-toggle");
      let passwordEye = document.getElementById("password-eye");

      passwordToggle.addEventListener("click", () => {
        if (passwordInput.type === "password") {
          passwordInput.type = "text";
          passwordEye.classList.add("fa-eye-slash");
        } else {
          passwordInput.type = "password";
          passwordEye.classList.remove("fa-eye-slash");
        }
      });
    </script>
  </body>
</html>
