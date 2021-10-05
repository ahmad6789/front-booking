<template>
  <div id="mySidenav" class="sidenav">
    <a href="javascript:void(0)" class="closebtn" @click="closeNav"
      ><svg
        xmlns="http://www.w3.org/2000/svg"
        width="20"
        height="20"
        fill="currentColor"
        class="bi bi-x-circle"
        viewBox="0 0 16 16"
      >
        <path
          d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"
        />
        <path
          d="M4.646 4.646a.5.5 0 0 1 .708 0L8 7.293l2.646-2.647a.5.5 0 0 1 .708.708L8.707 8l2.647 2.646a.5.5 0 0 1-.708.708L8 8.707l-2.646 2.647a.5.5 0 0 1-.708-.708L7.293 8 4.646 5.354a.5.5 0 0 1 0-.708z"
        /></svg
    ></a>
    <a style="display: flex">
      <img src="img/logo.png" style="width: 60px; height: 50px" />
      <h2 class="font-weight-bold">حجوزاتي</h2></a
    >
    <div class="links">
      <router-link to="/Home"
        ><svg
          xmlns="http://www.w3.org/2000/svg"
          width="22"
          height="22"
          fill="currentColor"
          class="bi bi-house-door"
          viewBox="0 0 16 16"
        >
          <path
            d="M8.354 1.146a.5.5 0 0 0-.708 0l-6 6A.5.5 0 0 0 1.5 7.5v7a.5.5 0 0 0 .5.5h4.5a.5.5 0 0 0 .5-.5v-4h2v4a.5.5 0 0 0 .5.5H14a.5.5 0 0 0 .5-.5v-7a.5.5 0 0 0-.146-.354L13 5.793V2.5a.5.5 0 0 0-.5-.5h-1a.5.5 0 0 0-.5.5v1.293L8.354 1.146zM2.5 14V7.707l5.5-5.5 5.5 5.5V14H10v-4a.5.5 0 0 0-.5-.5h-3a.5.5 0 0 0-.5.5v4H2.5z"
          />
        </svg>
        الصفحة الرئيسية</router-link
      >
      <a href="#"
        ><svg
          xmlns="http://www.w3.org/2000/svg"
          width="22"
          height="22"
          fill="currentColor"
          class="bi bi-download"
          viewBox="0 0 16 16"
        >
          <path
            d="M.5 9.9a.5.5 0 0 1 .5.5v2.5a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1v-2.5a.5.5 0 0 1 1 0v2.5a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2v-2.5a.5.5 0 0 1 .5-.5z"
          />
          <path
            d="M7.646 11.854a.5.5 0 0 0 .708 0l3-3a.5.5 0 0 0-.708-.708L8.5 10.293V1.5a.5.5 0 0 0-1 0v8.793L5.354 8.146a.5.5 0 1 0-.708.708l3 3z"
          />
        </svg>
        تحميل التطبيق</a
      >
      <a href="#"
        ><svg
          xmlns="http://www.w3.org/2000/svg"
          width="22"
          height="22"
          fill="currentColor"
          class="bi bi-person-check"
          viewBox="0 0 16 16"
        >
          <path
            d="M6 8a3 3 0 1 0 0-6 3 3 0 0 0 0 6zm2-3a2 2 0 1 1-4 0 2 2 0 0 1 4 0zm4 8c0 1-1 1-1 1H1s-1 0-1-1 1-4 6-4 6 3 6 4zm-1-.004c-.001-.246-.154-.986-.832-1.664C9.516 10.68 8.289 10 6 10c-2.29 0-3.516.68-4.168 1.332-.678.678-.83 1.418-.832 1.664h10z"
          />
          <path
            fill-rule="evenodd"
            d="M15.854 5.146a.5.5 0 0 1 0 .708l-3 3a.5.5 0 0 1-.708 0l-1.5-1.5a.5.5 0 0 1 .708-.708L12.5 7.793l2.646-2.647a.5.5 0 0 1 .708 0z"
          />
        </svg>
        تسجيل الدخول</a
      >
      <router-link to="/about"
        ><svg
          xmlns="http://www.w3.org/2000/svg"
          width="22"
          height="22"
          fill="currentColor"
          class="bi bi-bookmark-heart"
          viewBox="0 0 16 16"
        >
          <path
            fill-rule="evenodd"
            d="M8 4.41c1.387-1.425 4.854 1.07 0 4.277C3.146 5.48 6.613 2.986 8 4.412z"
          />
          <path
            d="M2 2a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v13.5a.5.5 0 0 1-.777.416L8 13.101l-5.223 2.815A.5.5 0 0 1 2 15.5V2zm2-1a1 1 0 0 0-1 1v12.566l4.723-2.482a.5.5 0 0 1 .554 0L13 14.566V2a1 1 0 0 0-1-1H4z"
          />
        </svg>
        من نحن</router-link
      >
      <a href="#"
        ><svg
          xmlns="http://www.w3.org/2000/svg"
          width="22"
          height="22"
          fill="currentColor"
          class="bi bi-chat-left-dots"
          viewBox="0 0 16 16"
        >
          <path
            d="M14 1a1 1 0 0 1 1 1v8a1 1 0 0 1-1 1H4.414A2 2 0 0 0 3 11.586l-2 2V2a1 1 0 0 1 1-1h12zM2 0a2 2 0 0 0-2 2v12.793a.5.5 0 0 0 .854.353l2.853-2.853A1 1 0 0 1 4.414 12H14a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2z"
          />
          <path
            d="M5 6a1 1 0 1 1-2 0 1 1 0 0 1 2 0zm4 0a1 1 0 1 1-2 0 1 1 0 0 1 2 0zm4 0a1 1 0 1 1-2 0 1 1 0 0 1 2 0z"
          />
        </svg>
        تواصل معنا</a
      >

      <a href="#" class="logout"
        ><svg
          xmlns="http://www.w3.org/2000/svg"
          width="22"
          height="22"
          fill="currentColor"
          class="bi bi-box-arrow-left"
          viewBox="0 0 16 16"
        >
          <path
            fill-rule="evenodd"
            d="M6 12.5a.5.5 0 0 0 .5.5h8a.5.5 0 0 0 .5-.5v-9a.5.5 0 0 0-.5-.5h-8a.5.5 0 0 0-.5.5v2a.5.5 0 0 1-1 0v-2A1.5 1.5 0 0 1 6.5 2h8A1.5 1.5 0 0 1 16 3.5v9a1.5 1.5 0 0 1-1.5 1.5h-8A1.5 1.5 0 0 1 5 12.5v-2a.5.5 0 0 1 1 0v2z"
          />
          <path
            fill-rule="evenodd"
            d="M.146 8.354a.5.5 0 0 1 0-.708l3-3a.5.5 0 1 1 .708.708L1.707 7.5H10.5a.5.5 0 0 1 0 1H1.707l2.147 2.146a.5.5 0 0 1-.708.708l-3-3z"
          />
        </svg>
        تسجيل خروج</a
      >
    </div>
  </div>

  <div class="tes" id="tes">
    <nav class="navbar navbar-expand-md mb-4">
      <div id="main">
        <span style="font-size: 30px; cursor: pointer" @click="openNav"
          ><svg
            xmlns="http://www.w3.org/2000/svg"
            width="22"
            height="22"
            fill="currentColor"
            class="bi bi-list-nested"
            viewBox="0 0 16 16"
          >
            <path
              fill-rule="evenodd"
              d="M4.5 11.5A.5.5 0 0 1 5 11h10a.5.5 0 0 1 0 1H5a.5.5 0 0 1-.5-.5zm-2-4A.5.5 0 0 1 3 7h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm-2-4A.5.5 0 0 1 1 3h10a.5.5 0 0 1 0 1H1a.5.5 0 0 1-.5-.5z"
            /></svg
        ></span>
      </div>

      <div class="navbar navbar-expand" id="navbarCollapse">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <div class="notif">
              <div class="bell-icon" tabindex="0">
                <svg
                  version="1.1"
                  xmlns="http://www.w3.org/2000/svg"
                  xmlns:xlink="http://www.w3.org/1999/xlink"
                  x="0px"
                  y="0px"
                  width="50px"
                  height="30px"
                  viewBox="0 0 50 30"
                  enable-background="new 0 0 50 30"
                  xml:space="preserve"
                >
                  <g class="bell-icon__group">
                    <path
                      class="bell-icon__ball"
                      id="ball"
                      fill-rule="evenodd"
                      stroke-width="1.5"
                      clip-rule="evenodd"
                      fill="none"
                      stroke="#currentColor"
                      stroke-miterlimit="10"
                      d="M28.7,25 c0,1.9-1.7,3.5-3.7,3.5s-3.7-1.6-3.7-3.5s1.7-3.5,3.7-3.5S28.7,23,28.7,25z"
                    />
                    <path
                      class="bell-icon__shell"
                      id="shell"
                      fill-rule="evenodd"
                      clip-rule="evenodd"
                      fill="#FFFFFF"
                      stroke="#currentColor"
                      stroke-width="2"
                      stroke-miterlimit="10"
                      d="M35.9,21.8c-1.2-0.7-4.1-3-3.4-8.7c0.1-1,0.1-2.1,0-3.1h0c-0.3-4.1-3.9-7.2-8.1-6.9c-3.7,0.3-6.6,3.2-6.9,6.9h0 c-0.1,1-0.1,2.1,0,3.1c0.6,5.7-2.2,8-3.4,8.7c-0.4,0.2-0.6,0.6-0.6,1v1.8c0,0.2,0.2,0.4,0.4,0.4h22.2c0.2,0,0.4-0.2,0.4-0.4v-1.8 C36.5,22.4,36.3,22,35.9,21.8L35.9,21.8z"
                    />
                  </g>
                </svg>
                <div class="notification-amount">
                  <span>1</span>
                </div>
              </div>
            </div>
          </li>
        </ul>
        <form class="form-inherit mx-3 mx-sm-0">
          <input
            class="SearchInp form-control"
            type="text"
            placeholder="أبحث هنا ...."
            aria-label="Search"
          />
          <button class="SearchBtn btn" type="submit">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="16"
              height="16"
              fill="currentColor"
              class="bi bi-search"
              viewBox="0 0 16 16"
            >
              <path
                d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z"
              />
            </svg>
          </button>
        </form>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Sidebar",
  methods: {
    openNav() {
      if (window.matchMedia("(max-width: 800px)").matches) {
        document.getElementById("content").style.marginRight = "16px";
        document.getElementById("tes").style.marginRight = "16px";
        document.getElementById("mySidenav").style.width = "250px";
        document.getElementById("main").style.visibility = "hidden";
      } else {
        document.getElementById("content").style.marginRight = "250px";
        document.getElementById("tes").style.marginRight = "250px";
        document.getElementById("mySidenav").style.width = "250px";
        document.getElementById("main").style.visibility = "hidden";
      }
    },

    closeNav() {
      document.getElementById("content").style.marginRight = "16px";
      document.getElementById("tes").style.marginRight = "16px";
      document.getElementById("mySidenav").style.width = "0";
      document.getElementById("main").style.visibility = "visible";
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
.form-control:focus {
  background-color: #fff;
  border-color: none;
  outline: 0;
  box-shadow: none;
}
.btn:focus {
  box-shadow: none;
}
body {
  font-family: "DroidArabicKufiRegular";
  font-weight: normal;
  font-style: normal;
  margin-right: 0px;
}
.sidenav {
  background-color: #fff;
  height: 100%;
  width: 0;
  position: fixed;
  z-index: 1;
  top: 0;
  right: 0;
  overflow-x: hidden;
  transition: 0.5s;
  padding-top: 60px;
}

.sidenav a {
  padding: 8px 32px 8px 8px;
  text-decoration: none;
  font-size: 17px;
  color: #818181;
  display: block;
  transition: 0.8s;
  margin-top: 10px;
  font-family: "DroidArabicKufiRegular";
  font-weight: normal;
  font-style: normal;
}

.links a:hover {
  color: #f1f1f1;
  background-color: #1ec28b;
  margin-left: 20px;
  margin-right: 20px;
  border-radius: 9px;
}
.links {
  justify-content: right;
  text-align: right;
}

.sidenav .closebtn {
  position: absolute;
  top: 0;
  right: 165px;
  font-size: 36px;
}
.sidenav .closebtn:hover {
  color: #1ec28b;
}
#main {
  width: 0px;
  transition: margin-right 0.5s;
  padding: 16px;
}

.tes {
  background-color: #f5faf8;
  margin: 20px 16px -35px 16px;
  border-radius: 16px;
  margin-left: 250px;
}
@media screen and (max-height: 450px) {
  .sidenav {
    padding-top: 15px;
  }
  .sidenav a {
    font-size: 15px;
  }
}
.tes {
  margin-left: 16px;
}
@media screen and (min-width: 992px) {
  .sidenav {
    width: 250px;
  }
  .tes {
    margin-right: 250px;
    margin-left: 250px;
  }
  #main {
    visibility: hidden;
  }
}
@media screen and (min-width: 768px) {
  .collapse li {
    display: flex;
  }
}
////////////////////////////////////
.form-inherit {
  display: flex;
  position: relative;
  font-family: "DroidArabicKufiRegular";
  font-weight: normal;
  font-style: normal;
}

.SearchInp {
  border: none;

  border-top-right-radius: 20px;
  border-bottom-right-radius: 20px;
}
.SearchBtn {
  border: none;
  border-top-left-radius: 20px;
  border-bottom-left-radius: 20px;
  background-color: #fff;
}
h2,
h6 {
  font-family: "DroidArabicKufiRegular";
  font-weight: normal;
  font-style: normal;
  text-align: right;
}
h6 {
  color: #8c8c8c;
}

/////////////////////////////// Bell Notification Icon /////////////////////////////////////////

.bell-icon {
  position: relative;
  width: 50px;
  height: 50px;
  background: #fff;
  border-radius: 50%;
  display: flex;
  svg {
    margin: auto;
    position: relative;
    right: 2%;
    width: 80%;
    height: 80%;
    stroke: rgba(0, 0, 0, 0.75);
  }
  .bell-icon__group {
    transform-origin: 50% 2px;
    transform: rotate(-8deg);
    animation-fill-mode: both;
    animation-iteration-count: 1;
    animation-timing-function: ease-in-out;
  }
  .bell-icon__ball {
    transform-origin: 50% 2px;
    transform: translateX(-6.5%);
    animation-fill-mode: both;
    animation-iteration-count: 1;
    animation-timing-function: ease-in-out;
  }
  &:focus,
  &:hover {
    outline: none;
    box-shadow: 0 0 12px -8px rgba(0, 0, 0, 0.6);
    .bell-icon__group {
      animation: animateGroup 2.3s;
    }
    .bell-icon__ball {
      animation: animateBall 2.3s;
    }
    .notification-amount {
      opacity: 1;
      visibility: visible;
      &::before {
        animation-name: bounce;
        animation-delay: 450ms;
      }
    }
  }
}

.notification-amount {
  opacity: 0;
  visibility: hidden;
  position: absolute;
  top: 20%;
  right: 24%;
  width: 15px;
  height: 15px;
  color: white;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: "Copse", serif;
  font-size: 10px;
  span {
    position: relative;
  }
  &::before {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    background-color: #f72918;
    border-radius: 50%;
    z-index: 0;
    transform: scale(0);
    animation-duration: 800ms;
    animation-fill-mode: both;
  }
}

$frameLength: 0.8771;

@keyframes animateGroup {
  0%,
  100% {
    transform: rotate(-8deg);
  }
  #{$frameLength * 20%} {
    transform: rotate(0deg);
  }
  #{$frameLength * 40%} {
    transform: rotate(-20deg);
  }
  #{$frameLength * 55%} {
    transform: rotate(20deg);
  }
  #{$frameLength * 65%} {
    transform: rotate(-20deg);
  }
  #{$frameLength * 74%} {
    transform: rotate(8deg);
  }
  #{$frameLength * 85%} {
    transform: rotate(-15deg);
  }
  #{$frameLength * 90%} {
    transform: rotate(-7deg);
  }
}

@keyframes animateBall {
  0%,
  100% {
    transform: translateX(-6.5%);
  }
  #{$frameLength * 20%} {
    transform: translateX(0%);
  }
  #{$frameLength * 25%} {
    transform: translateX(-1%);
  }
  #{$frameLength * 40%} {
    transform: translateX(11%);
  }
  #{$frameLength * 55%} {
    transform: translateX(-11%);
  }
  #{$frameLength * 60%} {
    transform: translateX(0%);
  }
  #{$frameLength * 68%} {
    transform: translateX(10%);
  }
  #{$frameLength * 78%} {
    transform: translateX(-11%);
  }
  #{$frameLength * 90%} {
    transform: translateX(11%);
  }
  #{$frameLength * 98%} {
    transform: translateX(-11%);
  }
}

@keyframes bounce {
  0% {
    transform: scale(0);
  }

  14% {
    transform: scale(1.15);
  }

  28% {
    transform: scale(1);
  }

  42% {
    transform: scale(1.15);
  }

  70% {
    transform: scale(1);
  }
  100% {
    transform: scale(1);
  }
}

.logout {
  position: absolute;
  bottom: 20px;
  padding-left: 57px !important;
}
.Right {
  right: auto;
  left: 0px;
}

///////////////////////////////// Calender Css Style ////////////////////////////////////////
</style>
