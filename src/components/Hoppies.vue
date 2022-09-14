<template>
    <div class="hoppies">
        <div class="songs">
            <header class="songs-header">my playlist songs</header>
            <audio controls autoplay>
                <source src="../assets/01.mp3" type="audio/mpeg">
            </audio>
            <audio controls>
                <source src="../assets/02.mp3" type="audio/mpeg">
            </audio>
            <audio controls>
                <source src="../assets/03.mp3" type="audio/mpeg">
            </audio>
        </div>
        <div class="languages">
            <header class="languages-header">languages</header>
            <div class="container">
                <div class="english-parent">
                    <div class="rounded">
                        <div class="child"></div>
                    </div>
                </div>
                <div class="arabic-parent">
                    <div class="rounded">
                        <div class="child"></div>
                    </div>
                </div>
            </div>
            
        </div>
        <div class="courses">
            <header class="courses-header">courses</header>
            <div class="first-course">
                <h3 class="course-name">Front-End Development - Udacity</h3>
                <p class="course-details">(Html - Css & Advanced Css - JavaScript)</p>
            </div>
        </div>
    </div>
</template>
<script>


    export default {
        name:"Hoppies",
        data(){
            return{
                name:"hoppies"
            }
        },
        methods:{
            addClass:function(){
                    let roundedElements = document.querySelectorAll(".rounded");
                    roundedElements.forEach((rotation)=>{
                        setTimeout(()=>{
                            rotation.classList.add("rotate");
                        },200)
                        
                    })
            },
        },
        mounted(){
            this.addClass();
        }
    }
    
</script>