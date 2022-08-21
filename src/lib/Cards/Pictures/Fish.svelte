<div class="wrap"><div class="spike"></div><div class="tail"></div><div class="trunk"><div class="eye"></div><div class="eye" id="eye2"></div><div class="lip"></div><div class="lip" id="lip2"></div></div></div>




<style>
.trunk{
    height: 60px;
    width:70px;
    border:solid black 4px;
    background-color: rgb(110, 193, 175);
    border-radius: 40px;
    position:relative;

}
.lip{
  height:10px;
  width:20px;
  border-radius:20px;
  background-color: rgb(59, 146, 137);
  z-index:1;
  border: solid black 4px;
  position:absolute;
  top: 25px;
  left:-5px;

}
#lip2{
    top:35px;
}
.eye{
    height:10px;
    width:10px;
    border-radius: 100%;
    background:black;
    z-index:1;
    position:absolute;
    top:10px;
}
#eye2{
left: 20px;
}
.tail{
height:30px;
width:30px;
border: solid black 4px;
position:absolute;
right:-10px;
top:30px;
transform:rotate(45deg);
z-index:0;
background-color:rgb(59, 146, 137);
}
.wrap{
    height:100px;
    width:100px;
    display: flex;
    align-items: center;
    justify-content: center;
    position:relative;

}
.spike{
    height:20px;
    width:20px;
    border: solid black 4px;
    transform: rotate(45deg);
    position:absolute;
    top:10px;
    left:40px;
    background:rgb(59, 146, 137);
}
</style>
