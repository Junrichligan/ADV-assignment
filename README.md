// 1. Create a variable using var to store your name.
var myName = "Bisacoder";

// 2. Create a variable using let to store your age, but store it as a string, not a number.
let myAge = "Twenty-two";

// 3. Create a constant PI with the value 3.1416 and try reassigning it — observe the error.
const PI = 3.1416;
// Uncomment the next line to see the error:
// PI = 3.15; // TypeError: Assignment to constant variable.

// 4. Create variable boolean is Student, but set it dynamically to true if your age is less than 25, otherwise false.
let isStudent = Number(22) < 25;

// 5. Create an object person with nested properties.
let person = {
	name: "Justin",
	age: "22",
	address: {
		street: "123 Main St",
		city: "Nabunturan City",
		country: "Philippines"
	},
	hobbies: ["reading", "coding", "music"]
};

// 6. An array colors containing at least 5 color names (include at least one repeated value).
let colors = ["red", "blue", "green", "yellow", "blue"];

// 1. Reverse and Transform
let words = ["apple", "banana", "grape", "orange", "melon"];
let transformed = [];
for (let i = 0; i < words.length; i++) {
	let reversed = "";
	for (let j = words[i].length - 1; j >= 0; j--) {
		reversed += words[i][j];
	}
	transformed.push(reversed.toUpperCase());
}
console.log("Transformed words:", transformed);

// 2. Filtering and Counting
let numbers = [12, 45, 67, 23, 90, 32, 11, 9, 28];
let evenAndGreaterThan20 = [];
let count = 0;
for (let num of numbers) {
	if (num % 2 === 0 && num > 20) {
		evenAndGreaterThan20.push(num);
		count++;
	}
}
console.log(`Found ${count} numbers: [${evenAndGreaterThan20.join(", ")}]`);
