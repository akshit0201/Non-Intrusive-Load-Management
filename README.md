# Non-Intrusive-Load-Management
Machine Learning model for finding user's appliance level data based on smart meter data.

The given model is trained on the [REFIT dataset](https://pureportal.strath.ac.uk/en/datasets/refit-electrical-load-measurements). Once the dataset is downloaded, the steps from **Extracting Variables** can be followed. 

In the uploaded Ipynb data from *House 2* of the REFIT dataset is analyzed , but the given model can be used to learn the data from any appliance in any house: 

![model](https://github.com/akshit0201/Non-Intrusive-Load-Management/blob/7293cc37ee0fa1d8011f94314b695f72207725a5/model.png)

Input consists of a *non-overlapping sliding window* containing *aggregate power* and *Unix time*. The length of the window is taken as **128 units** for short duration appliances and **512 units** for long duration appliances. 

A satisfactory model accuracy of around **75 percent** is acheived for each of the appliance , once the NILM is complete *load scheduling* and *cost optimization* can be performed on the dataset.
