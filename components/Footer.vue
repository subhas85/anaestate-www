<template>
    <footer class="footer">
      <div class="container mx-auto px-4 py-8 flex flex-col md:flex-row justify-between items-center">
        <div class="copyright">
          &copy; {{ new Date().getFullYear() }} Ana's Estate. All Rights Reserved.
        </div>
        <nav class="social-links">
          <a href="#" class="inline-block mr-4 text-xl text-gray-700 hover:text-green-500">
            <i class="fa fa-facebook"></i>
          </a>
          <a href="#" class="inline-block mr-4 text-xl text-gray-700 hover:text-red-500">
            <i class="fa fa-instagram"></i>
          </a>
          <a href="#" class="inline-block text-xl text-gray-700 hover:text-blue-500">
            <i class="fa fa-twitter"></i>
          </a>
        </nav>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    // ...
  }
  </script>
  
  <style scoped>
  .footer {
    @apply bg-gray-200 text-center md:text-left;
    /* Add a subtle border to the top */
    border-top: 1px solid rgba(0, 0, 0, 0.1);
  }
  
  .copyright {
    @apply mb-4 md:mb-0;
    color: #888; /* Adjust text color as needed */
  }
  
  .social-links {
    @apply mt-4 md:mt-0; /* Add margin-top for mobile */
  }
   
  
  .social-links i {
    @apply transition duration-300 ease-in-out transform hover:scale-110;
  }
  </style>
  