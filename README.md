# SNHU_CS360_Project
Full-stack Android inventory app written in Java using Android Studio for CS-360: Mobile Architecture and Programming.

## Briefly summarize the requirements and goals for the app you developed. What user needs was this app designed to address?
This Inventory App was intended to allow viewing and manipulation of items in a warehouse. Business owners, employees, and small-scale sellers can use this application to track inventory items with their corresponding prices and quantities. This eliminates the need for archaic solutions like pen-and-paper.

## What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?
The application includes a login screen, a grid list of items, an add items screen, and an item details screen. These screens are very simple to navigate to and within, and the available actions for users to perform are limited and clear. I believe the designs were successful because they avoid overwhelming users with too many options at once.

## How did you approach the process of coding your app? What techniques or strategies did you use? How could those be applied in the future?
I employed incremental development to code the app. I personally like development methodologies like Agile where the development process is broken up into sections that are both designed and developed incrementally. I understand that Agile is common in this field of work, and I intend to translate this experience to it.

## How did you test to ensure your code was functional? Why is this process important and what did it reveal?
Testing of this application was entirely manual; I did not make use of powerful testing tools like JUnit. The number of features available in the application are limited, so I was able to test them manually with relative ease. I did find on multiple occasions that some UI components or database interactions were not working, and fixed them promptly.

## Considering the full app design and development process, from initial planning to finalization, where did you have to innovate to overcome a challenge?
Finding a way to access the application Context and databases from anywhere in the app proved to be a bit of a challenge. The non-Activity class InventoryItem needed to be able to fire a notification when an InventoryItem's quantity was set to or below zero within its setQuantity() method, but this requires access to the application Context. I had to employ the singleton pattern to handle this in the InventoryApp class.

## In what specific component from your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?
I think that building the InventoryApp singleton (which granted access to the Context as well as both the Login and Items databases) was the clearest demonstration of my skills. This was not specifically outlined in the course materials and was thus something I needed to build on my own. I have experience working with singletons on personal projects in the past and was fortunately able to recognize that the pattern was a good solution to the issue I faced when developing this app.
