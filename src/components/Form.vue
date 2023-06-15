<template>
  <div class="container mx-auto px-20 py-10">
    <div class="w-full h-auto my-4 mx-auto">
      <div
        class="bg-white w-full rounded-md py-5 flex flex-col gap-3 lg:flex-row px-4 justify-between items-center"
      >
        <div class="flex flex-row items-center gap-2">
          <button
            @click="backToOldPage"
            class="form-button text-black text-xl font-[500]"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              fill="none"
              viewBox="0 0 24 24"
              stroke-width="1.5"
              stroke="currentColor"
              class="w-6 h-6"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M18.75 19.5l-7.5-7.5 7.5-7.5m-6 15L5.25 12l7.5-7.5"
              />
            </svg>
          </button>
          <span
            class="font-[ui-sans-serif - 700] text-[22px] font-[700] text-black"
            >Form</span
          >
        </div>
        <div class="text-center bg-[#BD3401] py-1 w-20 rounded-md text-black">
          <button
            type="submit"
            @click="saveData"
            class="text-xl font-[500] text-white"
          >
            Save
          </button>
        </div>
      </div>
    </div>
    <div class="flex flex-col items-center justify-center w-full">
      <div class="bg-white w-full mt-2 rounded p-4">
        <h1 class="text-3xl font-bold text-center py-4">CREATE NEW ACCOUNT</h1>
        <form
          action=""
          @submit="login"
          class="border p-4 rounded flex flex-col lg:gap-10 gap-2 shadow w-full"
        >
          <div
            class="flex flex-col lg:flex-row items-center justify-between w-full gap-4"
          >
            <div class="relative w-full">
              <input
                type="text"
                v-model="fullName"
                placeholder="Full Name"
                class="w-full py-4 outline-none border rounded pl-4 text-xl"
              />
              
              <span class="absolute right-3 top-3 text-lg text-red-900">{{
                errorName
              }}</span>
            </div>
            <div class="relative w-full">
              <input
                type="text"
                v-model="componyName"
                placeholder="Compony Name"
                class="w-full py-4 outline-none border rounded pl-4 text-xl"
              />
              <span>{{ v$.componyName?.errors }}</span>
              <span class="absolute right-3 top-3 text-lg text-red-900">{{
                componyNameError
              }}</span>
            </div>
          </div>

          <div
            class="flex flex-col lg:flex-row items-center justify-between w-full gap-4"
          >
            <div class="relative w-full">
              <input
                type="text"
                v-model="city"
                placeholder="City"
                class="w-full py-4 outline-none border rounded pl-4 text-xl"
              />
              <span class="absolute right-3 top-3 text-lg text-red-900">{{
                locationNameError
              }}</span>
            </div>
            <div class="relative w-full">
              <input
                type="text"
                v-model="year"
                placeholder="Year Created"
                class="w-full py-4 outline-none border rounded pl-4 text-xl"
              />
              <span class="absolute right-3 top-3 text-lg text-red-900">{{
                yearError
              }}</span>
            </div>
          </div>
          <div
            class="flex flex-col lg:flex-row items-center justify-between w-full gap-4"
          >
            <div class="relative w-full">
              <input
                type="text"
                v-model="email"
                placeholder="Email"
                class="w-full py-4 outline-none border rounded pl-4 text-xl"
              />
              <span>{{ v$.email?.errors }}</span>
              <span class="absolute right-3 top-3 text-lg text-red-900">{{
                emailError
              }}</span>
            </div>
            <div class="relative w-full">
              <input
                type="password"
                v-model="password"
                placeholder="Password"
                class="w-full py-4 outline-none border rounded pl-4 text-xl"
              />
              <span class="absolute right-3 top-3 text-lg text-red-900">{{
                passwordError
              }}</span>
            </div>
          </div>
        </form>
        <div class="">
          <button
            @click="backToOldPage"
            type="button"
            class="w-full py-3 outline-none border-2 bg-[#F7F7F7] rounded text-[#232323] font-bold mt-4"
          >
            Already have an account?
            <a href="#" class="text-blue-400">Get account</a>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { useVuelidate } from "@vuelidate/core";
import { required, email } from "@vuelidate/validators";
export default {
  name: "Form",
  setup() {
    return { v$: useVuelidate() };
  },
  data() {
    return {
      fullName: "",
      componyName: "",
      city: "",
      year: "",
      email: "",
      password: "",
      errorName: "",
      componyNameError: "",
      locationNameError: "",
      yearError: "",
      emailError: "",
      passwordError: "",
    };
  },
 

  watch: {
    fullName() {
      this.checkName();
    },
    componyName() {
      this.checkComponyName();
    },
    city() {
      this.checkLocation();
    },
    year() {
      this.checkYear();
    },
    email() {
      this.checkEmail();
    },
    password(val) {
      this.checkPassword(val);
    },
  },

  methods: {
    async saveData(e) {
      const isFormCorrect = await this.v$.$validate();
      if(isFormCorrect){
          alert("Successfully your form submitted!!");
        }else{
            console.log(this.v$.fullName?.errors);
            alert("Valid validation")
      }
    },

    backToOldPage() {
      this.$emit("getPage", "table");
    },
    checkName() {
      if (this.fullName === "") {
        this.errorName = "Name is required";
      } else if (!/^[A-Za-z]*\s{1}[A-Za-z]*$/.test(this.fullName)) {
        this.errorName = "Write full name";
      } else {
        this.errorName = null;
      }
    },
    checkComponyName() {
      if (this.componyName === "") {
        this.componyNameError = "Compony Name is required";
      }
    },
    checkLocation() {
      if (this.city === "") {
        this.locationNameError = "Location is required";
      }
    },
    checkYear() {
      if (this.year.length === 0) {
        this.yearError = "Created Year is required";
        // }else if (phone.length !== 10){
        //     telError.innerHTML = "Phone number should be 10 digits";
        // }else if (!phone.match(/^[0-9]{10}$/)){
        //     telError.innerHTML = "Only digits please";
      } else if (!/^[0-9]{4}$/.test(this.year)) {
        this.yearError = "Invalid Year";
        // }else if (this.year.length > 3){
        //     this.yearError = "Digits must be 4 digits";
      } else {
        this.yearError = null;
      }
    },
    checkEmail() {
      if (this.email == "") {
        this.emailError = "Email is required";
      } else if (!/^[^@]+@\w+(\.\w+)+\w$/.test(this.email)) {
        this.emailError = "Invalid email";
      } else {
        this.emailError = null;
      }
      // else if(this.email.test(/^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/)){
      //     this.emailError = "valid Email"
      // }else{
      //     this.emailError = "valid Email"
      // }
    },
    checkPassword() {
      if (this.password == "") {
        this.passwordError = "Email is required";
      } else if (this.password.length < 6) {
        this.passwordError = "password at least six characters";
      } else {
        this.passwordError = null;
      }
    },
  },

  validations() {
    return {
      fullName: { required },
      componyName: { required },
      city: { required },
      year: { required },
      email: { required, email },
      password: { required },
    };
  },
};
</script>

<style></style>
