<template>
  <header>
    <NuxtLink class="home" to="/">アキラ</NuxtLink>
    <span>リョウカ、だいすき。</span>
    <nav>
      <ul>
        <li>
          <a
            class="ds"
            target="_blank"
            href="https://youtube.com/channel/UCnCPN9xi7y8arkpymcTXzNw"
            aria-label="YouTube"
          >
            <img
              class="external"
              src="~/assets/youtube.svg"
              alt="Icon YouTube"
            />
          </a>
          <a
            class="ds"
            target="_blank"
            href="https://twitch.tv/akiranohikari"
            aria-label="Twitch"
          >
            <img
              class="external"
              src="~/assets/twitch.svg"
              alt="Icon  Twitch"
            />
          </a>
          <a
            class="ds"
            target="_blank"
            href="https://twitter.com/AkiraNoHikariii"
            aria-label="Twitter"
          >
            <img
              class="external"
              src="~/assets/twitter.svg"
              alt="Icon Twitter"
            />
          </a>
          <a
            class="ds"
            target="_blank"
            href="https://github.com/AkiraNoHikari"
            aria-label="GitHub"
          >
            <img class="external" src="~/assets/github.svg" alt="Icon GitHub" />
          </a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
header {
  display: flex;
  font-size: 1.25rem;
  justify-content: space-between;
  padding: 3vmin;
  position: fixed;
  width: 100%;
  top: 0;
}

span {
  user-select: text;
  color: transparent;
}

.external {
  width: 25px;
  height: 100%;
  margin: 0.5rem;
  vertical-align: middle;
  filter: invert();
}

.home {
  padding: 0;
  font-size: 2rem;
  vertical-align: middle;
  font-weight: bold !important;
}

ul {
  display: flex;
  align-items: center;
  justify-content: center;
}

.logo {
  height: 56px;
  border-radius: 100%;
}

nav {
  display: flex;
  flex-direction: row;
}

a:not(.ds) {
  padding: 0.5rem;
  vertical-align: middle;
  font-weight: 200;
}

a:hover:not(.home) {
  text-shadow: 0 1px 0 rgba(255, 255, 255, 0.651);
}

.route {
  text-transform: capitalize;
}
</style>

export default {
  name: "Header",
};