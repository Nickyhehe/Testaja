<script>
export default{
    name: 'Header',
}

</script>


<template>
    <header>
        <img src="../assets/ghibli.jpg" alt="">
        <div class="intro">
            <div class="animate__animated animate__fadeInDown">
                <h1 >Hello, My name is <br>
                <span>Nicky Dharmawan</span></h1>
            </div>
            
        </div>
    </header>

</template>

<style lang="scss">

html, body {
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100%;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    background: rgb(217,94,101);
background: linear-gradient(90deg, rgba(217,94,101,1) 0%, rgba(93,206,201,1) 0%, rgba(217,94,101,1) 100%);
}

    header{
         position: relative;
        img{
            width: 100%;
            height: 100vh;
       
        }
        .intro{
            position:absolute;
            top: 20%;
            left: 50%;
            transform: translate(-50%, -50%);
            
            animation:  fade-in 1.3s ease-in-out forwards;
            
            
            h1{
               
                color: rgb(217,94,101);;
                font-size: 40px;
                font-weight: 400;
              
                span{
                    font-weight: 800;
                    font-size: 50px;
                }
            }
        }

    }
</style>