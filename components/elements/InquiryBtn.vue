<template>
  <div class="fixed bottom-10 right-10 z-50">
    <button
      @click="showModal = true"
      class="bg-green-900 hover:bg-green-800 text-white font-bold py-2 px-4 rounded-full transition-colors duration-300 shadow-lg"
      aria-label="Open inquiry form"
    >
      <img
        src="/assets/images/icons/icon-animal.svg"
        alt="Chatbot icon"
        class="w-6 h-6"
        style="border: 10px solid red"
      />
    </button>
  </div>

  <!-- Inquiry Form Modal -->
  <div
    v-if="showModal"
    class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50"
    @click.self="showModal = false"
  >
    <div class="bg-white rounded-lg p-6 w-96 max-w-md shadow-xl relative">
      <button
        @click="showModal = false"
        class="absolute top-4 right-4 text-gray-500 hover:text-gray-700"
        aria-label="Close form"
      >
        <svg
          class="w-6 h-6"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M6 18L18 6M6 6l12 12"
          />
        </svg>
      </button>

      <h2 class="text-2xl font-bold mb-4 text-center">Inquiry Form</h2>

      <form @submit.prevent="handleSubmit">
        <div class="mb-4">
          <label for="name" class="block text-gray-700 text-sm font-bold mb-2"
            >Name</label
          >
          <input
            type="text"
            id="name"
            v-model="formData.name"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            required
          />
        </div>

        <div class="mb-4">
          <label for="email" class="block text-gray-700 text-sm font-bold mb-2"
            >Email</label
          >
          <input
            type="email"
            id="email"
            v-model="formData.email"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            required
          />
        </div>

        <div class="mb-4">
          <label
            for="message"
            class="block text-gray-700 text-sm font-bold mb-2"
            >Message</label
          >
          <textarea
            id="message"
            v-model="formData.message"
            rows="4"
            class="shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline"
            required
          ></textarea>
        </div>

        <div class="flex justify-end space-x-4">
          <button
            type="button"
            @click="showModal = false"
            class="bg-gray-300 hover:bg-gray-400 text-gray-800 font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
          >
            Cancel
          </button>
          <button
            type="submit"
            class="bg-green-900 hover:bg-green-800 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline"
          >
            Submit
          </button>
        </div>
      </form>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";

const showModal = ref(false);
const formData = ref({
  name: "",
  email: "",
  message: "",
});

const handleSubmit = () => {
  // Here you would typically send the form data to your backend
  console.log("Form submitted:", formData.value);
  // Reset form and close modal
  formData.value = { name: "", email: "", message: "" };
  showModal.value = false;
};
</script>

<style>
/* Add any additional styles if needed */
</style>
