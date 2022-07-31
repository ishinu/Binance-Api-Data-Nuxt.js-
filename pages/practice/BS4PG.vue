<template>
    <div>
        <p class="fw-bold">Bold text.</p>
<p class="fw-bolder">Bolder weight text (relative to the parent element).</p>
<p class="fw-normal">Normal weight text.</p>
<p class="fw-light">Light weight text.</p>
<p class="fw-lighter">Lighter weight text (relative to the parent element).</p>
<p class="fst-italic">Italic text.</p>
<p class="fst-normal">Text with normal font style</p>
    </div>
</template>

<script>
    export default {
        data() {
            return { 

            }
        },
        methods : {

        }
    }
</script>

<style>
    .progress-bar-vertical {
  width: 1px;
  min-height: 400px;
  margin-right: 20px;
  float: left;
  display: -webkit-box;  /* OLD - iOS 6-, Safari 3.1-6, BB7 */
  display: -ms-flexbox;  /* TWEENER - IE 10 */
  display: -webkit-flex; /* NEW - Safari 6.1+. iOS 7.1+, BB10 */
  display: flex;         /* NEW, Spec - Firefox, Chrome, Opera */
  /* align-items: flex-end;
  -webkit-align-items: flex-end; Safari 7.0+ */
}

.progress-bar-vertical .progress-bar {
  width: 100%;
  height: 0;
  -webkit-transition: height 0.6s ease;
  -o-transition: height 0.6s ease;
  transition: height 0.6s ease;
}
</style>