# UFOs
McMinnville is famous for its sightings and even has an annual Gathering of UFO enthusiasts. W. Avy, a UFO-enthusiast and amateur ufologist, helped us to research and fill `data.json` file with the mysterious objects seen in the sky in the McMinnville area.

Tina is a data journalist who wanted to reconnect with her hometown McMinnville Oregon, to revisit the memories and people back home and know about UFOs. In this Module we helped her to build a Dynamic Web Page. 

Using JavaScript ES6+, we converted Json objects into objects that HTML can interpret as table's elements and added a function that can hear the user's inputs to filter the table. Because there's so much data, sifting through it without any adjustments would be a challenge. JavaScript provides a way to manipulate the data by adding filters.

![HTML Final Module](https://github.com/RebecaOsorio/UFOs/blob/main/images/HTML/Final%20Module%20HTML.png)



## Overview of the analysis

Dana’s webpage and dynamic table are working as intended, but she’d like to provide a more in-depth analysis of UFO sightings by allowing users to filter for multiple criteria at the same time. In addition to the date, there will be table filters for the city, state, country, and shape.

![Delivery Results](https://github.com/RebecaOsorio/UFOs/blob/main/images/HTML/Challenge%20Delivery%202%20Results.png)

### Resources

To accomplish this project, we used:

-   **Data Source:**  [`data.json` file](https://github.com/RebecaOsorio/UFOs/blob/main/static/js/data.js), research generously funded by W. Avy
    
-   **Software:**  VS Code 1.64.2(user setup)-*as our code interpreter*.
We will also use basic HTML , Bootstrap and CSS to build and style the entire page. And finally, JavaScript version VS6+ to populate and dynamically filter a table.


## Results

Unfortunately, Dana couldn't get data from her childhood hometown because there wasn't any record of UFOs in the McMinnville, Oregon area. 

The UFO enthusiasts should keep track of its sightings!

![Dana's Searching Results](https://github.com/RebecaOsorio/UFOs/blob/main/images/HTML/Challenge%20Delivery%202%20Dana%27s%20Results.png)


Any way, if we zoom out the searching, we find that some mysterious objects were seen in the state of Oregon. Not her hometown, but  somewhat closer.

![Dana's Results Zoomed Out](https://github.com/RebecaOsorio/UFOs/blob/main/images/HTML/Challenge%20Delivery%202%20Dana%27s%20Results%20Reduced.png)

## Summary
As seen in the **Results** Section the database is small. We should include a *Contribute* page so the users can update the `data.js` file.


For now, we can add `placeholder` tags in each filter so the costumer can look how to introduce the data.

![PlaceHolders](https://github.com/RebecaOsorio/UFOs/blob/main/images/HTML/PlaceHolder.png)



And what happens when the user is just playing with the database? It's easy to input invalid parameters.

For this reason, when the filtered table doesn't have data, a random object from the `data.js` will be displayed in the console

![Invalid Inputs](https://github.com/RebecaOsorio/UFOs/blob/main/images/HTML/Invalid%20Inputs.png)



## Code Overview
Modifying `index.html`, we'll create more table filters for the city, state, country, and shape.

Using JavaScript, we’ll replace the `handleClick()` in the `app.js` file with a new function that saves the **element**, **value**, and **id** of the filter that was changed. Then, in a new function, we'll to loop through the dataset and keep only the results that match the search criteria. The webpage will be updated with the search criteria after pressing "Enter".
