# MyPlaces-v2

This is the second version of the project. To view the first version, please see the MyPlaces repository.

#### Introduction

Even though there are already many applications to use for places search in the mobile environment, most offer many functionalities in their applications and do not aim for a specific task. The purpose of this project is to provide the user with a simple interface that will allow them to search and keep track of the places that they saved for future reference. This can be a company address for an interview or a hike location that is planned for the weekend. Information for places is provided using the Google Places Web service. If a place’s information cannot be obtained from the web service, the application will also allow the user to add their own place to be saved.

Note this is a second version of the project. In the version, the application mainly uses the SQLite database and the Google Places web service. To add flexibility for the users, the second versions integrate Parse as a cloud back-end that will allow the users to view the saved places on different devices.


#### User and Application Requirements:

- Users will be able to create their account and login on different devices.
- Users will be able to search for nearby places in relation to their device location based on a certain keyword and radius distance    in miles.
- Users will be able to search for places based on a phrase of text. This can be an address, location name or text phrase such as     “Food around University of Washington.”
- Users will be able to view the place information, visit their website, get directions using Google Maps, call its phone number, and   save the location for future reference.
- Users will be able to view their saved places to revisit their information, share, or delete them.
- Users will be able to add their own place if it is not available through the web service.

#### Implementations:

- Uses the Google Places web service to make http requests for places search and view their information.
- Displays a place’s information by parsing the JSON data after retrieving it through a request.
- Saves the user accounts and their places on the Parse cloud backend.
- Performs permission checks as required by Android API 23 and uses the device location through LocationManager and searches for   nearby locations.
- Uses Android Intents for place’s information sharing through social media or messaging, performs number dialing from the application and launches the Google Maps application for directions.
- Uses the ContextMenu to display the delete and share place option.

