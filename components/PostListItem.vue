<template>
<div class="post">
    <img :src="item.image" alt="post image" class="h-80 w-65 object-cover ml-5 mr-5 my-5" >
    <h3 class="mr-0.5">{{item.title}}</h3>
    <p class="text-white-500">{{item.description}}</p>
</div>
</template>

<script>
export default {
    props:['item'],
    data() {
        return {

        }
    }
}
</script>

<style>



.post{
order: 0;

display: flex;

justify-content:center;
flex-direction: column;
transition: transform .2s;
margin-top: 70px;
background-color: black;
color: white;
width: 310px;
height: 350px;
/* padding-left: 45px;
padding-bottom: 10px; */
border-radius: 10px;


}

/* .post:hover p {
  transform: scaleY(0.66)
} */

.post:hover {
  transform: scale(1.15);
  /* transform: scaleX(1.2); */
  /* transform-origin: bottom; */
  
}
</style>