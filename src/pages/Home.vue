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
            I am a Software Developer based in Boise, Idaho. I enjoy working
            with Vue.js, Node.js, C#, .Net, and MongoDB. I also hold an
            Associates of Arts Degree in Information Technology from The
            University of Phoenix.
          </h5>
          <h5 class="mt-5">
            I wanted to learn software development because I grew up playing
            video games and watching computers and the internet evolve, and have
            never been able to escape the curiousity for computers and how they
            work. Alongside software development and video games, I love cars,
            animals, finding new music, athletic activities, and challenging
            myself to learn new skills.
          </h5>
          <h5 class="mt-5">
            Software development has given me a hunger to learn as much as I
            can, so I can sharpen my skills and become a master at my craft. I'm
            looking forward to learning as much as I can as well as applying my
            skills to continue to build applications that I am proud of.
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
          class="contents card text-center mx-3 my-2"
          href="https://bug-log89.herokuapp.com/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <img class="appImg" src="../assets/BugLogImg.png" alt="" />
          <div class="overlay text-center p-1">
            <h4>Bug-Log</h4>
            <h5>Vue.js, Node.js, MongoDB</h5>
            <p>
              Bug tracker app where users can login, open bugs, add comments,
              edit bugs and comments, and close bugs.
            </p>
          </div>
        </a>
        <a
          class="contents card text-center mx-3 my-2"
          href="https://keepr20.herokuapp.com/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <img class="appImg" src="../assets/KeeprImg.png" alt="" />
          <div class="overlay text-center p-1">
            <h4>Keepr</h4>
            <h5>Vue.js, .Net, MongoDB</h5>
            <p>
              App where users can log in, add images(keeps) and save others'
              images to their own public or private vaults.
            </p>
          </div>
        </a>
        <a
          class="contents card text-center mx-3 my-2"
          href="https://petpal7.herokuapp.com/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <img class="appImg" src="../assets/PetPalImg.png" alt="" />
          <div class="overlay text-center p-1">
            <h4>Pet-Pal</h4>
            <h5>Vue.js, Node.js, MongoDB</h5>
            <p>
              Mobile card swiping app for adopting pets. Utilizes nationwide
              shelter data from an API to help users find pets in their area.
            </p>
          </div>
        </a>
        <a
          class="contents card text-center mx-3 my-2"
          href="https://joealmanza.github.io/soulclicker/"
          target="_blank"
          rel="noopener noreferrer"
        >
          <img class="appImg" src="../assets/SoulClicker.png" alt="" />
          <div class="overlay text-center p-1">
            <h4>Soul Clicker</h4>
            <h5>Vue.js</h5>
            <p>
              Simple clicker/idle game based off of one of my favorite video
              games, Dark Souls. Click the dragon to acquire souls, then use
              those to buy weapons and spells to increase soul intake.
            </p>
          </div>
        </a>
        <h5 class="col-12 text-center mt-5">
          Check out these and all my other projects here!
        </h5>
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
          <h5 class="my-5">
            Any comments or questions, feel free to reach out!
          </h5>
        </div>

        <div class="col-lg-3 pt-4 mx-0 text-center">
          <a class="my-4" :href="'mailto:JoeAlmanza2113@gmail.com'">
            <i
              class="fa fa-envelope-o contactImg text-secondary"
              aria-hidden="true"
            ></i>
            <br />
            <h5 class="text-info">JoeAlmanza2113@gmail.com</h5>
          </a>
        </div>

        <div class="col-lg-3 pt-4 mx-0 text-center">
          <a
            class="my-4"
            onclick="location.href='https://www.linkedin.com/in/joseph-almanza/';"
          >
            <i
              class="fa fa-linkedin-square contactImg text-secondary"
              aria-hidden="true"
            ></i>
            <br />
            <h5>LinkedIn</h5>
          </a>
        </div>

        <div class="col-lg-3 pt-4 mx-0 text-center">
          <a
            class="my-4"
            onclick="location.href='https://joealmanza.github.io/Joe-Almanza/';"
          >
            <i
              class="fa fa-file-text-o contactImg text-secondary"
              aria-hidden="true"
            ></i>
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
  max-width: 100%;
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
  box-shadow: 9px 9px 18px #020212, -9px -9px 18px #060836;
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
