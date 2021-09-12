<template>
    <div class="bigText">
        <span class="up"></span>
        <h2>Roccat Magma</h2>
        <span class="down"></span>
    </div>
</template>
    
<script>
export default {
    name: 'BigText',
};

// document.getElementById("barreSoulignement").animate([
//     {transform: 'translateX(-31rem)'},
//     {transform: 'translateX(0rem)'},
// ], {
//     duration: 1500,
// });

</script>

<style scoped>

    .bigText {   
        z-index: 999;
        position: absolute;
        top: 10rem;
        text-align: center;
        font-size: 5rem;
        color: var(--palePink);
        width: 100%;
        height: 10rem;
        display: flex;
        place-content: center;
        place-items: center;
        flex-direction: column;
    }
    h2 {
        z-index: 999;
        text-align: center;
        font-size: 5rem;
        color: var(--palePink);
        width: 100%;
        animation: fade 1s ease-in-out forwards; 
    }
    span.up {
        width: 30rem;
        height: .5rem;
        background-color: aqua;
        transform: translateY(0rem);
        animation: slideUp .8s ease-in-out forwards;
    }
    span.down {
        width: 30rem;
        height: .5rem;
        background-color: aqua;
        transform: translateY(1rem);
        animation: slideDown .8s ease-in-out forwards;
    }

    @keyframes slideUp {
        0% {transform: translateY(3rem); opacity: 0;};
        100%{transform: translateY(0rem); opacity: 1;}
    }
    @keyframes slideDown {
        0% {transform: translateY(-3rem); opacity: 0;};
        80% {transform: translateY(-3rem); opacity: 0;};
        100%{transform: translateY(0rem); opacity: 1;}
    }

    @keyframes fade {
        0% {
            opacity: 0;
        }
        100% {
            opacity: 1;
        }
    }

</style>