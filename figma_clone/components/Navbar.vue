<template>
  <section class="head_section">
    <div class="header">
      <nav class="navbar">
        <div>
          <div class="nav-items">
            <span class="logo">
              <img src="@/public/icon-192.png" alt="Logo" />
            </span>
            <div class="nav-item" @mouseover="showDropdown = true" @mouseleave="showDropdown = false">
              Products <div v-if="showDropdown" class="dropdown-menu">
                <div>
                  <div class="dropdown-raw">
                    <div class="dropdown-column">
                      <div>Figma Design</div>
                      <h6>Design and prototype in one place</h6>
                      <span class="menu_feat">
                        <img src="@/public/FigmaDesign.avif" alt="Logo" />
                      </span>
                    </div>
                    <div class="dropdown-column">
                      <div>Fig Jam</div>
                      <h6>Collaborate with a digital whiteboard</h6>
                      <span class="menu_feat">
                        <img src="@/public/Jam.avif" alt="Logo" />
                      </span>
                    </div>
                    <div class="dropdown-column">
                      <div>Dev Mode</div>
                      <h6>Translate designs into code</h6>
                      <span class="menu_feat">
                        <img src="@/public/Dev.avif" alt="Logo" />
                      </span>
                    </div>
                    <div class="dropdown-column">
                      <div>Figma Slides</div>
                      <h6>Co-create presentations</h6>
                      <span class="menu_feat">
                        <img src="@/public/Slides.avif" alt="Logo" />
                      </span>
                    </div>
                  </div>
                  <div class="break"></div> <!-- break -->
                  <div class="dropdown-raw">
                    <div class="dropdown-column">
                      <div>AI</div>
                      <h6>Explore all Figma AI features</h6>
                    </div>
                    <div class="dropdown-column">
                      <div>Downloads</div>
                      <h6>Get the desktop, mobile and font installer aps</h6>
                    </div>
                    <div class="dropdown-column">
                      <div>What's new</div>
                      <h6>See the latest features and releases</h6>
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
          <button class="get-started">Get started for free</button>
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
      showDropdown: false,
    };
  },
};
</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: start;
  background-color: blue;
  width: 100%;
}

.logo img {
  height: 40px;
  width: 40px;
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
}

button {
  margin-left: 10px;
}
</style>
