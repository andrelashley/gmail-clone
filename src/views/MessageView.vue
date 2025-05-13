<template>
  <div 
    id="SingleMessageRow"
    class="w-full bg-white ml-2 rounded-t-xl h-full shadow-sm"
    >
    <div 
      class="border-b">
        <div class="flex items-center justify-between px-1.5 py-0.5">
          <div class="flex">
            <router-link to="/email">
              <IconComponent
                iconString="back"
                iconColor="#636363"
                :iconSize="19"
                hoverColor="hover:bg-gray-200"
                text="Back to Inbox"
              />
            </router-link>

            <IconComponent
                iconString="trash"
                iconColor="#636363"
                :iconSize="19"
                hoverColor="hover:bg-gray-200"
                text="Delete"
                class="ml-3"
              />
          </div>
          <div class="text-xs text-gray-500">1 -50 of 153</div>
        </div>
    </div>

    <div class="w-full text-xl ml-20 font-light pt-5">
      Subject
    </div>

    <div class="w-full flex">
      <img
        class="rounded-full mt-8 mx-5 custom-img" 
        src="https://placehold.co/45"
      >
      <div class="w-full my-4 mx-0.6">
        <div class="font-semibold text-sm mt-4 mb-4">
          <div class="w-full flex justify-between items-center">
            <div>john.doe@mail.com</div>
            <div class="mr-5 text-xs font-normal">June 20 15:15</div>
          </div>
          <span class="text-xs text-gray-500 font-normal">to me</span>
        </div>
        <div>Lorem ipsum dolor sit amet, consectetur adipisicing elit.
           Asperiores id obcaecati nemo dolorum delectus earum soluta quod totam 
           ullam rem, sequi atque, reprehenderit iure explicabo ipsam
           laboriosam architecto? Laudantium, qui?
          Lorem ipsum dolor sit amet, consectetur adipisicing elit.
           Asperiores id obcaecati nemo dolorum delectus earum soluta quod totam 
           ullam rem, sequi atque, reprehenderit iure explicabo ipsam
           laboriosam architecto? Laudantium, qui?
           Lorem ipsum dolor sit amet, consectetur adipisicing elit.
           Asperiores id obcaecati nemo dolorum delectus earum soluta quod totam 
           ullam rem, sequi atque, reprehenderit iure explicabo ipsam
           laboriosam architecto? Laudantium, qui?
          </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  // import { toRefs, defineProps } from 'vue'
  import IconComponent from '@/components/IconComponent.vue';
  // import StarOutlineIcon from 'vue-material-design-icons/StarOutline.vue'

  // const props = defineProps({
  //   from: String,
  //   subject: String,
  //   body: String,
  //   time: String,
  // })

  // const { from, subject, body, time } = toRefs(props);

  // let icon = null
</script>

<style lang="scss">
#SingleMessageSection {
  .custom-img {
    width: 40px;
    height: 40px;
  }
}
</style>
