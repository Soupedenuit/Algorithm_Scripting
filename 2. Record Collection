/ Setup
var collection = {
    "2548": {
      "album": "Slippery When Wet",
      "artist": "Bon Jovi",
      "tracks": [ 
        "Let It Rock", 
        "You Give Love a Bad Name" 
      ]
    },
    "2468": {
      "album": "1999",
      "artist": "Prince",
      "tracks": [ 
        "1999", 
        "Little Red Corvette" 
      ]
    },
    "1245": {
      "artist": "Robert Palmer",
      "tracks": [ ]
    },
    "5439": {
      "album": "ABBA Gold"
    }
};
// Keep a copy of the collection for tests
var collectionCopy = JSON.parse(JSON.stringify(collection));

// Only change code below this line
function updateRecords(id, prop, value) {
    
  // value === "" empty ******************************************************************************
  
  if (value === "" && prop === "album") {
    delete collection[id][prop];
  }
  
  else if (value === "" && prop === "artist") {
    delete collection[id][prop];
  }
  
  else if (value === "" && prop === "tracks") {
    delete collection[id][prop];
  }
  
  // prop === tracks ******************************************************************************
    
  else if (prop === "tracks" && collection[id].hasOwnProperty("tracks") === false) {
    collection[id][prop] = [];
    collection[id][prop][0] = value;
  }
  
  else if (prop === "tracks" && collection[id][prop] === "") {
    delete collection[id][prop];
    collection[id][prop] = [];
    collection[id][prop][0] = value;
  }
  
  else if (prop === "tracks" && collection[id][prop] !== "") {
    collection[id][prop].push(value);
  }
 
  // prop === album *******************************************************************************
  
  else if (prop === "album" && collection[id].hasOwnProperty("album") === false) {
    collection[id][prop] = value;
  }
  
  else if (prop === "album" && collection[id][prop] === "") {
    delete collection[id][prop];
    collection[id][prop] = [];
    collection[id][prop][0] = value;
  }
  
  else if (prop === "album" && collection[id][prop] !== "") {
    collection[id][prop].push(value);
  }
 
 
  // prop === artist *******************************************************************************
  
  else if (prop === "artist" && collection[id].hasOwnProperty("artist") === false) {
    collection[id][prop] = value;
  }
  
  else if (prop === "artist" && collection[id][prop] === "") {
  delete collection[id][prop];
    collection[id][prop] = [];
    collection[id][prop][0] = value;
  }
  
  else if (prop === "artist" && collection[id][prop] !== "") {
    collection[id][prop].push(value);
  }
 
  return collection;
}

// Alter values below to test your code
updateRecords(5439, "tracks", "Take a Chance on Me");

