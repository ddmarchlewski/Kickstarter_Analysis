# An Analysis of Kickstarter Campaigns

## Unconvering trends by performing an analysis on Kickstarter data.  

### Help Louise start a crowdfunding campagin to help fund her upcoming play Fever.

---

# Analysis and Challeneges
 
 The first step I took here was to familiarize myself with the data I was working with. I did this by figuring out how many rows and columns were in the dataset, what data types were present, and if any data needed to converted. One challenge I came accross here after seeing all of the columns, rows, and data types was that some of the data was not readable. Columns I and J had data that looked like dates, however they were not in a readable format. So, by using a timestamp converter, I was able to convert the data in those columns into a readable format.

  From here, I created a new column to show percentages of each campaigns funding. I was able to see how close some campagins came to reaching their funding goals. Some even surpassed their goal. I also applied some conditonal formatting to this column so I can see which projects were fully funded just by looking at the color grading alone. I then made another column to show the average donation people have made to each campaign. This also came with some problems. The Average Donation column that I made created some #DIV/0! errors. To fix these errors, I used the IFERROR() forumula to replace all errors with a 0 instead. 

  Then, I split the Category and Subcategory column into two distinct columns to show some additional data: "Parent category" and "Subcategory." Then I took the data from those two columns and made a Pivot Table to better visualize the data from the table. This table easily shows which parent category did well and which ones did not.
![Parent Category Outcomes](https://user-images.githubusercontent.com/80054925/111880548-2aae1800-897a-11eb-8f9e-38b3a963961d.png)
