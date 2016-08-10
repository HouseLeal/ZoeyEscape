# ZoeyEscape
a simple JS escape game

alert("You are trying to go to the bathroom.  Zoey sits quietly in the hallway, staring at you.... ");

var weapon = prompt("You decide to battle: What is your weapon of choice? Spoon | Dagger | Guitar | Soap")
var randomNum = Math.round(Math.random());

console.log(randomNum);
console.log(weapon);

alert("You battle with Zoey, armed with " + weapon);

if (randomNum === 0){
  alert("MeOWWWWW   Zoey claws your leg and scratches your face! She knocks the " + weapon + " out of your hand");
  var move = prompt("Bloody and barely breathing, you chose to: Bite | Claw | Run");
}
else if (randomNum === 1){
  alert("You whoop zoey with " + weapon + " YOU WIN! HAPPY SHITTING!");
}

console.log(move);

if (move == "Bite"){
  alert("You bite Zoey in half but her tail half smacks you and you go flying accross the room");
}
else if (move == "Claw"){
  alert("Zoey blocks your claw attack and kicks you in the mouth.  She calls you Claw Aikens and walks away like a boss");
}
else {
  alert("Run! Hooman RUN!!!!");
}
