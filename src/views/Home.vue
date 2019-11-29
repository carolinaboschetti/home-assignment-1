<template>   
    <div class="hello">
    <h1 class="title">Conheça algumas opções de doces</h1>
        <div class="options">
            <Cupcake v-for="(cupcake, i) in cupcakes" :key="i" :cupcake="cupcake" />
        </div>
         <div>
            <button>Faça um teste!</button>
            <p>Cupcake Voluptatibus animi magni blanditiis voluptate deserunt, recusandae quasi enim sit! Natus!</p>
        </div>
  </div>
</template>

<script>
import Cupcake from '@/components/Cupcake.vue'
// @ is an alias to /src

export default {
    name: "home",
    components: {
        Cupcake
    },
    data() {
        return {
            cupcakes: [
                {
                    title: 'Opção X',
                    desc: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vel quaerat cupiditate quibusdam ipsam beatae. Numquam culpa explicabo sunt deserunt, assumenda, nesciunt possimus quasi in voluptates expedita, repellendus ea odit reprehenderit!',
                    stuff: [
                        'Candy canes cheesecake',
                        'Apple pie wafer',
                        'Tiramisu cupcake',
                        'Lemon drops faworki'
                    ]
                },
                {
                    title: 'Opção Y',
                    desc: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vel quaerat cupiditate quibusdam ipsam beatae. Numquam culpa explicabo sunt deserunt, assumenda, nesciunt possimus quasi in voluptates expedita, repellendus ea odit reprehenderit!',
                    stuff: [
                        'Tootsie roll cheesecake',
                        'Chupa Chups wafer',
                        'Danish marzipan'
                    ]
                },
                {
                    title: 'Opção Z',
                    desc: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Vel quaerat cupiditate quibusdam ipsam beatae. Numquam culpa explicabo sunt deserunt, assumenda, nesciunt possimus quasi in voluptates expedita, repellendus ea odit reprehenderit!',
                    stuff: [
                        'Chocolate marzipan jelly',
                        'Sweet lollipop ice cream',
                        'Soufflé jelly-o bear claw sweet',
                        'Brownie pie gummi bears',
                        'Jelly beans dragée'
                    ]
                }
            ]
        }
    }
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
    text-align: center;
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

