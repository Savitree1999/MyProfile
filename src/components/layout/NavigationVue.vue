<template>
  <div>
    <a @click="nar_tab = !nar_tab" class="menu-toggle rounded" >
      <i class="fas fa-bars"></i>
    </a>
    <Transition name="slide-fade">
    <nav v-show="nar_tab" id="sidebar-wrapper">
      <ul class="sidebar-nav">
        <li class="sidebar-brand"><a @click="nar_tab = !nar_tab" href="#page-top">My Profile</a></li>
        <li @click="nar_tab = !nar_tab" class="sidebar-nav-item"><a href="#page-top">Home</a></li>
        <li @click="nar_tab = !nar_tab" class="sidebar-nav-item"><a href="#about">Education</a></li>
        <li @click="nar_tab = !nar_tab" class="sidebar-nav-item"><a href="#courses">Courses</a></li>
        <li @click="nar_tab = !nar_tab" class="sidebar-nav-item"><a href="#projects">My Projects</a></li>
        <li @click="nar_tab = !nar_tab" class="sidebar-nav-item"><a href="#additional_courses">Additional Courses & Certificate</a></li>
        <li @click="nar_tab = !nar_tab" class="sidebar-nav-item"><a href="#skill">Skills</a></li>
        <li @click="nar_tab = !nar_tab" class="sidebar-nav-item"><a href="#contact">Contact</a></li>
      </ul>
    </nav>
    </Transition>
  </div>
</template>

<script>
export default {
    data() {
        return {
          nar_tab: false,
          check: false,
        }
    },
  
};
</script>

<style>
.slide-fade-enter-active {
  transition: all 0.5s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.5s cubic-bezier(1, 0, 0, 1);
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(250px);
  opacity: 1;
}

</style>

