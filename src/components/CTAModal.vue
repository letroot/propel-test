<template>
  <div>
    <div class="overlay-container">
      <div class="modal-container">
        <img class="close-modal" src="../assets/img/close-modal.svg" />
        <header>
          <h1>
            Would you like to <br />
            join <span class="org-title">GirlsCanCode</span><span>?</span>
          </h1>
          <img class="modal-motif" src="../assets/img/modal-motif.svg" />
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
              background and professional experience, and take that first step
              to apply!
            </li>
          </ul>
        </article>
        <div class="btn-container">
          <a href="#" class="join-different">Join a different community</a>
          <button class="join-button">
            <img class="join-image" src="../assets/img/join.svg" />
            Join GirlsCanCode
          </button>
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
  position: relative;
  border-top-left-radius: var(--border-modal);
  border-top-right-radius: var(--border-modal);
  overflow: hidden;
}

h1 {
  padding: 51px 32px 20px 32px;
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
  padding-left: 
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

.close-modal {
  position: absolute;
  top: 0;
  right: 0;
  margin-right: -25px;
  margin-top: -25px;
}

.modal-motif {
  position: absolute;
  top: 0;
  right: 0;
}

.btn-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-top: 12px;
  padding: 0 28px 24px 28px;
}

.overlay-container {
  background-color: rgba(0, 0, 0, 0.6);
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 100;
  width: 100vw;
}
.modal-container {
  position: absolute;
  width: 40%;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  margin-right: -50%;
  right: auto;
  bottom: auto;
  background-color: white;
  border-radius: var(--border-modal);
  z-index: 110;
}

.join-different {
  color: #384747;
  border-bottom: 1px solid #384747;
  text-decoration: none;
  font-size: var(--text-sm);
}

.join-button {
  background-color: var(--blue-400);
  border-radius: 12px;
  box-shadow: 0px -1px 4px rgba(0, 207, 255, 0.15),
    0px 8px 8px rgba(0, 207, 255, 0.15);
  color: white;
  font-weight: 700;
  font-size: var(--text-sm);
  display: flex;
  align-items: center;
  outline: none;
  border: none;
  padding: 12px 18.5px;
}

.join-image {
  margin-right: 8px;
}
</style>
