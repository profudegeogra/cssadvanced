html,
body {
  background-color: #05030a; 
  background-image: linear-gradient(0deg, #0f0c18, #050507);
  height: 100%;
  overflow: hidden;
  display:flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  align-content: flex-start;
  align-items: center;
}

.center {
  margin: 0 auto;
}

.extern-ring {
  
  background-image:radial-gradient(closest-corner at 60% 55%,rgb(95, 95, 97),rgb(116, 119, 116),rgb(112, 112, 108),rgb(175, 169, 169));
    height: 320px;
    width: 320px;
    border-radius: 100%;
    position: absolute;
    z-index: -1;
    animation-duration: 4s;
    animation-name: rotate;
    animation-iteration-count: infinite;

}


.outer-ring {
  position: absolute;
  
  height: 300px;
  width: 300px;
  background-image: repeating-linear-gradient(135deg, #eeede7 0%, #adacac 5%, #ED00AA 15%, #2FE3FE 50%, #08060a 100%);
  border-radius: 50%;
  
  /*  Rotate  */
  animation-duration: 2s;
  animation-name: rotate;
  animation-iteration-count: infinite;

}

.inner-ring {
  position: absolute;
  left: calc(50% - 140px);
  height: 280px;
  width: 280px;
  background-image:radial-gradient(closest-corner at 60% 55%,rgb(95, 95, 97),rgb(116, 119, 116),rgb(112, 112, 108),black);

  border-radius: 50%;
  animation-duration: 4s;
  animation-name: animatie2;
  animation-iteration-count: infinite;

}


@keyframes animatie1{
  0% {transform:rotate(0deg);}
  100% {transform:rotate(360deg);}
}

@keyframes animatie2{
  0% {transform:1(90deg);}
  50% {transform:1(180deg);}
  100% {transform:rotate(360deg);}
}


@keyframes rotate {
    0% {transform:rotate(0deg);}
    100% {transform:rotate(360deg);}
}



