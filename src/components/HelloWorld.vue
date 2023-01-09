<template>
  <div class="video-container">
    <video src="https://pixabay.com/videos/id-145308/" controls autoplay loop></video>
  </div>
  <div class="container">
    <iframe src="https://momento360.com/e/u/662eb3d719344370be3aba5373c53f98?utm_campaign=embed&utm_source=other&heading=0&pitch=0&field-of-view=75&size=medium&display-plan=true" width="80%" height="480"></iframe>
  </div>
</template>


<script>
// import pdfjs from "https://mozilla.github.io/pdf.js/build/pdf.js";
// import "./main.js";

export default {
  name: "PDFViewer"
};
</script>

<style>
  video {
    height: 60vh;
    border: 2px solid black;
  }
  .video-container {
    height: 100vh;
    width: 100vw;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .container {
    margin: 2rem;
    height: 100vh;
    width: 100vw;
    display: flex;
    justify-content: center;
    align-items: center;
  }
</style>
