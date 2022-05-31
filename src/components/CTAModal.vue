<template>
  <div>
    <div class="overlay-container">
      <div class="modal-container">
        <header>
          <h1>
              Would you like to <br />
              join <span class="org-title">GirlsCanCode</span><span>?</span>
          </h1>
        </header>
        <article>
          <p class="invite-text">It appears you don't have a community yet</p>
          <ul>
            <li>
              Joining a Propel community gives you access to perks, services,
              and jobs well suited to your career goals.
            </li>
            <li>
              Please note you can’t join more than one community at a time, so
              please choose carefully
            </li>
            <li>
              We encourage you to provide accurate information about your
              background and professional experience, and take that first step to
              apply!
            </li>
          </ul>
        </article>
        <div class="btn-container">
            <a href="#">Join a different community</a>
            <button>Join GirlsCanCode</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  active: Boolean,
});
</script>

<style scoped>
header {
  font-family: Gilroy, sans-serif;
  line-height: 1;
  background-color: var(--blue-50);
}

h1 {
  padding-top: 24px;
  padding: 24px 28px;
  font-size: var(--text-h1);
}

h1 .org-title {
  font-weight: bold;
  text-decoration: underline;
  text-underline-position: below;
}


article {
  padding-top: 16px;
  padding: 24px 28px;
}

p.invite-text {
  color: var(--cta-blue);
  font-weight: bold;
  margin-bottom: 5px;
}

ul {
    padding-left: 24px;
    font-weight: 300;
    font-size: var(--text-sm);
}

li {
    margin-bottom: 5px;
}

.btn-container {
    display: flex;
    justify-content: space-between;
}
.overlay-container {
  z-index: 40;
  background-color: var(--modal-background);
  display: absolute;
  top: 0;
  left: 0;
  /* height: 100vh; */
  width: 100vw;
}
.modal-container {
  position: relative;
  width: 40%;
  /* z-index: 50; */
  margin: auto auto;
  background-color: white;
  border-radius: var(--border-modal);
  border: solid 1px red;
}
</style>