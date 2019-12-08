<template>
  <Layout>

    <h1>About My Book</h1>

    <div class="chapters-container">
      <div v-for="index in Array(81).keys()" class="chapter-pointer">
        <span :data-tooltip="`Chapter ${index + 1}`">{{ index + 1 }}</span>
      </div>
    </div>

    <div class="height-holder"></div>

  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'About the Book'
  }
}
</script>

<style>
.home-links a {
  margin-right: 1rem;
}
body {
  background-image: url("/img/dragon.jpg");
  background-color: #eeddcb;
  background-position: center top;
}
.chapters-container {
  display: flex;
  flex-wrap: wrap;
  justify-content2: space-between;
  border2: solid 1px red;
  width: 220px;
  height: 200px;
  margin: 230px calc(50% - 110px - 20px);
}
.chapter-pointer {
  width: 22px;
  height: 22px;
  text-align: center;
  vertical-align: center;
  font-size: 10px;
  line-height: 20px;
  background-color: #ddccbc;
  border: solid 1px darkgoldenrod;
  border-radius: 50%;
  cursor: pointer;
  margin-top2: 1px;
  margin-right2: 1px;
}
.height-holder {
  height: 30px;
}


/**
 * Tooltip Styles
 */

/* Base styles for the element that has a tooltip */
[data-tooltip],
.tooltip {
  position: relative;
  cursor: pointer;
}

/* Base styles for the entire tooltip */
[data-tooltip]:before,
[data-tooltip]:after,
.tooltip:before,
.tooltip:after {
  position: absolute;
  visibility: hidden;
  -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=0)";
  filter: progid:DXImageTransform.Microsoft.Alpha(Opacity=0);
  opacity: 0;
  -webkit-transition:
          opacity 0.2s ease-in-out,
          visibility 0.2s ease-in-out,
          -webkit-transform 0.2s cubic-bezier(0.71, 1.7, 0.77, 1.24);
  -moz-transition:
          opacity 0.2s ease-in-out,
          visibility 0.2s ease-in-out,
          -moz-transform 0.2s cubic-bezier(0.71, 1.7, 0.77, 1.24);
  transition:
          opacity 0.2s ease-in-out,
          visibility 0.2s ease-in-out,
          transform 0.2s cubic-bezier(0.71, 1.7, 0.77, 1.24);
  -webkit-transform: translate3d(0, 0, 0);
  -moz-transform:    translate3d(0, 0, 0);
  transform:         translate3d(0, 0, 0);
  pointer-events: none;
}

/* Show the entire tooltip on hover and focus */
[data-tooltip]:hover:before,
[data-tooltip]:hover:after,
[data-tooltip]:focus:before,
[data-tooltip]:focus:after,
.tooltip:hover:before,
.tooltip:hover:after,
.tooltip:focus:before,
.tooltip:focus:after {
  visibility: visible;
  -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=100)";
  filter: progid:DXImageTransform.Microsoft.Alpha(Opacity=100);
  opacity: 1;
}

/* Base styles for the tooltip's directional arrow */
.tooltip:before,
[data-tooltip]:before {
  z-index: 1001;
  border: 6px solid transparent;
  background: transparent;
  content: "";
}

/* Base styles for the tooltip's content area */
.tooltip:after,
[data-tooltip]:after {
  z-index: 1000;
  padding: 8px;
  width: 160px;
  background-color: #000;
  background-color: hsla(0, 0%, 20%, 0.9);
  color: #fff;
  content: attr(data-tooltip);
  font-size: 14px;
  line-height: 1.2;
}
</style>
