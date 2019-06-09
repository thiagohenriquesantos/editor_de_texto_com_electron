<template>
  <div class="editor">
    <quill-editor
      v-model="content"
      :options="editorOption"
    ></quill-editor>
  </div>
</template>
<script>
export default {
  name: "Editor",
  data() {
    return {
      content: "",
      editorOption: {}
  },
  methods: {}
};
</script>

<style>
.quill-editor, .quill-code {
  width: 100%;
  height: 90vh;
}

.quill-code {
  height: auto;
  border: none;
}
.quill-code > .title {
  border: 1px solid #ccc;
  border-left: none;
  height: 3em;
  line-height: 3em;
  text-indent: 1rem;
  font-weight: bold;
}
</style>