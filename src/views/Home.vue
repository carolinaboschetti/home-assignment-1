<template>
    <div class="hello">
    <h1 class="title">Conheça algumas opções de doces</h1>
        <div class="options">
            <div class="optionx">
                <h2>Opção X</h2>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vel quaerat cupiditate quibusdam ipsam beatae. Numquam culpa explicabo sunt deserunt, assumenda, nesciunt possimus quasi in voluptates expedita, repellendus ea odit reprehenderit!</p>
                <ul class="list">
                    <li>Candy canes cheesecake;</li>
                    <li>Apple pie wafer;</li>
                    <li>Tiramisu cupcake;</li>
                    <li>Lemon drops faworki;</li>
                </ul>
                <button>Veja Mais</button>
            </div>
            <div class="optiony">
                <h2>Opção Y</h2>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vel quaerat cupiditate quibusdam ipsam beatae. Numquam culpa explicabo sunt deserunt, assumenda, nesciunt possimus quasi in voluptates expedita, repellendus ea odit reprehenderit!</p>
                <ul class="list">
                    <li>Tootsie roll cheesecake;</li>
                    <li>Chupa Chups wafer;</li>
                    <li>Danish marzipan;</li>
                </ul>
                <button>Veja Mais</button>
            </div>
            <div class="optionz">
                <h2>Opção Z</h2>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vel quaerat cupiditate quibusdam ipsam beatae. Numquam culpa explicabo sunt deserunt, assumenda, nesciunt possimus quasi in voluptates expedita, repellendus ea odit reprehenderit!</p>
                <ul class="list">
                    <li>Chocolate marzipan jelly;</li>
                    <li>Sweet lollipop ice cream;</li>
                    <li>Soufflé jelly-o bear claw sweet;</li>
                    <li>Brownie pie gummi bears;</li>
                    <li>Jelly beans dragée;</li>
                </ul>
                <button>Veja Mais</button>
            </div> 
        </div>
         <div>
            <button>Faça um teste!</button>
            <p>Cupcake Voluptatibus animi magni blanditiis voluptate deserunt, recusandae quasi enim sit! Natus!</p>
        </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "home",
};
</script>

<style scoped lang="scss">
body > * {
    background-color: #ffffff;
    padding: 10px 20px 20px;
    width: 70%;
    margin: auto;
}
.carroussel > img{
    width: 100%;
}
h1 {
    color: #ee2961;
    padding: 10px 0;
}
h2{
    color: #ee2961;
}
 .options{
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: flex-start;
    padding: 10px;
} 
button{
  padding: 5px;
  border-radius: 12%;
  background-color: #ee2961;
  color: #ffffff;
}
  
@media (min-width: 768px) and (max-width: 1023px){
  //tablet
  .options{
    flex-direction: row;
  }
}
@media (min-width: 1024px) {
    //desktop
    .options{
    flex-direction: row;
  }
}

</style>

