<script setup>
defineProps({
  name: {
    type: String,
    required: true,
  },
  title: {
    type: String,
  },
});
</script>

<template>
  <svg
    v-if="name === 'circle'"
    viewBox="0 0 24 24"
    xmlns="http://www.w3.org/2000/svg"
  >
    <title>Add one node</title>

    <path
      d="M12,2A10,10 0 0,0 2,12A10,10 0 0,0 12,22A10,10 0 0,0 22,12A10,10 0 0,0 12,2Z"
    />
  </svg>

  <svg
    v-else-if="name === 'multiple'"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 24 24"
  >
    <title>Add multiple node</title>
    <path
      d="M13,14C9.64,14 8.54,15.35 8.18,16.24C9.25,16.7 10,17.76 10,19A3,3 0 0,1 7,22A3,3 0 0,1 4,19C4,17.69 4.83,16.58 6,16.17V7.83C4.83,7.42 4,6.31 4,5A3,3 0 0,1 7,2A3,3 0 0,1 10,5C10,6.31 9.17,7.42 8,7.83V13.12C8.88,12.47 10.16,12 12,12C14.67,12 15.56,10.66 15.85,9.77C14.77,9.32 14,8.25 14,7A3,3 0 0,1 17,4A3,3 0 0,1 20,7C20,8.34 19.12,9.5 17.91,9.86C17.65,11.29 16.68,14 13,14M7,18A1,1 0 0,0 6,19A1,1 0 0,0 7,20A1,1 0 0,0 8,19A1,1 0 0,0 7,18M7,4A1,1 0 0,0 6,5A1,1 0 0,0 7,6A1,1 0 0,0 8,5A1,1 0 0,0 7,4M17,6A1,1 0 0,0 16,7A1,1 0 0,0 17,8A1,1 0 0,0 18,7A1,1 0 0,0 17,6Z"
    />
  </svg>

  <svg
    v-else-if="name === 'trash'"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 24 24"
  >
    <title>Delete the node</title>
    <path
      d="M9,3V4H4V6H5V19A2,2 0 0,0 7,21H17A2,2 0 0,0 19,19V6H20V4H15V3H9M9,8H11V17H9V8M13,8H15V17H13V8Z"
    />
  </svg>

  <svg
    v-else-if="name === 'play'"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 24 24"
  >
    <title>play</title>
    <path d="M8,5.14V19.14L19,12.14L8,5.14Z" />
  </svg>

  <svg
    v-else-if="name === 'chevronDown'"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 24 24"
  >
    <title>{{ title }}</title>
    <path d="M7.41,8.58L12,13.17L16.59,8.58L18,10L12,16L6,10L7.41,8.58Z" />
  </svg>

  <svg
    v-else-if="name === 'chevronUp'"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 24 24"
  >
    <title>{{ title }}</title>
    <path d="M7.41,15.41L12,10.83L16.59,15.41L18,14L12,8L6,14L7.41,15.41Z" />
  </svg>

  <svg
    v-else-if="name === 'messageText'"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 24 24"
  >
    <title>message-text</title>
    <path
      d="M20,2H4A2,2 0 0,0 2,4V22L6,18H20A2,2 0 0,0 22,16V4A2,2 0 0,0 20,2M6,9H18V11H6M14,14H6V12H14M18,8H6V6H18"
    />
  </svg>

  <svg
    v-else-if="name === 'edit'"
    xmlns="http://www.w3.org/2000/svg"
    viewBox="0 0 24 24"
  >
    <title>Edit branch Name</title>
    <path
      d="M20.71,7.04C21.1,6.65 21.1,6 20.71,5.63L18.37,3.29C18,2.9 17.35,2.9 16.96,3.29L15.12,5.12L18.87,8.87M3,17.25V21H6.75L17.81,9.93L14.06,6.18L3,17.25Z"
    />
  </svg>
</template>
