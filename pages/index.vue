<template>
    <div class="container">
      <TheHeader />
      <HomeMainSection />
      <HomeLatestProjectsSection />
      <HomeExperienceSection />
      <HomeLearningJourneySection />
      <HomeEmailSection />
      <TheFooter />
    </div>
</template>

<script>
export default {}
</script>

<style>
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

/* THIS IS THE NEW ONE, NEED TO BREAKDOWN */
* {
    margin: 0;
    padding: 0;
}

body {
    color: #333;
    font-family: 'Lato', sans-serif;
}

.container {
    margin: auto;
    /* background-color: blue; */
    max-width: 1140px;
    min-width: 320px;
    min-height: 100vh;
}

.header-menu {
    background-color: #fff;
    padding: 30px;
}

.left-header-menu {
    /* background-color: blueviolet; */
    display: inline-block;
    padding: 20px;
}

.left-header-menu span {
    font-weight: bold;
    font-size: 15pt;
    letter-spacing: 0.05em;
}

.left-header-menu a {
    text-decoration: none;
    color: #333;
}

.right-header-menu {
    /* background-color: aqua; */
    display: inline-block;
    /* TODO: how to not use float? */
    float: right;
}

.right-header-menu ul li {
    list-style: none;
    display: inline-block;
    padding: 20px;
}

.main-header {
    background-color: #fff;
    /* background-color: rgb(156, 39, 39); */
    height: 340px;
    padding: 0 40px 0 40px;
    position: relative;
}

.left-main-header {
    /* background-color: aqua; */
    display: inline-block;
    top: 50%;
    transform: translate(0, -50%);
    position: absolute;
}

.left-main-header h1 {
    font-size: 99pt;
}

.left-main-header h2 {
    font-size: 51.75pt;
}

.right-main-header {
    /* background-color: yellow; */
    display: inline-block;
    font-size: 18.75pt;
    width: 266px;
    text-align: right;
    top: 50%;
    right: 40px;
    transform: translate(0, -50%);
    position: absolute;
}

.section {
    background-color: #fff;
    /* background-color: rgb(64, 231, 72); */
    padding: 20px 40px;
}

.section-title {
    padding: 15px 0;
}

.section-title h3 {
    font-size: 17pt;
}

.section-title h4 {
    font-size: 14pt;
    font-weight: 500;
}

.section-title-2 {
    text-align: center;
    padding: 0 0 35px 0;
}

.section-title-2 h2 {
    font-weight: 400;
    font-size: 27pt;
}

.section-title-3 {
    text-align: center;
    padding: 0 0 35px 0;
}

.section-title-3 h2 {
    font-weight: 400;
    font-size: 27pt;
}

.section-body {
    /* background-color: aqua; */
    margin-top: 25px;
}

.card-container {
    position: relative;
}

.section-body .card-container {
    /* background-color: rgb(162, 199, 61); */
    display: inline-block;
    width: 32%;
    text-align: center;
}

.section-body .card-container .card {
    margin: 0 auto;
    width: 201px;
    height: 262px;
    /* background-color: #333; */
    border-radius: 5px;
    border: #999 solid 1px;
    position: relative;
    color: #666;
}

.card img {
    width: 100%;
    display: block;
    border-bottom: #ddd solid 1px;
}

.learning-journey-card img {
    width: 100%;
    display: block;
    border-bottom: #ddd solid 1px;
}

.card-title {
    text-align: center;
    position: absolute;
    width: 100%;
    margin-top: 15px;
    font-size: 15pt;
}

.card-description {
    text-align: center;
    position: absolute;
    width: 100%;
    top: 185px;
}

.card-tag {
    text-align: center;
    position: absolute;
    width: 100%;
    bottom: 0;
    font-size: 8pt;
    padding-bottom: 10px;
}

.section-body .card-container:first-child {
    /* background-color: rgb(162, 199, 61); */
    /* display: inline-block; */
    /* width: 33%; */
    text-align: left;
}

.section-body .card-container:first-child .card {
    /* background-color: rgb(162, 199, 61); */
    /* display: inline-block; */
    /* width: 33%; */
    margin: 0;
}

.section-body .card-container:last-child {
    /* background-color: rgb(162, 199, 61); */
    /* display: inline-block; */
    /* width: 33%; */
    /* text-align: right; */
    position: relative;
    height: 264px;
}

.section-body .card-container:last-child .card {
    /* background-color: rgb(162, 199, 61); */
    /* display: inline-block; */
    /* width: 33%; */
    /* text-align: right; */
    position: absolute;
    top: 0;
    right: 0;
}

/* .experience .section-body {
    text-align: center;
} */

.experience .section-body .experience-container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
    padding-bottom: 50px;
    /* justify-content: center; */
}

.experience .section-body .experience-container:last-child {
    width: 53%;
    align-items: center;
    margin: 0 auto;
}

.experience .section-body .flex-center {
    justify-content: space-around;
}

.experience-card {
    display: inline-block;
    /* background-color: antiquewhite; */
    text-align: center;
}

.experience-position {
    word-wrap: break-word;
    width: 210px;
}

.experience-company {
    word-wrap: break-word;
    width: 210px;
}

.card a {
    text-decoration: none;
    color: #666;
}

/* .section-body .experience-container:last-child {
    background-color: #333;
}

.section-body .experience-container:last-child .experience-card {
    background-color: aqua;
    position: absolute;
    right: 0;
    top: 0;
} */

/* .experience-container:last-child {
    height: 201px;
} */

/* .experience-container:last-child .experience-card {
    background-color: #333;
    position: absolute;
    right: 0;
    top: 0;
} */

.learning-journey {
    background-color: #fff;
}

.learning-journey-container {
    display: flex;
    flex-wrap: wrap;
}

.learning-journey-card-container {
    flex-grow: 1;
    flex-basis: 25%;
    padding-bottom: 30px;
}

.learning-journey-card {
    margin: 0 auto;
    width: 187px;
    height: 244px;
    /* background-color: #333; */
    border-radius: 5px;
    border: #999 solid 1px;
}

.email {
    background-color: #fff;
    text-align: center;
}

.connect-text {
    font-size: 16pt;
}

.footer {
    padding: 30px 0 70px 0;
    background-color: #fff;
    text-align: center;
}

.view-all {
    padding: 40px 0;
    text-align: center;
}

.social-media-logo {
    display: inline-block;
    /* height: 44px;
    width: 44px; */
    /* border: #999 solid 1px; */
    margin: 25px;
}

.social-media-logo img {
    height: 44px;
    width: 44px;
}

.learning-journey-card {
    position: relative;
    color: #666;
}

.company-logo {
    position: relative;
    display: inline-block;
    width: 140px;
    height: 140px;
    /* border: #999 solid 1px; */
}

.company-logo img {
    position: absolute;
    width: 140px;
    height: auto;
    left: 0;
    top: 50%;
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
}

.card-2 {
    border-radius: 5px;
    margin: 0 auto;
    width: 80%;
    border: #999 solid 1px;
    margin-bottom: 30px;
    height: 261px;
    text-align: center;
    margin-top: 20px;
}

.card-2 img {
    height: 80%;
    margin-top: 30px;
}

.card-3 {
    display: inline-block;
    border-radius: 5px;
    width: 40%;
    border: #999 solid 1px;
    margin-bottom: 30px;
    height: 261px;
    text-align: center;
    margin-top: 20px;
    margin-left: 105px;
}

.card-3 img {
    height: 80%;
    margin-top: 30px;
}

.project-headline {
    /* text-align: center; */
}

.project-description {
    display: inline-block;
    /* border-radius: 5px; */
    /* margin: 0 auto; */
    width: 20%;
    margin-left: 20px;
    position: absolute;
    text-align: center;
    /* border: #999 solid 1px; */
    /* margin-bottom: 30px; */
    height: 261px;
    /* text-align: center; */
}

.project-description span {
    display: inline-block;
    margin-top: 130px;
    margin-left: 40px;
}

.section-detail {
    padding: 0 145px;
    padding-bottom: 50px;
}

.section-detail .section-body {
    margin-top: 8px;
}

.card-4 {
    border-radius: 5px;
    border: #999 solid 1px;
    height: 300px;
    text-align: center;
}

.card-4 p {
    margin-top: 133px;
}

.photo-gallery {
    display: inline-block;
    border-radius: 5px;
    width: 242px;
    height: 152px;
    border: #999 solid 1px;
    text-align: center;
    margin-bottom: 47px;
    margin-right: 55px;
}

.photo-gallery img {
    height: 60%;
    margin-top: 27px;
    margin-left: 3px;
}

.mr-0 {
    margin-right: 0;
}

.center {
    text-align: center;
}

.company-detail {
    color: #707070;
}

.company-detail .logo {
    display: inline-block;
    border-radius: 5px;
    width: 400px;
    height: 270px;
    border: #999 solid 1px;
    text-align: center;
}

.company-detail .logo img {
    height: 60%;
    margin-top: 47px;
    margin-left: 8px;
}

.company-detail h2 {
    margin-top: 25px;
    font-weight: 400;
    font-size: 24pt;
    letter-spacing: 0.1em;
}

.company-detail h3 {
    margin-top: 10px;
    font-weight: 400;
    font-size: 19pt;
    letter-spacing: 0.1em;
}
</style>
