<template>
  <div class="cards" >
    <div  @click="$emit('map', i)" class="dates">
        <i class="fa-solid fa-plus"></i>
        <p>{{live.date}}, {{live.festival}}, {{live.country}}</p>
    </div>
    <div v-show="live.visible" >
        <div  class="maps">
            <img src="../../assets/img/maps.png" alt="maps">
            <div class="text_maps" >
                <h4>Untold Stories</h4>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Iusto, dolorum ipsam, nihil possimus illum totam vitae cupiditate voluptatem autem vero praesentium fugiat incidunt saepe et nostrum, esse cum quas beatae!</p>
                <button>BOOK NOW</button>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: "CardDates",
    props: {
        live: Object,
        i: Number,
    },
    
}
</script>

<style lang="scss" scoped>
.cards {
    background-color: #323844;
    

    .dates {
        color: var(--color-primary);
        display: flex;
        align-items: center;
        gap: 1.25rem;
        padding: 10px;
        cursor: pointer;
    }

    p {
        margin: 0;
    }

    i {
        color: white;
        font-size: 8px;
        margin-left: 1.25rem;
    }

    
    
        
        .text_maps {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            color: white;

            h4 {
                padding-top: 1.25rem;
                font-size: 30px;
            }

            p {
                color: #7d7b8d;
            }

            button {
                background-color: var(--color-primary);
                border: none;
                color: white;
                padding: 10px 0px;
                width: 20%;
                
            }
        }
        

        img {
            height: 200px;
        }
    
}
.maps {
    padding: 20px;
    gap: 4rem;
    display: flex;
   
} 
.active {
    opacity: 1;
    max-height: 1000px;
}  
</style>