# Application MyRistorante

This app is a basic customer reviews app to upload and interact with reviews of clients of a single restaurant. The main page allows to navigate to the other three views: to create a new review, see current reviews, and see stats.
 

The app is **responsive** and has two breakpoints as required. This is reflected in how the screen is organized. I also added a custom feature so the background color changes for each different screen setting (3 colours in total). You can play around with screen width and see for yourself. There is also a maximum width for screens of high resolution.
 

You can "Like" the different reviews and there is a setting to limit the number of likes to one per review (which would be expected). Data is stored in local browser data between sessions using hive_ce, so your data will be kept even if you close the browser and reopen. There is also data check in place so the rating number is within the allowed range. Form deosn't send otherwise.
 

Navigation is very intuitive. Use **path variables** in all reviews screen to filter content (see below).

## Link
You can find the app in this [link](https://martinruddym.github.io/Flutter-Restaurant-Reviews-App/).

## Creating a new review
Creating a new review involves adding a title and description as well as a numeric 1-5 rating. The information is stored persistently and will load into new sessions once the review is submitted. The form checks for type of data and does not allow to send e.g. a string in lieu of a numebr fo the rating.

## Seeing all reviews
This page allows to see all current reviews and give likes to them.

## Path variables
Path variables are implemented in all reviews screen to allow to filter the reviews. Add iinto the URL "/#Rating" e.g. "/5" to see only reviews whose rating is 5. This is essentially a filtering tool to provide better app usability.

## See stats
This page shows some basic calculated statistics for the restaurant, regarding total number of reviews on the app and the average rating between them.
