<template>
  <div>
    <header>
      <div class="wrapper">
        <a class="logo" href="/">The Kaiser Zone</a>
        <nav class="social">
          <a
            href="https://twitter.com/honzikec"
            target="_blank"
          ><img :src="twitter" /></a>
          <a
            href="https://github.com/honzikec"
            target="_blank"
          ><img :src="github" /></a>
        </nav>
      </div>
    </header>
    <div class="wrapper">
      <nuxt />
    </div>
  </div>
</template>

<style>
body,
html {
  margin: 0;
  padding: 0;
}
body {
  font-family: "Bitter", serif;
  font-size: 1.1rem;
  line-height: 2rem;
  background: #f8f8f8;
}
.wrapper {
  margin: 0 auto;
  max-width: 1024px;
  padding: 2rem;
}

header {
  display: block;
  background: #fff;
  padding: 1rem 0;
}

header .logo {
  font-weight: bold;
  font-size: 1.5rem;
  line-height: 2.4rem;
}

header:after {
  content: "";
  clear: both;
  display: table;
}

header .social {
  float: right;
}

header .social a {
  display: block;
  float: left;
  margin-left: 1rem;
  padding: .5rem 0 0.25rem 0;
}

header .wrapper {
  padding-top: 0;
  padding-bottom: 0;
}

a {
  color: #2672af;
}

a:hover {
  color: #317fbe;
}

blockquote {
  border-left: 10px solid #ccc;
  margin: 1.5rem 0;
  padding: 1rem 20px;
  quotes: "\201C""\201D""\2018""\2019";
  font-style: italic;
  font-size: 1.25rem;
}
blockquote:before {
  color: #ccc;
  content: open-quote;
  font-size: 4em;
  line-height: 0.1em;
  margin-right: 0.25em;
  vertical-align: -0.4em;
}
blockquote p {
  display: inline;
}
figure {
  display: block;
  margin: 2rem 0;
}
figure figcaption {
  color: grey;
  font-style: italic;
}

/* Headings */
h1,
h2,
h3,
h4,
h5,
h6 {
  /* Change heading typefaces here */
  margin-top: 1.5rem;
  margin-bottom: 0;
  line-height: 1.5rem;
}
h1 {
  font-size: 3rem;
  line-height: 4.5rem;
  margin-top: 3rem;
}
h2 {
  font-size: 2rem;
  line-height: 3rem;
  margin-top: 3rem;
}
h3 {
  font-size: 1.414rem;
}
h4 {
  font-size: 0.707rem;
}
h5 {
  font-size: 0.4713333333333333rem;
}
h6 {
  font-size: 0.3535rem;
}
/* Copy & Lists */
p {
  line-height: 2rem;
  margin-top: 1.5rem;
  margin-bottom: 0;
}
ul,
ol {
  margin-top: 1.5rem;
  margin-bottom: 1.5rem;
}
ul li,
ol li {
  line-height: 1.8rem;
  margin-top: 0.5rem;
  margin-bottom: 0.5rem;
}
ul ul,
ol ul,
ul ol,
ol ol {
  margin-top: 0;
  margin-bottom: 0;
}
/* Tables */
table {
  margin-top: 1.5rem;
  border-spacing: 0px;
  border-collapse: collapse;
}
table td,
table th {
  padding: 0;
  line-height: 33px;
}
/* Code blocks */
code {
  vertical-align: bottom;
}

.sources {
  border-top: 5px solid #ccc;
  margin-top: 3rem;
}
</style>

<script>
import twitter from '~/assets/twitter.svg'
import github from '~/assets/github.svg'
export default {
  data: () => ({
    twitter,
    github
  })
}
</script>
