var correctGuess = false;
var randomNumber = Math.floor(Math.random() * 6 ) + 1;
var guess = prompt("I am thinking of a number between 1 and 6. What is it?");
  if (parseInt(guess) === randomNumber ) {
  correctGuess = true;
} 
if ( correctGuess ) {
    document.write('<p>You guessed the number!</p>');
} 

else if (parseInt(guess) < randomNumber){
  var guessMore = prompt("You have guessed " + guess + ". my number is larger than your guess")
}

if (parseInt(guess) === randomNumber){
  correctGuess = true;
}

else if (parseInt(guess) > randomNumber){
  var guessMore = prompt("You have guessed " + guess + ". my number is smaller than your guess")
}
  if (parseInt(guess) === randomNumber){
 correctGuess = true;
}

   if (correctGuess){
  document.write("You guess right!")
}
else {
    document.write("<p>Sorry. The number was " + randomNumber + ".</p>");
}
