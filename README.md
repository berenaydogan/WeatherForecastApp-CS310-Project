This repository contains the term project we did as a team of two for the course CS310 Mobile Application Development in Sabancı University on developing mobile applications consuming web services

As a term project, we were required to develop a full native Android application. Our app, called Activity Forecast, provides the users weather information based on the specified location, as well as activity ideas based on the weather conditions.

The application requests the user to select the preferred location provided in a spinner. The weather forecast for the location is displayed after the user selects the desired location.
From there, the users are able to see activity recommendations tailored for the current weather conditions. The app uses the weather data and suggests possible activities in accordance with the forecasted weather. These activities come in two sections: indoor and outdoor so that the user can utilize the application for plans in both settings.

For all the activities provided, the application provides activity details where there is a brief information about the recommended activity and a review section where the users can share their thoughts on the activities.

The backend of this app utilizes Java with the Spring framework. The app's core components include models for Activity, Location, Review, and Weather, which are mapped to a MongoDB database using Spring Data annotations. The AppController class serves as the main controller, handling HTTP requests and responses, and managing various activities and locations based on weather conditions. It fetches real-time weather data from OpenWeatherMap API. The Activity and Review classes are linked through MongoDB references. The backend also incorporates RESTful principles, to allow integration with frontend components and external services. Current implementation of the app includes 5 cities in Turkey but it can be easily expanded. 

The frontend of this app is developed using Android Framework using Android components. The app integrates network operations for data fetching and synchronization, employing RecyclerViews and Adapters for data display. It uses fragments and dynamic UI updates to ensure the application remains responsive and user-friendly.
