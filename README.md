# nombre-premier



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <title>Calcul des nombres premiers</title>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
  <h1>Calcul des nombres premiers</h1>
  <label for="number">Entrez un nombre :</label>
  <input type="number" id="number">
  <button onclick="calculatePrimes()">Calculer</button>
  <p id="result"></p>

  <script >
  <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <title>Calcul des nombres premiers</title>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
  <h1>Calcul des nombres premiers</h1>
  <label for="number">Entrez un nombre :</label>
  <input type="number" id="number">
  <button onclick="calculatePrimes()">Calculer</button>
  <p id="result"></p>

  <script >
   // Function to calculate prime numbers
function calculatePrimes() {
  // Get the value entered by the user and convert it to an integer
  var number = parseInt(document.getElementById("number").value);
  // Initialize an empty array to store the prime numbers
  var primes = [];

  // Loop to iterate from 2 to the given number
  for (var i = 2; i <= number; i++) {
    // Check if the current number is prime by calling the helper function isPrime()
    if (isPrime(i)) {
      // If the number is prime, add it to the array of prime numbers
      primes.push(i);
    }
  }

  // Get the HTML element to display the result
  var resultElement = document.getElementById("result");
  // Update the content of the HTML element with the found prime numbers
  resultElement.textContent = "Voici les nombres premiers entre 1 et " + number + ": " + primes.join(", ");
}

// Helper function to check if a number is prime
function isPrime(num) {
  // Loop to iterate from 2 to the square root of the number
  for (var j = 2; j <= Math.sqrt(num); j++) {
    // Check if the number is divisible by another number (non-prime)
    if (num % j === 0) {
      // If the number is divisible, it is not prime
      return false;
    }
  }
  // If the loop completes without finding divisors, the number is prime
  return num > 1;
}


  </script>
</body>
</html>

<style>
    body {
  font-family: Arial, sans-serif;
  text-align: center;
}

h1 {
  color: #333;
}

label {
  font-weight: bold;
}

input {
  padding: 5px;
}

button {
  padding: 8px 16px;
  background-color: #3f3f3f;
  color: white;
  border: none;
  cursor: pointer;
}

button:hover {
  background-color: #0f100f;
}

#result {
  margin-top: 20px;
  font-weight: bold;
}

</style>

  </script>
</body>
</html>

<style>
    body {
  font-family: Arial, sans-serif;
  text-align: center;
}

h1 {
  color: #333;
}

label {
  font-weight: bold;
}

input {
  padding: 5px;
}

button {
  padding: 8px 16px;
  background-color: #3f3f3f;
  color: white;
  border: none;
  cursor: pointer;
}

button:hover {
  background-color: #0f100f;
}

#result {
  margin-top: 20px;
  font-weight: bold;
}

</style>
