<template>
  <a-card
    hoverable
    title="Card title"
    :style="{ marginBottom: '20px' }"
  >
    <p>card content</p>
    <template #actions>
      <a-icon type="delete" />
    </template>
  </a-card>
</template>
