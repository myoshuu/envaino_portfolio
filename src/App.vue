<template>
  <div class="flex justify-center align-center mx-5 my-5">
    <!-- <p class="uppercase text-xs p-2 text-slate-400">Pdt. Edy Pangangkat</p> -->
    <section class="border rounded-md p-10 w-3/4">
      <!-- Header -->
      <header>
        <div class="title text-lg text-slate-500 text-center lowercase">
          It's Me
        </div>
        <p class="sub-title text-2xl text-center text-blue-900 font-medium">
          Edy Pangangkat
        </p>
        <div class="image mx-auto w-40 mt-8">
          <img class="rounded-xl" src="@/assets/me.jpg" alt="" />
        </div>
      </header>

      <!-- Profesi -->
      <div class="profesi mt-4 flex justify-center content-center">
        <div class="w-fit">
          <div class="grid grid-flow-col grid-rows-max grid-cols-max gap-2">
            <SkillCard title="Gembala Jemaat GKMI Sion" />
            <SkillCard title="Dosen STAK AW" />
          </div>
        </div>
      </div>

      <!-- Medsos -->
      <div class="contact flex flex-col justify-center items-center">
        <div class="title text-lg text-slate-500 my-6 text-center">
          Contact me
        </div>
        <div class="content p-2 grid grid-cols-3 gap-5 w-4/5">
          <!-- Whatsapp -->
          <div
            class="
              border
              rounded-lg
              hover:border-green-400
              transition-colors
              p-2
            "
          >
            <a
              class=""
              href="https://api.whatsapp.com/send?phone=https://api.whatsapp.com/send?phone=https://wa.me/628979704444"
              target="_blank"
            >
              <div class="card-title flex items-center">
                <fa
                  :icon="['fab', 'whatsapp']"
                  class="text-xl text-green-600"
                />
                <p class="ml-3 text-green-600">Whatsapp</p>
              </div>
              <div class="card-content mt-3">
                <p class="text-sm text-slate-500">Edy Pangangkat</p>

                <div class="sub-content flex justify-between items-center">
                  <span>(+62) 897-9704-444</span>
                  <fa :icon="['fas', 'angle-right']" class="mr-3" />
                </div>
              </div>
            </a>
          </div>

          <!-- Facebook -->
          <div
            class="
              border
              rounded-lg
              p-2
              hover:border-blue-400
              transition-colors
            "
          >
            <a href="https://facebook.com/edy.pangangkat" target="_blank">
              <div class="card-title flex items-center">
                <fa :icon="['fab', 'facebook']" class="text-xl text-blue-600" />
                <p class="ml-3 text-blue-600">Facebook</p>
              </div>
              <div class="card-content mt-3">
                <p class="text-sm text-slate-500">Edy Pangangkat</p>

                <div class="sub-content flex justify-between items-center">
                  <span>Berbagi Sukacita</span>
                  <fa :icon="['fas', 'angle-right']" class="mr-3" />
                </div>
              </div>
            </a>
          </div>

          <!-- Email -->
          <div
            class="border rounded-lg p-2 hover:border-red-400 transition-colors"
          >
            <a href="mailto: envaino@gmail.com">
              <div class="card-title flex items-center">
                <fa :icon="['fas', 'envelope']" class="text-lg text-red-600" />
                <p class="ml-3 text-red-600">Gmail</p>
              </div>
              <div class="card-content mt-3">
                <p class="text-sm text-slate-500">Edy Pangangkat</p>

                <div class="sub-content flex justify-between items-center">
                  <span>envaino@gmail.com</span>
                  <fa :icon="['fas', 'angle-right']" class="mr-3" />
                </div>
              </div>
            </a>
          </div>

          <!-- Website -->
          <div
            class="
              border
              rounded-lg
              p-2
              hover:border-slate-400
              transition-colors
            "
          >
            <a href="https://envaino.id">
              <div class="card-title flex items-center">
                <fa :icon="['fas', 'globe']" class="text-lg text-slate-600" />
                <p class="ml-3 text-slate-600">Website</p>
              </div>
              <div class="card-content mt-3">
                <p class="text-sm text-slate-500">Edy Pangangkat</p>

                <div class="sub-content flex justify-between items-center">
                  <span>envaino.id</span>
                  <fa :icon="['fas', 'angle-right']" class="mr-3" />
                </div>
              </div>
            </a>
          </div>

          <!-- Youtube -->
          <div
            class="
              border
              rounded-lg
              p-2
              hover:border-red-400
              transition-colors
              cursor-pointer
            "
            @click="show"
          >
            <div class="card-title flex items-center">
              <fa :icon="['fab', 'youtube']" class="text-lg text-red-600" />
              <p class="ml-3 text-red-600">Youtube</p>
            </div>
            <div class="card-content mt-3">
              <p class="text-sm text-slate-500">Edy Pangangkat</p>

              <div class="sub-content flex justify-between items-center">
                <span>Choose</span>
                <fa :icon="['fas', 'angle-right']" class="mr-3" />
              </div>
            </div>
          </div>

          <!-- Instagram -->
          <div
            class="
              border
              rounded-lg
              p-2
              hover:border-purple-400
              transition-colors
            "
          >
            <a href="https://www.instagram.com/envaino/">
              <div class="card-title flex items-center">
                <fa
                  :icon="['fab', 'instagram']"
                  class="text-lg text-purple-800"
                />
                <p class="ml-3 text-purple-800">Instagram</p>
              </div>
              <div class="card-content mt-3">
                <p class="text-sm text-slate-500">Edy Pangangkat</p>

                <div class="sub-content flex justify-between items-center">
                  <span>envaino</span>
                  <fa :icon="['fas', 'angle-right']" class="mr-3" />
                </div>
              </div>
            </a>
          </div>
        </div>
      </div>

      <!-- Copyright -->
      <div class="copyright text-xs text-slate-400 text-center mt-10">
        <p>Copyright &copy; <span></span> envaino.id</p>
      </div>
    </section>

    <!-- Modal -->
    <div class="modal-parent" id="modal">
      <div
        class="
          modal
          bg-white
          w-1/5
          py-1
          px-3
          border
          rounded-xl
          flex flex-col
          justify-evenly
        "
      >
        <div class="title mb-2 flex items-center justify-between">
          <p>Choose The Channel</p>
          <fa
            class="hover:text-red-700 cursor-pointer"
            :icon="['fas', 'times']"
            @click="show"
          />
        </div>

        <!-- Button -->
        <a href="https://www.youtube.com/c/envaino">
          <div class="border py-5 rounded-xl hover:border-red-300">
            <p class="text-center">envaino</p>
          </div>
        </a>
        <a href="https://www.youtube.com/c/envainoid">
          <div class="border py-5 rounded-xl hover:border-red-300">
            <p class="text-center">envaino.id</p>
          </div>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
// Components
import SkillCard from "@/components/SkillCard.vue";
import Card from "@/components/Card.vue";

export default {
  name: "App",
  components: {
    SkillCard,
    Card,
  },
  methods: {
    show() {
      let modal = document.getElementById("modal");
      // console.log("tes");
      modal.classList.toggle("active");
    },
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Fredoka&family=Poppins:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Fredoka", monospace;
}

p.sub-title {
  font-family: "Poppins";
}

.modal {
  position: absolute;
  z-index: 2;
  top: 73%;
  left: 50%;
  transform: translate(-50%, -50%) scale(0);
  width: 250px;
  height: 215px;
  z-index: 2;
  background: white;
  box-shadow: 2px 3px 10px rgba(0, 0, 0, 0.15);
  transition: 150ms cubic-bezier(0.165, 0.84, 0.44, 1);
}

.overlay {
  position: fixed;
  display: none;
  background: rgba(0, 0, 0, 0.15);
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  z-index: 1;
  width: 100vw;
  height: 100vh;
}

.modal-parent.active .overlay {
  display: block;
}

.modal-parent.active .modal {
  transform: scale(1);
}
</style>
