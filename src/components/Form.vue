<script setup>
  import { ref } from 'vue';
  import { PlusIcon } from '@heroicons/vue/20/solid'
  import { SparklesIcon } from '@heroicons/vue/20/solid'
  import { Cog8ToothIcon } from '@heroicons/vue/20/solid'
  import { XMarkIcon } from '@heroicons/vue/20/solid'
  import { BarsArrowUpIcon } from '@heroicons/vue/20/solid'
  import { UsersIcon } from '@heroicons/vue/20/solid'
  import { ChevronUpDownIcon } from '@heroicons/vue/20/solid'
</script>
<template>
  <form class="mx-auto w-full max-w-2xl bg-white rounded-lg">
    <div>
      <div class="border-b border-gray-200 px-4 py-5 sm:px-6">
        <div class="-ml-4 -mt-2 flex flex-wrap items-center justify-between sm:flex-nowrap">
          <div class="ml-4 mt-2">
            <h3 class="text-base font-semibold leading-6 text-gray-900">Add a new interview</h3>
          </div>
          <div class="ml-4 mt-2 flex gap-x-3 items-center">
            <button type="button" class="rounded-full bg-[#f18024] px-4 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-[#de6b0e] focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-[#f18024]">Settings</button>
            <XMarkIcon class="h-8 w-8 text-gray-400" aria-hidden="true" />
          </div>
        </div>
      </div>
      <div class="space-y-8">
        <div class="grid grid-cols-1 pt-5 px-4 sm:px-6 gap-x-8 md:grid-cols-3">
          <div class="col-span-full relative">
            <label for="website" class="absolute -top-2 left-2 bg-white px-1 block text-xs font-medium leading-6 text-gray-900">Interview Topic</label>
            <div class="mt-2">
              <div class="flex rounded-md shadow-sm ring-1 ring-inset ring-gray-300 focus-within:ring-2 focus-within:ring-inset focus-within:ring-[#f18024]">
                <input type="text" name="website" id="website" class="block flex-1 border-0 bg-transparent py-1.5 pl-2 text-gray-900 placeholder:text-gray-400 focus:ring-0 sm:text-sm sm:leading-6" placeholder="www.example.com" />
              </div>
            </div>
          </div>
        </div>
        <!--  -->
        <div class="grid grid-cols-1 px-4 sm:px-6 gap-x-8 md:grid-cols-3">
          <div class="col-span-full">
            <div class="relative">
              <div class="absolute inset-0 flex items-center" aria-hidden="true">
                <div class="w-full border-t border-gray-300" />
              </div>
            </div>
          </div>
        </div>
        <!--  -->
        <div class="grid grid-cols-1 px-4 sm:px-6 gap-x-8 md:grid-cols-3 items-center">
          <div class="col-span-2">
            <label for="questions" class="block text-sm font-medium leading-6 text-gray-900">Questions</label>
          </div>
          <div class="col-span-1 gap-x-3 justify-end inline-flex">
            <button type="button" class="rounded-full bg-[#f18024] px-4 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-[#de6b0e] focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-[#f18024]">
              <SparklesIcon class="h-5 w-5" aria-hidden="true" />
            </button>
            <button type="button" class="rounded-full bg-[#f18024] px-4 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-[#de6b0e] focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-[#f18024]">
              <PlusIcon class="h-5 w-5" aria-hidden="true" />
            </button>
          </div>
        </div>
        <!--  -->
        <!--  -->
        <div class="grid grid-cols-1 px-4 sm:px-6 gap-x-8 md:grid-cols-3">
          <div class="col-span-full">
            <div class="relative">
              <div class="absolute inset-0 flex items-center" aria-hidden="true">
                <div class="w-full border-t border-gray-300" />
              </div>
            </div>
          </div>
        </div>
        <!--  -->
        <div  class="grid grid-cols-1 px-4 sm:px-6 gap-x-8 md:grid-cols-3 div-clone">
          <div class="col-span-full">
            <div class="mt-2 flex rounded-md items-center">
              <ChevronUpDownIcon class="size-6 drag-trigger" />
              <div class="relative flex flex-grow items-stretch focus-within:z-10">
                <input type="text" class="block w-full rounded-none rounded-l-md border-0 py-1.5 pl-2 text-gray-900 ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-1 focus:ring-inset focus:ring-[#f18024] sm:text-sm sm:leading-6" placeholder="John Smith" />
              </div>
              <button type="button" class="relative -ml-px inline-flex items-center gap-x-1.5 rounded-r-full px-3 py-2 text-sm text-[#f18024] hover:text-white hover:bg-[#f18024] ring-inset ring-1 ring-[#f18024]">
                <Cog8ToothIcon class="size-5" />
              </button>
              <XMarkIcon class="size-6 delete-input-group"/>
            </div>
          </div>
        </div>
        <!--  -->
        <div class="grid grid-cols-1 px-4 sm:px-6 gap-x-8 md:grid-cols-3">
          <div class="col-span-full">
            <div class="relative">
              <div class="absolute inset-0 flex items-center" aria-hidden="true">
                <div class="w-full border-t border-gray-300" />
              </div>
              <div class="relative flex justify-center">
                <span class="bg-white px-2 text-sm text-gray-500">Link to the interview</span>
              </div>
            </div>
          </div>
        </div>
        <!--  -->
        <!--  -->
        <div class="grid grid-cols-1 px-4 sm:px-6 gap-x-8 md:grid-cols-3">
          <div class="col-span-full relative">
            <label for="email" class="absolute -top-2 left-2 bg-white px-1 z-20 block text-xs font-medium leading-6 text-gray-900">Interview URL</label>
            <div class="mt-2 flex rounded-md items-center">
              <div class="relative flex flex-grow items-stretch focus-within:z-10">
                <input type="email" name="email" id="email" class="block w-full rounded-none rounded-l-md border-0 py-1.5 pl-2 text-gray-900 ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-1 focus:ring-inset focus:ring-[#f18024] sm:text-sm sm:leading-6" placeholder="John Smith" />
              </div>
              <button type="button" class="relative -ml-px inline-flex items-center gap-x-1.5 rounded-r-full px-3 py-2 text-sm text-[#f18024] hover:text-white hover:bg-[#f18024] ring-inset ring-1 ring-[#f18024]">
                Save and Get URL
              </button>
            </div>
          </div>
        </div>
        <!--  -->
      <div class="grid grid-cols-1 px-4 sm:px-6 gap-x-8 md:grid-cols-3">
        <div class="col-span-full">
          <div class="relative">
            <div class="absolute inset-0 flex items-center" aria-hidden="true">
              <div class="w-full border-t border-gray-300" />
            </div>
            <div class="relative flex justify-center">
              <span class="bg-white px-2 text-sm text-gray-500">Send by email</span>
            </div>
          </div>
        </div>
      </div>
      <!--  -->
      <div class="grid grid-cols-1 px-4 py-5 sm:px-6 gap-x-8 md:grid-cols-3">
        <div class="col-span-2 relative">
          <label for="about" class="absolute -top-2 left-2 bg-white px-1 block text-xs font-medium leading-6 text-gray-900">Candidates' email addresses. One per line</label>
          <div class="mt-2">
            <textarea id="about" name="about" rows="3" class="px-2 block w-full rounded-md border-0 py-1.5 text-gray-900 shadow-sm ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-[#f18024] sm:text-sm sm:leading-6" />
          </div>
          
        </div>
        <div class="col-span-1 justify-end gap-y-1 md:flex flex-wrap items-start">
          <div class="flex gap-x-3 items-center">
            <label for="location" class="block text-sm font-medium leading-6 text-gray-900">language</label>
            <select id="location" name="location" class="mt-2 block w-full rounded-md border-0 py-1.5 pl-3 pr-10 text-gray-900 ring-1 ring-inset ring-gray-300 focus:ring-2 focus:ring-[#f18024] sm:text-sm sm:leading-6">
              <option selected="">Eng</option>
            </select>
          </div>
          <button type="button" class="rounded-full bg-[#fff] border border-[#f18024] px-4 py-2.5 text-sm font-semibold text-[#f18024] hover:text-white shadow-sm hover:bg-[#de6b0e] focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-[#f18024]">Send by email</button>
        </div>
      </div>
      
      </div>
      </div>

    <div class="mt-6 flex items-center justify-end gap-x-3 border-t border-gray-300 px-4 py-5">
      <button type="button" class="rounded-full bg-[#fff] px-4 py-2.5 text-sm font-semibold text-[#f18024] hover:text-white shadow-sm hover:bg-[#f18024] border-2 border-[#f18024] focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-[#f2f2f2] mt-3">Cancel</button>
      <button type="submit" class="rounded-full bg-[#f18024] px-4 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-[#de6b0e] focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-[#f18024] mt-3">Save</button>
    </div>
  </form>
</template>
