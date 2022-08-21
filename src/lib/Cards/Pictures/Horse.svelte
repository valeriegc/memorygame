<article class="container">
    <div class="head">
        <div class="ear leftEar"></div>
        <div class="ear rightEar"></div>
        <div class="eye leftEye"></div>
        <div class="eye rightEye"></div>
        <div class="nose">
            <div class="nostril leftNostril"></div>
            <div class="nostril rightNostril"></div>
        </div>
    </div>
    <div class="body"></div>
</article>

<style>
.container{
    margin-top: 35px;
    position: relative;
}
div{
    background: rgb(98, 63, 44);
    border-radius: 50%;
    border: 4px solid black;
}
.body{
    width: 60px;
    height: 85px;
}
.head{
    width: 40px;
    height: 70px; 
    position: absolute;
    top: -25px;
    left: 10px;
}
.ear{
    position: absolute;
    width: 10px;
    height: 25px; 
    background: rgb(54, 32, 20);
    top: -17px;
}
.leftEar{
    right: -6px;
}
.rightEar{
    left: -6px;
}
.eye{
    position: absolute;
    width: 3px;
    height: 8px; 
    background: black;
    border: white 4px solid;
    top: 20px;
}
.leftEye{    
    left: 5px;
}
.rightEye{
    right: 5px;
}
.nose{
    position: absolute;
    width: 40px;
    height: 30px; 
    background: rgb(211, 142, 99);
    top: 50px;
    left: -4px;
}
.nostril{
    position: absolute;
    width: 5px;
    height: 7px; 
    background: grey;
    top: 7px;
}
.leftNostril{
    left: 4px;
}
.rightNostril{
    right: 4px;
}
</style>