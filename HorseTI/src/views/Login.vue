<template>
  <div class="outer">
    <main>
      <div class="title">
        <h1>Login</h1>
      </div>

      <div class="social-midia">
        <a href="#">
          <img src="@/assets/img/facebook.png" alt="" />
        </a>
        <a href="#">
          <img src="@/assets/img/google.png" alt="" />
        </a>
        <a href="#">
          <img src="@/assets/img/twitter.png" alt="" />
        </a>
      </div>
      <div class="alternative">
        <span> ou </span>
      </div>
      <div class="name-top">
        <span>Email:</span>
      </div>
      <div class="input-field">
        <input type="text" placeholder="Digite seu E-mail" />
      </div>
      <div class="name-top">
        <span>Senha:</span>
      </div>
      <div class="input-field">
        <input type="Password" placeholder="Digite sua Senha" />
      </div>
      <div class="input-button">
        <input type="button" value="Entrar" />
      </div>
    </main>
    <section class="images">
        <img src="@/assets/img/img-2.svg" alt="image" />
        <div class="circle"></div>
    </section>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

/* * {
    margin: 0;
  padding: 0;
  border: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
} */

.outer {
  background: linear-gradient(#161e35, #3071e7);
  background-repeat: no-repeat;
  min-height: 100vh;
  display: flex;
}

main {
  width: 50vw;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.title h1 {
  margin-bottom: 1rem;
  background: -webkit-linear-gradient(45deg, #8a93e4, #00b7ff, #3071e7);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

.name-top span {
  margin-right: 12rem;
  margin-top: 1rem;
  color: #fff;
}

.alternative span {
  position: relative;
  color: #fff;
}

.alternative span::before,
.alternative span::after {
  position: absolute;
  content: "";
  height: 1px;
  width: 100px;
  bottom: 50%;
  right: 30px;
  background-color: #fff;
}

.alternative span::after {
  left: 30px;
  background-color: #fff;
}

.social-midia {
  margin-top: 1rem;
  margin-left: 35px;
  margin-bottom: 1rem;
}

.social-midia img {
  height: 36px;
  margin-right: 35px;
}

.input-field input {
  width: 250px;
  height: 40px;
  margin-top: 1rem;
  background-color: #161e35;
  border-radius: 6px;
  color: #fff;
  outline: none;
  padding: 3% 5%;
}

.input-field input:first-child {
  margin-bottom: 1rem;
}

.input-button input {
  background: linear-gradient(to right, #0419d6, #00b7ff);
  color: #fff;
  width: 250px;
  height: 40px;
  border-radius: 40px;
  margin-top: 30px;
  cursor: pointer;
}

.input-button input:hover {
  background: linear-gradient(to right, rgb(230, 108, 169), #970584);
  color: #fff;
  width: 250px;
  height: 40px;
  border-radius: 40px;
}

section.images {
   width: 100%;
  margin-left: 0px; 
  display: flex;
  align-items: flex-end;
  justify-content: flex-end; 
}

section.images .circle {
  position: absolute;
  height: 100%;
  width: 100%;
  top: 0;
  left: 0;
  background: linear-gradient(45deg, #8a93e4, #00b7ff, #3071e7);
  clip-path: circle(70% at right 80%);
  
}
</style>
