<template>
    <figure class="snip1157">
      <blockquote>{{testimContent.quote}}
        <div class="arrow"></div>
      </blockquote>
      <img :src="testimContent.author.img" alt="sq-sample3" />
      <div class="author">
        <h5>{{testimContent.author.name}} <span> {{testimContent.author.description}}</span></h5>
      </div>
  </figure>
</template>

<script>
export default {
    props: ['testimContent']
}
</script>

<style lang="scss" scoped>
  @import url(https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css);
  @import url(https://fonts.googleapis.com/css?family=Raleway:400,800);
  figure.snip1157 {
    font-family: 'Raleway', Arial, sans-serif;
    position: relative;
    float: left;
    overflow: hidden;
    min-width: 220px;
    max-width: 450px;
    width: 100%;
    color: #333;
    text-align: left;
    box-shadow: none !important;
  }
  figure.snip1157 * {
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
    -webkit-transition: all 0.35s cubic-bezier(0.25, 0.5, 0.5, 0.9);
    transition: all 0.35s cubic-bezier(0.25, 0.5, 0.5, 0.9);
  }
  figure.snip1157 img {
    max-width: 100%;
    vertical-align: middle;
    height: 90px;
    width: 90px;
    border-radius: 50%;
    margin: 30px 0 0 10px;
  }
  figure.snip1157 blockquote {
    display: block;
    border-radius: 8px;
    position: relative;
    background-color: #fafafa;
    padding: 25px 50px 30px 50px;
    font-size: 0.8em;
    font-weight: 500;
    margin: 0;
    line-height: 1.6em;
    font-style: italic;
  }
  figure.snip1157 blockquote:before,
  figure.snip1157 blockquote:after {
    font-family: 'FontAwesome';
    content: "\201C";
    position: absolute;
    font-size: 50px;
    opacity: 0.3;
    font-style: normal;
  }
  figure.snip1157 blockquote:before {
    top: 25px;
    left: 20px;
  }
  figure.snip1157 blockquote:after {
    content: "\201D";
    right: 20px;
    bottom: 0;
  }
  figure.snip1157 .arrow {
    top: 100%;
    width: 0;
    height: 0;
    border-left: 0 solid transparent;
    border-right: 25px solid transparent;
    border-top: 25px solid #fafafa;
    margin: 0;
    position: absolute;
  }
  figure.snip1157 .author {
    position: absolute;
    bottom: 45px;
    padding: 0 10px 0 120px;
    margin: 0;
    text-transform: uppercase;
    color: #000;
    -webkit-transform: translateY(50%);
    transform: translateY(50%);
  }
  figure.snip1157 .author h5 {
    opacity: 0.8;
    margin: 0;
    font-weight: 800;
  }
  figure.snip1157 .author h5 span {
    font-weight: 400;
    text-transform: none;
    padding-left: 5px;
  }

  @media (max-width: 900px) {
      figure.snip1157 {
          margin: 3% 1%;
  }
}

</style>
