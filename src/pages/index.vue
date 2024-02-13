<template>
  <div id="container">
    <h1>
      Virgin Vue
    </h1>

    <p class="message">{{ message }}</p>
    <button @click="changeMessage">Cambiar Mensaje</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: "Este es un mensaje dentro del componente."
    };
  },
  methods: {
    changeMessage() {
      this.message = "Nuevo mensaje cambiado por el botón.";
    }
  }
}
</script>

<style scoped>
/* Aquí van tus estilos CSS */
</style>

<style scoped>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

  * {
    font-family: Roboto;
    box-sizing: border-box;
  }

  #container {
    background-color: #f5f5f5; /* Cambié el color de fondo */
    height: 100vh;
    width: 100vw;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background-color: #65849f;
  }

  h1#logo {
    font-family: 'Montserrat', sans-serif;
    font-size: 64px;
    font-weight: 700;
    color: #333333;
    text-shadow: 2px 2px 4px rgba(255, 255, 255, 0.9);
    margin-bottom: 20px;
    letter-spacing: -6px;
  }

  #joystick {
    width: 100px;
    height: 400px;
    border: 2px solid #dddddd;
    background-color: #ffffff33;
    border-radius: 15px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    display: flex;
    justify-content: center;
    align-items: center;
    display: flex;
    flex-direction: column;
  }

  .points {
    font-size: 24px;
    border: none;
    background-color: #e0e0e0; /* Suavicé el color de fondo */
    color: #333333;
    border-radius: 10px;
    text-align: center;
    display: grid;
    align-items: center;
    padding: 10px;
  }

  #controlers {
    display: flex;
    flex-direction: column;
    gap: 10px;
    justify-content: center;
    align-items: center;
  }

  .racket {
    width: 80px;
    height: 80px;
    font-size: 24px;
    border: none;
    background-color: #4c96af; /* Cambié el color del botón */
    color: #ffffff;
    border-radius: 50%;
    cursor: pointer;
    transition: background-color 0.3s ease;
    display: flex;
    justify-content: center;
    align-items: center;
    box-shadow: -2px 3px 4px 0px rgba(0, 0, 0, 3); 
  }

  .racket:hover {
    background-color: #72b5cc; /* Cambié el color al pasar el ratón */
  }

  #buttoner {
    margin-top: 20px;
  }

  #restart_btn {
    padding: 10px 20px;
    font-size: 18px;
    background-color: #f44336; /* Cambié el color del botón */
    color: #ffffff;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    transition: background-color 0.3s ease;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 3); /* Añadí una sombra suave */
  }

  #restart_btn:hover {
    background-color: #f1655b; /* Cambié el color al pasar el ratón */
  }

  #wrapper{
    display: flex;
    flex-direction: row-reverse;
    padding: 20px 0px;
    gap: 30px;
  }

  #court {
    border: 2px solid #cccccc; /* Cambié el color del borde */
    width: 150px;
    height: 400px;
    border-radius: 15px;
    display: grid;
    justify-items: center;
    align-items: center;
    transition: background-color 1s ease;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Añadí una sombra suave */
    background-color: #ffffff33;
  }

  #energy{
    font-size: 28px;
    font-weight: 800;
    color: #5e5e5e;
  }

  #barr {
    width: 30px;
    height: 250px;
    background-color: #849db2;
    display: flex;
    align-items: center;
    border-radius: 15px;
    overflow: hidden;
    border: 1px solid white;
  }

  #barr #ball {
    height: 30px;
    width: 100%;
    background-color: #5e5e5e;
  }

  .ball_home {
    display: flex;
    flex-direction: column;
  }

  .ball_away {
    display: flex;
    flex-direction: column-reverse;
  }

  #dice {
    font-size: 48px;
    font-weight: bold;
    color: #ffffff;
    background-color: #9e9e9e; /* Cambié el color de fondo */
    width: 80px;
    height: 80px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1); /* Suavicé la sombra */
    margin: 10px 10px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Añadí una sombra suave */
  }

  .dice-roll {
    transform: scale(1.5);
  }

  #pointer {
    display: flex;
    flex-direction: column;
    background-color: #5e5e5e;
    width: 300px;
    height: 100px;
    text-align: left;
    justify-content: center;
    color: #e0e0e0;
    border: 2px solid #cccccc;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    border-radius: 15px;
  }

  .player_score {
    display: flex;
    align-items: center;
    font-size: 24px;
    height: 50px;
  }

  .player_score ul{
    display: flex;
    flex-direction: row;
    margin: 0px;
    gap: 10px;
    margin: 0 auto;
  }

  .player_name{
    text-indent: 10px;
  }

  .player_score li {
    list-style: none;
  }


  @media only screen and (max-width: 600px) {
    /* Aquí van tus estilos específicos para dispositivos móviles */
    #container {
      justify-content: start;
    }

  }



</style>