<template>
  <main>
    <!-- <div class="overlay">
      <div class="modal">
      <textarea name="note" id="note" cols="30" rows="10"></textarea>
      <button>Add Note</button>
      <button class="close">Close</button>
      </div>

    </div> -->
    <div class="container">
      <header>
        <h1>Notes</h1>
        <button>+</button>
      </header>
      <div class="cards-container">
        <div class="card">
          <p class="main-text">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolor
          </p>
          <p class="date">
            27/02/2023
          </p>
        </div>
        <div class="card">
          <p class="main-text">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolor
          </p>
          <p class="date">
            27/02/2023
          </p>
        </div>
      </div>
    </div>
  </main>
</template>

<style scoped>
  main {
    height: 100vh;
    width: 100vw;
  }

.container {
  max-width: 1000px;
  padding: 10px;
  margin: 0 auto;

}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

h1 {
  font-weight: bold;
  margin: 25px;
  font-size: 50px;
}

header button {
  border: none;
  padding: 10px;
  width: 50px;
  height: 50px;
  font-size: 20px;
  cursor: pointer;
  background-color: aquamarine;
  border-radius: 100%;
}

.card {
  width: 225px;
  height: 225px;
  background-color: dodgerblue;
  border-radius: 10px;
  padding: 10px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  margin-right: 20px;
  margin-bottom: 20px;
}
.cards-container {
  display: flex;
  flex-wrap: wrap;
  
}
.date {
  font-size: 12px;
  font-weight: bold;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  z-index: 10;
  display: flex;
  align-items: center;
  justify-content: center;
}

.modal {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background-color:gray;
  border-radius: 10px;
  padding: 20px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.modal button {
  padding: 10px 20px;
  margin-top: 20px;
  background-color: blueviolet;
  border: none;
  border-radius: 10px;
}

.modal .close{
  background-color: red;
}
</style>