<template>
  <section class="head_section">
    <div class="header">
      <nav class="navbar">
        <div>
          <div class="nav-items">
            <span class="logo">
              <svg xmlns="http://www.w3.org/2000/svg" width="23" height="30" fill="none" viewBox="0 0 33 49"
                aria-label="Homepage" class="css-v5hztt">
                <path fill="#00B6FF"
                  d="M16.5 23.612a7.28 7.28 0 0 1 7.28-7.279h1.053a8.167 8.167 0 1 1 0 16.333H23.78a7.28 7.28 0 0 1-7.279-7.279z">
                </path>
                <path fill="#24CB71"
                  d="M0 40.834a8.167 8.167 0 0 1 8.167-8.167H16.5v8.083c0 4.557-3.735 8.25-8.292 8.25C3.698 49 0 45.344 0 40.834">
                </path>
                <path fill="#FF7237" d="M16.5 0v16.333h8.333a8.167 8.167 0 1 0 0-16.333z"></path>
                <path fill="#FF3737" d="M0 8.166a8.167 8.167 0 0 0 8.167 8.167H16.5V0H8.167A8.167 8.167 0 0 0 0 8.166">
                </path>
                <path fill="#874FFF"
                  d="M0 24.5a8.167 8.167 0 0 0 8.167 8.167H16.5V16.334H8.167A8.167 8.167 0 0 0 0 24.5"></path>
              </svg>
            </span>
            <div class="nav-item" @mouseover="showDropdown = true" @mouseleave="showDropdown = false">
              Products <div v-if="showDropdown" class="dropdown-menu">
                <div>
                  <div class="dropdown-raw">
                    <div class="dropdown-column">
                      <div>Figma Design</div>
                      <h6 class="doubled-text">Design and prototype in one place</h6>
                      <span class="menu_feat">
                        <img src="@/public/FigmaDesign.avif" alt="Logo" />
                      </span>
                    </div>
                    <div class="dropdown-column">
                      <div>Fig Jam</div>
                      <h6 class="doubled-text">Collaborate with a digital whiteboard</h6>
                      <span class="menu_feat">
                        <img src="@/public/Jam.avif" alt="Logo" />
                      </span>
                    </div>
                    <div class="dropdown-column">
                      <div>Dev Mode</div>
                      <h6 class="doubled-text">Translate designs into code</h6>
                      <span class="menu_feat">
                        <img src="@/public/Dev.avif" alt="Logo" />
                      </span>
                    </div>
                    <div class="dropdown-column">
                      <div>Figma Slides</div>
                      <h6 class="doubled-text">Co-create presentations</h6>
                      <span class="menu_feat">
                        <img src="@/public/Slides.avif" alt="Logo" />
                      </span>
                    </div>
                  </div>
                  <div class="break"></div> <!-- break -->
                  <div class="dropdown-raw">
                    <div class="dropdown-column">
                      <div>AI</div>
                      <h6 class="doubled-text">Explore all Figma AI features</h6>
                    </div>
                    <div class="dropdown-column">
                      <div>Downloads</div>
                      <h6 class="doubled-text">Get the desktop, mobile and font installer aps</h6>
                    </div>
                    <div class="dropdown-column">
                      <div>What's new</div>
                      <h6 class="doubled-text">See the latest features and releases</h6>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="nav-item" @mouseover="showDropdown = true" @mouseleave="showDropdown = false">
              Products <div v-if="showDropdown" class="dropdown-menu">
              </div>
            </div>
            <div class="nav-item" @mouseover="showDropdown = true" @mouseleave="showDropdown = false">
              Solutions <div v-if="showDropdown" class="dropdown-menu">
              </div>
            </div>
            <div class="nav-item" @mouseover="showDropdown = true" @mouseleave="showDropdown = false">
              Community <div v-if="showDropdown" class="dropdown-menu">
              </div>
            </div>
          </div>
        </div>
        <div class="nav-right">
          <button class="contact-sales">Contact sales</button>
          <button class="login">Log in</button>
          <button @mouseover="hover = true" @mouseleave="hover = false" @click="showModal = true"
            :class="{ 'hovered': hover }" class="cta-button">
            <span v-if="hover"> → </span>Get started for free
          </button>
        </div>
      </nav>
    </div>
  </section>
  <hr class="divider" />
</template>

<script lang="ts">
export default {
  data() {
    return {
      hover: false,
      showDropdown: false,
      showModal: false,
    };
  },
};
</script>

<style scoped>
.doubled-text {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 16px;
  font-weight: 100;
  color: gray;
}

.nav-right .contact-sales {
  background: transparent;
  /* Прозрачный фон */
  border: none;
  /* Без рамки */
  cursor: pointer;
  /* Указатель при наведении */
  font-size: 16px;
  font-weight: 200;
  height: 50px;
}

.nav-right .login {
  background: transparent;
  /* Прозрачный фон */
  border: 1px solid black;
  /* Тонкая чёрная рамка */
  border-radius: 5px;
  /* Закруглённые края */
  cursor: pointer;
  /* Указатель при наведении */
  font-size: 16px;
  font-weight: 200;
  height: 50px;
  padding: 10px;
}

.cta-button {
  border-radius: 0;
  /* Прямые края при наведении */
  background: black;
  /* Чёрный фон */
  color: white;
  /* Белый текст */
  border-radius: 5px;
  /* Закруглённые края */
  cursor: pointer;
  /* Указатель при наведении */
  font-size: 16px;
  font-weight: 200;
  height: 50px;
  padding: 10px;
}

.cta-button.hovered {
  border-radius: 0;
  /* Прямые края при наведении */
  background: black;
  /* Чёрный фон */
  color: white;
  /* Белый текст */
  border-radius: 5px;
  /* Закруглённые края */
  cursor: pointer;
  /* Указатель при наведении */
  font-size: 16px;
  font-weight: 200;
  height: 50px;
  padding: 10px;


}

.get-started-animated {
  position: relative;
  transition: transform 0.3s;
}

.get-started-animated:hover {
  transform: scale(1.05);
}

.divider {
  color: #ffff;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: start;
  background-color: blue;
  width: 100%;
}

.logo {
  height: 30px;
  width: 23px;
  margin: 10px;
}

.menu_feat img {
  height: 140px;
  width: 245px;
}

.break {
  flex-basis: 100%;
  height: 0;
}

.navbar {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: start;
  background-color: white;
  padding: 10px 20px;
  width: 100%;
}

.nav-items {
  display: flex;
  align-items: center;
}

.nav-item {
  position: relative;
  margin-right: 20px;
}

.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  display: flex;
  background-color: white;
  border: 1px solid #ccc;
}

.dropdown-column {
  padding: 10px;
}

.dropdown-raw {
  display: flex;
  justify-content: space-between;
  align-items: start;
  padding: 10px;
}

.nav-right {
  display: flex;
  align-items: center;
  gap: 10px;
}

button {
  margin-left: 10px;
}
</style>
