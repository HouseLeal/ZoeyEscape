// Hooray Arrays1
var beginningScenario = ["You are trying to go to bed but Zoey is in your spot", 
"You want to brush your teeth but Zoey is sitting on your toothbrush", 
"You want to make Zoey a cake but she cant digest sugar"];

var weapon = ["the pear of anguish", "zoeys other half of her ear", 
"cyanide laced catnip", "an Illy punch"];

var occupation = ["guns rights activist", "youtuber", "Trump supporter", ]

//VERY VARIABLE
var randomOccupation = occupation[ (rando ( occupation.length -1))];
var survival = rando(2);
var randomWeapon = weapon[ (rando (weapon.length - 1))];

//CONJUNCTION FUNCTIONS
function rando(range){
	return Math.round(Math.random() * range);
}

//GO TIME!
alert(beginningScenario [rando (beginningScenario.length - 1) ] );
alert("This angers you.  You search for a weapon to battle Zoey.....");
alert("Oh yay! You find: " + randomWeapon);

if (survival === 0){
	alert("Zoey self destructs and creates a blast radius of 27.4 miles.  You survive the blast but now you encounter a " + randomOccupation);
}
else{
	alert("You beat Zoey with " + randomWeapon + " and go about your day like a normal human after its beaten a cat");
}

var goOn = prompt("Do you wish to take on the " + randomOccupation + " ? (y or n)");

if (goOn == 'y'){
	alert("The " + randomOccupation + " brings Zoey back to life and beats you with: " + randomWeapon);
}
else
	alert("The " + randomOccupation + " will not honor your surrender and beats you with: " + randomWeapon);

