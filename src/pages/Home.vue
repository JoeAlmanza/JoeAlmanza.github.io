<template>
  <div class="home">
    <div
      class="container-fluid bg-image"
      data-spy="scroll"
      data-target="#navbar"
      data-offset="0"
    >
      <div class="row justify-content-center align-items-center mainRow">
        <div class="col-lg-10 d-flex justify-content-center">
          <h1 class="text-center text-light">
            <strong> Full-Stack Software Developer </strong>
          </h1>
        </div>
      </div>
      <div class="row justify-content-center aboutRow" id="about">
        <div class="col-lg-7 text-center">
          <h2 class="mb-0">About Me</h2>
          <h2 class="">_____</h2>
          <h5 class="mt-5">
            Joe is a Software Developer who was born and raised in Idaho. His
            background in Escrow has ingrained a strong sense of importance when
            it comes to communication, meeting deadlines, thoroughly completing
            tasks, and providing client satisfaction by keeping them informed
            while managing hundreds of thousands of their dollars. While Escrow
            provided a sense of accomplishment when helping people buy or sell
            property, Joe has never been able to escape the curiousity for
            software development that comes with being a long time gamer, and
            growing up watching computers and the internet grow exponentially.
            Alongside Software Development and video games, Joe also loves
            animals, cars, clothes, sneakers and fitness. Joe also holds an
            Associates of Arts Degree in Information Technology from The
            University of Phoenix.
          </h5>
        </div>
      </div>

      <div class="row justify-content-center skillsRow" id="skills">
        <h2 class="col-12 mb-2 text-center">
          Technologies and Tools
        </h2>
        <img src="../assets/Icons2.png" class="mt-4" alt="" />
      </div>

      <div class="row justify-content-center appRow" id="portfolio">
        <h2 class="col-12 mb-5 text-center">Applications</h2>
        <a
          class="contents card text-center mx-5 my-2"
          href="https://bug-log89.herokuapp.com/"
        >
          <img class="appImg" src="../assets/BugLogImg.png" alt="" />
          <div class="overlay text-center p-1">
            <h4 class="">Bug-Log</h4>
            <h5>Vue.js, Node.js, MongoDB</h5>
            <p>
              Bug tracker app where users can login, open bugs, add comments,
              edit bugs and comments, and close bugs.
            </p>
          </div>
        </a>
        <a
          class="contents card text-center mx-5 my-2"
          href="https://keepr20.herokuapp.com/"
        >
          <img class="appImg" src="../assets/KeeprImg.png" alt="" />
          <div class="overlay text-center p-1">
            <h4 class="">Keepr</h4>
            <h5>Vue.js, .Net, MongoDB</h5>
            <p>
              App where users can log in, add images(keeps) and save others'
              images to public or private vaults.
            </p>
          </div>
        </a>
        <a
          class="contents card text-center mx-5 my-2"
          href="https://petpal7.herokuapp.com/"
        >
          <img class="appImg" src="../assets/PetPalImg.png" alt="" />
          <div class="overlay text-center p-1">
            <h4 class="">Pet-Pal</h4>
            <h5>Vue.js, Node.js, MongoDB</h5>
            <p>
              Card swiping app utilizing nationwide shelter data to help users
              find adoptable pets in their area and contact the shelters holding
              the pets.
            </p>
          </div>
        </a>
        <h5 class="col-12 text-center mt-5">Check out all my projects here!</h5>
        <input
          type="button"
          class="btn btn-outline-secondary"
          onclick="location.href='https://github.com/JoeAlmanza';"
          value="My Github!"
        />
      </div>

      <div class="row justify-content-center contactRow" id="contact">
        <div class="col-12 text-center">
          <h2>Contact Me!</h2>
          <h5 class="my-5">If you like what you see, let me know!</h5>
        </div>
        <div class="col-4 pt-4 mx-0 text-center">
          <a class="my-4" :href="'mailto:JoeAlmanza2113@gmail.com'">
            <i
              class="fa fa-envelope-o contactImg text-secondary"
              aria-hidden="true"
            ></i>
            <br />
            <h5 class="text-secondary">JoeAlmanza2113@gmail.com</h5>
          </a>
        </div>

        <div class="col-4 pt-4 mx-0 text-center">
          <a
            class="my-4"
            onclick="location.href='https://joealmanza.github.io/Joe-Almanza/';"
          >
            <i class="fa fa-file-text-o contactImg" aria-hidden="true"></i>
            <br />
            <h5 class="">Resume & More Info...</h5>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
};
</script>
<style>
strong {
  font-size: 4rem;
  text-shadow: 2px 2px black;
}
.mainRow {
  height: 100vh;
  background-image: url("../assets/kb-bg.jpg");
  background-position: center center;
  background-size: cover;
}
.aboutRow {
  background-color: #040524;
  color: #a8ccdd;
  padding-top: 6rem;
  padding-bottom: 7rem;
}
.skillsRow {
  color: #040524;
  padding-top: 5rem;
  padding-bottom: 4rem;
}
img {
  max-height: 40vh;
}
.appRow {
  background-color: #040524;
  color: #a8ccdd;
  padding-top: 6rem;
  padding-bottom: 6rem;
}
.appImg {
  max-height: 12rem;
  max-width: 25rem;
}
.overlay {
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  opacity: 0;
  transition: 0.5s ease;
  background-color: #040607b9;
  color: #a8ccdd;
  text-shadow: 1px 1px black;
}
.contents:hover .overlay {
  opacity: 1;
}
.contactRow {
  background-color: #000000;
  color: #a8ccdd;
  padding-top: 5rem;
  padding-bottom: 5rem;
}
.contactImg {
  font-size: 3em;
}
a {
  cursor: pointer;
}
</style>
