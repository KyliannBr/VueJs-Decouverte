<template>
    <setion class="halfPage">
            <div class="left">
                <div class="imgContainer">
                    <img src="../assets/halfLeft-1.png" alt="">
                </div>
                <div class="button">
                    <svg width="0" height="16" xmlns="http://www.w3.org/2000/svg"><g stroke="#fff" fill="none" fill-rule="evenodd"><path :d="path"></path></g></svg>
                    <router-link to="/about">{{text}}</router-link>
                </div>
            </div>
            
            <div class="right">
                <div class="imgContainer">
                    <img src="../assets/halfRight-1.png" alt="">
                </div>
                <div class="button">
                    <svg width="0" height="16" xmlns="http://www.w3.org/2000/svg"><g stroke="#fff" fill="none" fill-rule="evenodd"><path :d="path"></path></g></svg>
                    <router-link to="/about">{{text}}</router-link>
                </div>
            </div>
        </setion>
</template>

<script>
export default {
    name: 'HalfPage',
    data(){
        return {
            path: "M18.31 8.22H0M11.16 1l7.15 7.15-7.33 7.34",
            text: "Learn More",
        }
    }
}
</script>

<style scoped>
.halfPage {
    width: 100vw;
    height: calc(100vh - 5rem);
    display: flex;
    flex-direction: row;
}

.halfPage .left .imgContainer:hover {
    transform: scale(1.05);
    overflow-y: hidden;
}

.halfPage .right .imgContainer:hover {
    transform: scale(1.05);
    overflow-y: hidden;
}

.halfPage .left {
    width: 50%;
    height: calc(100vh - 5rem);
    position: relative;
    color: #fff;
    overflow-y: hidden;
}

.halfPage .left .imgContainer {
    width: 100%;
    height: 100%;
    background: url();
    background-position: center;
    background-size: cover;
    transition: all 1s;
    overflow-y: hidden;
}

.halfPage .right .imgContainer {
    width: 100%;
    height: 100%;
    background: url(/img/halfRight-1.png);
    background-position: center;
    background-size: cover;
    transition: all 1s;
    overflow-y: hidden;
}

.halfPage .imgContainer img {
    width: auto;
    height: 100%;
    object-fit: cover;
    object-position: center;
}

.halfPage .right {
    width: 50%;
    height: calc(100vh - 5rem);
    position: relative;
    color: #fff;
    overflow-y: hidden;
}

.halfPage a {
    background-color: transparent;
    border: none;
    font-size: 1.3rem;
    color: #fff;
    text-decoration: none;
}

.halfPage .button {
    position: absolute;
    bottom: 2rem;
    left: 2rem;

    border: solid #fff 2px;
    border-radius: 99px;
    padding: 1rem 1rem;
    transition: all .2s;
}

.halfPage .button svg {
    opacity: 0;
    translate: -10px;
    transition: all .3s;
}

.halfPage .left:hover .button {
    transition: padding 0.3s cubic-bezier(0.25, 0, 0, 1);
    padding: 1rem 1.5rem;
}

.halfPage .left:hover .button svg {
    opacity: 1;
    translate: 10px;
    width: 30px;
}

.halfPage .right:hover .button {
    transition: padding 0.3s cubic-bezier(0.25, 0, 0, 1);
    padding: 1rem 1.5rem;
}

.halfPage .right:hover .button svg {
    opacity: 1;
    translate: 10px;
    width: 30px;
}

</style>