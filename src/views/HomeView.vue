<template>
  <div
    id="HomeView"
    class="w-full bg-white ml-2 rounded-t-xl h-full shadow-sm">
    <div class="border-b">
      <div class="flex items-center justify-between px-4 my-3">
        <IconComponent
          class="-m-2 -ml-2.5"
          iconString="trash"
          iconColor="#636363"
          :iconSize="19"
          hoverColor="hover:bg-gray-200"
          text="Delete selected"
        />
        <div class="text-xs text-gray-500">1-50 of 153</div>
      </div>
    </div>

    <div>
      <MessageRow
        from="john.doe@mail.com"
        subject="Test row 1"
        body="This is the body text"
        time="Jun 20 15:15"
      />
    </div>
  </div>
</template>

<script setup>
import IconComponent from '@/components/IconComponent.vue';
import MessageRow from '@/components/MessageRow.vue';
</script>
