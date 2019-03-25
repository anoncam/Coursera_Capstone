# Week 2 Capstone Coursera Course


## Introduction/Business Problem
/* Introduction where you discuss the business problem and who would be interested in this project. */

"Would/WHERE one would recommend a location in Hong Kong to open a cinema?"
The stakeholder wants to open a new cinema.  Using data science we can determine the best location for a new cinema.

From the customer point of view, watching films is a part of an experience taking an entire afternoon along with other activities. Cinemas should have  restaurants and shopping places nearby. Transportation is also an integral factor. 

Customer can walk to cinema within 5 minutes from public transport facilities such as a bus stop or a metro station.

The methodology focuses on the selection of a cinema location according to its nearby environment. A cinema's facility and rental price is a factor of concern. The stakeholder provides their 10 favorite cinemas in Hong Kong with their respective rating.

Given the above: which location should be suggested to the stakeholder?


## The Data

This section describes the data that will be used to solve the problem and the source of the data.

According to the question, the following is required, along with the Foursquare API to answer the question posed previously.

1. Geographic coordinate of Hong Kong cinemas
I need to compare 5 possible locations with current cinemas in Hong Kong. Therefore, I need to find a list of Hong Kong cinema and cinemas' geographic coordinates. Luckily, I can find the list and coordinates from the website https://hkmovie6.com/cinema .

2. **Eating, Shopping and Public transportation facility around cinema**

The recommended cinema location needs to have eating and shopping venues nearby. Location based public transport is also required.
Using the FourSquare API we can find these venues around the location.

The paramaters for suitable transportation is a bus or metro within 5 minutes walking distance or about 500m. 

The Foursquare API provides maximum 50 results, so it is better to search for venues by category. 

A list of categories can be found [here](Eating, Shopping and Public transportation facility around cinema
The recommended cinema location needs to have many eating and shopping venues nearby. Convenient public transport is also required.
I can use FourSquare API to find these venues around the location.

5 minutes walking distance is about 500m. I think it is the suitable distance to search nearby venues.
The Foursquare API limits us to 50 results, so it is more comprehensive to search venues by category.

The following categories will be used for finding the target venues. For a full list of categories: [see this list](https://developer.foursquare.com/docs/resources/categories).

This data is best suited for **content-based** recommendation in order to solve the problem.

Combined with the FourSquare API by counting how many different venues (Food, Transport, Night Life etc.) and Hong Kong cinema list, a cinema nearby a venues matrix can be built. 

The stakeholder's preference is the data to combine with cinemas and venues to create a weighted matrix of favorite cinemas.

The weighted matrix can be applied on 5 possible locations with venues information to generate a ranking result. The the most desired cinema on the ranking list will be recommended to the stakeholder.

## Methodology
In the methodology section, which represents the main components of the report allows the discussion of the methods used and describe any exploratory data analysis that was conducted, any inferential statistical testing that is performed, and what machine learning models were used and why.

## Results

This is where the results of the data is broken down both contextually and quantitatively.

## Discussion

This section allows the explaination of observations and reccomendations based on the aforementioned sections.


## Conclusion

Conclusions of the processes listed above