//testing lat/long distance measurement


// if event == "entity added" || "entity updated" || "entity deleted" || "field updated"?
// make a GET request to list entities endpoint
// create a dictionary
// for page in response, pull lat/long values into dictionary where key = entity ID and value = lat/long pair
// for each key in dictionary, calculate the distance btwn that entity and every other entity, store in a list, sort by smallest distance, save top five fields
// push top five entity IDs to POST entities endpoint

var lat1 = 40.7428306
var lon1 = -74.0034739
var lat2 = 40.7421853
var lon2 = -74.0057859

function myFunction(lat1, lon1, lat2, lon2) {
    var lat1r = lat1 / 57.29577951
    var lon1r = lon1 / 57.29577951
    var lat2r = lat2 / 57.29577951
    var lon2r = lon2 / 57.29577951
    var distanceInMiles = 3963.0 * Math.acos((Math.sin(lat1r) * Math.sin(lat2r)) + Math.cos(lat1r) * Math.cos(lat2r) * Math.cos(lon2r - lon1r))
    var distanceInKm = 1.609344 * distanceInMiles 
    return distanceInKm
}

console.log(myFunction(lat1,lon1,lat2,lon2))
