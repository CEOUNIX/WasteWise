# WasteWise
// Define an array to store waste disposal records
let wasteRecords = [];

// Function to add a waste disposal record
function addWasteRecord(date, wasteType, amount) {
  const record = { date, wasteType, amount };
  wasteRecords.push(record);
}

// Function to get waste disposal records by date
function getWasteRecordsByDate(date) {
  return wasteRecords.filter(record => record.date === date);
}

// Example usage:
addWasteRecord('2023-07-14', 'Plastic', 2.5);
addWasteRecord('2023-07-14', 'Paper', 1.8);
addWasteRecord('2023-07-15', 'Glass', 0.5);

console.log(getWasteRecordsByDate('2023-07-14'));
