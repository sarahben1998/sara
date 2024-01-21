function checkSeason(month) {
  // Convert month to lowercase for case-insensitive comparison
  const lowerMonth = month.toLowerCase();

  // Check the season based on the month
  switch (lowerMonth) {
    case 'december':
    case 'january':
    case 'february':
      return 'Winter';

    case 'march':
    case 'april':
    case 'may':
      return 'Spring';

    case 'june':
    case 'july':
    case 'august':
      return 'Summer';

    case 'september':
    case 'october':
    case 'november':
      return 'Autumn';

    default:
      return 'Invalid month'; // Return an error message for invalid input
  }
}

// Example usage:
const currentMonth = 'January';
const currentSeason = checkSeason(currentMonth);
console.log(`You are currently in ${currentSeason}.`);









// Generate a random number between 0 and 3 (inclusive)
const randomizer = Math.floor(Math.random() * 4);

// Determine fate based on the random number
let fate;

if (randomizer === 0) {
  fate = "A certain victory";
} else if (randomizer === 1) {
  fate = "Not so certain victory";
} else if (randomizer === 2) {
  fate = "An uneasy victory";
} else {
  fate = "Your fate is unclear, ô chosen undead";
}

// Output the result
console.log(fate);


