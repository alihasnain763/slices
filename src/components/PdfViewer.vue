<template>
    <div class="pdf-viewer">
        <canvas ref="canvas" width="800" height="600"></canvas>
    </div>
</template>

<script>
//   import pdfjs from "https://mozilla.github.io/pdf.js/build/pdf.js";
const pdfLink = "https://raw.githubusercontent.com/mozilla/pdf.js/ba2edeae/web/compressed.tracemonkey-pldi-09.pdf";

export default {
    name: "PDFViewer",
    data() {
        return {
            pdfLink: pdfLink,
        };
    },
    mounted() {
        this.loadPDF();
    },
    methods: {
        // async loadPDF() {
        //     try {
        //         // Load the PDF
        //         const loadingTask = pdfjs.getDocument(this.pdfLink);
        //         const pdf = await loadingTask.promise;

        //         // Get the first page of the PDF
        //         const page = await pdf.getPage(1);

        //         // Get the canvas element
        //         const canvas = this.$refs.canvas;

        //         // Get the canvas context
        //         const context = canvas.getContext("2d");

        //         // Set the canvas dimensions to match the PDF page dimensions
        //         const viewport = page.getViewport({ scale: 1 });
        //         canvas.width = viewport.width;
        //         canvas.height = viewport.height;

        //         // Render the PDF page on the canvas
        //         const renderTask = page.render({
        //             canvasContext: context,
        //             viewport: viewport,
        //         });
        //         await renderTask.promise;
        //     } catch (error) {
        //         console.error(error);
        //     }
        // },
    },
};
</script>

<style>
/* Add your own styles here */
</style>
