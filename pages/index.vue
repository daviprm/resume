<template>

  <main>

    <header>
      <div class="header_container">
        <h2><span>Res</span>ume</h2>
        <div class="header_links">
          <a href="#">Inicio</a>
          <a href="#">Resumos</a>
          <a href="#">Contato</a>
        </div>
        <a href="#" class="btn_git">Github</a>
      </div>
      <div class="header_blur"></div>
    </header>

    <!-- cover -->

    <div class="cover">
      <div class="cover_container">

        <div class="cover_text">
          <span>Resume</span>
          <h2>Seu Resumo em <br> Poucos Cliques</h2>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia sunt natus expedita dolorum nostrum totam eveniet aperiam porro optio. Perspiciatis vitae voluptatum quam ullam aut quae ab iste esse molestiae?</p>
          <a href="#">Visualizar Resumos</a>
        </div>

        <img src="/cover.svg" alt="">

      </div>
      <div class="cover_blur"></div>
      <div class="cover_square"></div>
      <div class="cover_square_bottom"></div>
    </div>

  </main>

</template>

<script>

  export default {
    name: 'IndexPage'
  }

</script>

<style scoped>

  main {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  header {
    width: 100%;
    height: 80px;
    display: flex;
    justify-content: center;
    align-items: center;
    animation: from_top .5s ease-in-out;
  }

  .header_blur {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    background: #ff4848;
    position: absolute;
    top: -100px;
    left: -100px;
    filter: blur(140px);
  }
  
  .header_container {
    width: 1200px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .header_container h2 {
    font-size: 18px;
    color: var(--red);
    font-weight: 600;
  }

  .header_container h2 span {
    color: white;
  }

  .header_container .header_links {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .header_container .header_links a {
    font-size: 13px;
    text-decoration: none;
    color: #c5c5c5;
    padding: 10px 15px;
    border-radius: 3px;
    font-weight: 500;
    cursor: pointer;
    transition: .3s;
  }

  .header_container .header_links a:hover {
    background: #20212b;
  }

  .header_container .btn_git {
    padding: 10px 30px;
    border-radius: 4px;
    background: #ff4848;
    color: white;
    font-size: 13px;
    text-decoration: none;
    font-weight: 500;
    transition: .3s;
  }

  .header_container .btn_git:hover {
      filter: brightness(0.8);
  }

  /* cover */

  .cover {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .cover .cover_blur {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    background: #ff4848;
    position: absolute;
    bottom: 200px;
    right: -100px;
    filter: blur(140px);
    z-index: 99;
  }

  .cover .cover_square {
    width: 500px;
    height: 500px;
    border-radius: 30px;
    border: 2px solid #ff4848;
    position: absolute;
    bottom: 100px;
    right: -400px;
    transform: rotate(40deg);
  }

  .cover .cover_square_bottom {
    width: 500px;
    height: 500px;
    border-radius: 30px;
    border: 2px solid #ff4848;
    position: absolute;
    bottom: 200px;
    right: -400px;
    transform: rotate(40deg);
  }

  .cover .cover_container {
    width: 1200px;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .cover .cover_container .cover_text {
    width: 600px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    animation: from_left 1s ease-in-out;
  }

  .cover .cover_container .cover_text span {
    padding: 8px 12px;
    background: #13141b;
    border-radius: 20px;
    font-size: 11px;
    font-weight: 600;
    color: #a0a0a0;
  }

  .cover .cover_container .cover_text h2 {
    margin-top: 10px;
    font-size: 60px;
    line-height: 60px;
    font-weight: 800;
    color: white;
  }

  .cover .cover_container .cover_text p {
    margin-top: 20px;
    font-size: 13px;
    font-weight: 500;
    color: #808080;
  }

  .cover .cover_container .cover_text a {
    margin-top: 20px;
    padding: 13px 30px;
    border-radius: 4px;
    background: #24252e;
    color: #c5c5c5;
    font-size: 13px;
    text-decoration: none;
    font-weight: 500;
    transition: .3s;
  }

  .cover .cover_container .cover_text a:hover {
    filter: brightness(0.8);
  }

  .cover .cover_container img {
    width: 600px;
    animation: from_right 1.3s ease-in-out;
  }






  @keyframes from_left {
    0% {
      transform: translateX(-100px);
      opacity: 0;
    }
    100% {
      transform: translateX(0);
      opacity: 1;
    }
  }

  @keyframes from_right {
    0% {
      transform: translateX(100px);
      opacity: 0;
    }
    100% {
      transform: translateX(0);
      opacity: 1;
    }
  }

  @keyframes from_top {
    0% {
      transform: translateY(-80px);
      opacity: 0;
    }
    100% {
      transform: translateX(0);
      opacity: 1;
    }
  }








</style>