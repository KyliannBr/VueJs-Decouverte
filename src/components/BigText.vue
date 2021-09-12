<template>
    <div class="bigText">
        <span class="l1"></span>
        <h2>Roccat Magma</h2>
        <span class="l2"></span>
    </div>
</template>
    
<script>

export default {
    name: 'BigText',
};

</script>

<style scoped>

    .bigText {   
        z-index: 999;
        position: absolute;
        top: 7rem;
        text-align: center;
        font-size: 5rem;
        color: var(--palePink);
        width: 100%;
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
        padding: 1rem 0;
    }
    span.l1 {
        width: 30rem;
        height: .5rem;
        background-color: aqua;
        animation: slideUp .8s ease-in-out forwards;
    }
    span.l2 {
        width: 30rem;
        height: .5rem;
        background-color: aqua;
        animation: slideDown .8s ease-in-out forwards;
    }

    p {
        margin-top: 2rem;
        font-size: 1.5rem;
        width: 30rem;
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