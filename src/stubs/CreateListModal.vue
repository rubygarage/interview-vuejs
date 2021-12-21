<template>
  <div>
    <a-button
      :style="{ marginBottom: '40px' }"
      type="link"
      @click="onOpenModal"
    >
      My Lists
      <a-icon type="plus" />
    </a-button>

    <a-modal
      :visible="isModalVisible"
      title="Create list"
      okText="Create"
      @ok="handleSubmit"
      @cancel="handleCancel"
    >
      <a-form layout="vertical">
        <a-form-item label="Title">
          <a-input />
        </a-form-item>
        <a-form-item label="Description">
          <a-input />
        </a-form-item>
        <a-form-item class="collection-create-form_last-form-item">
          <a-radio-group
            v-decorator="[
              'modifier',
              {
                initialValue: 'private',
              },
            ]"
          >
            <a-radio value="public">Public</a-radio>
            <a-radio value="private">Private</a-radio>
          </a-radio-group>
        </a-form-item>
      </a-form>
    </a-modal>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ModalText: "Content of the modal",
      isModalVisible: false,
    };
  },
  methods: {
    onOpenModal() {
      this.isModalVisible = true;
    },
    handleSubmit() {
      //TODO:
    },
    handleCancel() {
      //TODO:
    },
  },
};
</script>
