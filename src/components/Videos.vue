<template>
  <section id="videos" class="container mx-auto my-6 p-4 max-w-4xl">
    <div class="mb-6">
      <h2 class="text-2xl font-bold mb-2">Videos</h2>
      <p>
        A collection of videos on my experience in project management.
      </p>
    </div>
    <div class="mb-6">
      <h3 class="text-xl font-semibold mb-4">Final Project</h3>
      <div class="video-wrapper">
        <iframe
          width="560"
          height="315"
          src="https://www.youtube.com/embed/P2y1m7AcDEg"
          frameborder="0"
          allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>
    </div>
    <div class="mb-6">
      <h3 class="text-xl font-semibold mb-4">Project Approach</h3>
      <div class="video-wrapper">
        <iframe
          width="560"
          height="315"
          src="https://www.youtube.com/embed/Xjyv-ndNAZ0"
          frameborder="0"
          allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>
    </div>
    <div class="mb-6">
      <h3 class="text-xl font-semibold mb-4">Tools Used</h3>
      <div class="video-wrapper">
        <iframe
          width="560"
          height="315"
          src="https://www.youtube.com/embed/PK-t58DLFu0"
          frameborder="0"
          allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>
    </div>
  </section>
</template>

<style>
.video-wrapper {
  position: relative;
  padding-bottom: 56.25%;
  height: 0;
}

.video-wrapper iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
</style>
