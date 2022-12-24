<template>
<div class="salaty"> САЛАТЫ   /  МЯСНЫЕ БЛЮДА   /  НАПИТКИ
    <div class="menu-block">
        <div v-for="p of pictures" :key="p.id" class="bludo-block">
            <div class="name">{{p.title}}</div>
             <div class="image-blok">
                <img :src="`image/${p.image}`"/>
            </div>
            <div class="recept">
                {{p.description}}
            </div>
        </div> 
       <!-- <div class="bludo-block">
            <div class="name">Салат из мяса индейки и мидиями</div>
            <div class="image-blok">
                <img src="image/sl 1.png"/>
            </div>
            <div class="recept">
                250 г • Филе индейки, сыр, мидии, микс салата,
                заправка соевая, 25 рублей
            </div>
        </div> 
        <div class="bludo-block">
            <div class="name">Овощи и говядина</div>
            <div class="image-blok">
                <img src="image/ sl 2.png"/>
            </div>
            <div class="recept">
                260 г • Говядина, перец сладкий, грибы, кабачок, 
                     сыр пармезан, соусная заправка, 35 рублей
            </div>
        </div> 
        <div class="bludo-block">
            <div class="name">Курица и баклажаны</div>
            <div class="image-blok">
                <img src="image/sl 3.png"/>
            </div>
            <div class="recept">
                350 г • Куриное филе, салат рукола, черри, яйцо, чипсы из баклажанов, 
                грудинка, сыр пармезан, мягкий сыр, 28 рублей
            </div>
        </div> 
    </div>
</div>
<div>Мясные блюда</div>
    <div class="menu-block2">
        <div class="bludo-block">
            <div class="name">Стейк из свинины и овощи</div>
            <div class="image-blok">
                <img src="image/gor 1.png"/>
            </div>
            <div class="recept">
                200 г. Стейк из свинины и овощи, 30 рублей
            </div>
        </div> 
        <div class="bludo-block">
            <div class="name">Паста и кнелики из говядины</div>
            <div class="image-blok">
                <img src="image/gor 2.png"/>
            </div>
            <div class="recept">
                400 г • Паста, лук, кнелики из говядины, специи, 
                сметанная подливка, 19 рублей
            </div>
        </div> 
        <div class="bludo-block">
            <div class="name">Свиная отбивная и овощи</div>
            <div class="image-blok">
                <img src="image/gor 3.png"/>
            </div>
            <div class="recept">
                400 г. Свиная вырезка, микс из свежих  
                овощей, перец, 28 рублей
            </div>
        </div> 
        <div class="bludo-block">
            <div class="name">Красная рыба и острые овощи</div>
            <div class="image-blok">
                <img src="image/gor 4.png"/>
            </div>
            <div class="recept">
                250 г • Филе красной рыбы, грибы, морковь по-корейски,
                морская капуста, базилик, специи,25 рублей
            </div>
        <div>Напитки</div>
    <div class="menu-block3">
        <div class="bludo-block">
            <div class="name"></div>
            <div class="image-blok">
                <img src="image/kon.png"/>
            </div>
            <div class="recept">
                100 г Коньяк, 30 рублей, 1 бутылка, 80 рублей
            </div>
        </div> 
        <div class="bludo-block">
            <div class="name">Вино, шампанское</div>
            <div class="image-blok">
                <img src="image/vin.png"/>
            </div>
            <div class="recept">
            100 г Вино, 15 рублей, 1 бутылка, 30 рублей
            100 г Шампанское, 10 рублей, 1 бутылка, 20 рублей  
            </div>
        </div>     
        -->
        </div>
    </div>
    

</template>


<script setup>

const pictures = [
      {id: 1, image:"sl 1.png", title:"Салат из мяса индейки и мидиями", description:"Филе индейки, сыр, мидии, микс салата, заправка соевая, 250 грамм, 25 рублей "},
      {id: 2, image:"sl 2.png", title:"Овощи и говядина", description:"Говядина, перец сладкий, грибы, кабачок, сыр пармезан, соусная заправка,260 грамм, 35 рублей "},
      {id: 3, image:"sl 3.png", title:"Курица и баклажаны", description:"Куриное филе, салат рукола, черри, яйцо, чипсы из баклажана, грудинка, сыр пармезан, мягкий сыр, 350 грамм, 28 рублей  "},
      {id: 4, image:"gor 1.png", title:"Стейк из свинины и овощи", description:"Стейк из свинины, овощи, 200 грамм, 30 рублей "},
      {id: 5, image:"gor 2.png", title:"Паста и кнелики из говядины", description:"Паста, лук, кнелики из говядины, специи, сметанная подлива, 400 грамм, 19 рублей "},
      {id: 6, image:"gor 3.png", title:'Свиная отбивная и овощи', description:"Свиная вырезка, микс из свежих овощей,400 грамм, 28 рублей "},
      {id: 7, image:"gor 4.png", title:"Красная рыба и  острые овощи", description:"Филе красной рыбы, грибы, морковь по-корейски, морская капуста, базилик, специи, 250 грамм, 25 рублей "},
      {id: 8, image:"kon.png", title:"Коньяк", description:"Коньяк, 100 грамм, 30 рублей, 1 бутылка, 80 рублей "},
      {id: 9, image:"vin.png", title:"Вино, шампанское", description:"Вино, 100 грамм, 15 рублей, 1 бутылка, 30 рублей. Шампанское, 100 грамм, 10 рублей, 1 бутылка, 20 рублей "},
    ];
</script>