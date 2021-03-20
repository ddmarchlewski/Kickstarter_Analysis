# An Analysis of Kickstarter Campaigns

## Unconvering trends by performing an analysis on Kickstarter data.  

### Help Louise start a crowdfunding campagin to help fund her upcoming play Fever.

---

# Analysis and Challeneges
 
  The first step I took here was to familiarize myself with the data I was working with. I did this by figuring out how many rows and columns were in the dataset, what data types were present, and if any data needed to converted. One challenge I came accross here after seeing all of the columns, rows, and data types was that some of the data was not readable. Columns I and J had data that looked like dates, however they were not in a readable format. So, by using a timestamp converter, I was able to convert the data in those columns into a readable format.

  From there, I created a new column to show percentages of each campaigns funding. I was able to see how close some campagins came to reaching their funding goals. Some even surpassed their goal. I also applied some conditonal formatting to this column so I can see which projects were fully funded just by looking at the color grading alone. I then made another column to show the average donation people have made to each campaign. This also came with some problems. The Average Donation column that I made created some #DIV/0! errors. To fix these errors, I used the IFERROR() forumula to replace all errors with a 0 instead. 

  Then, I split the Category and Subcategory column into two distinct columns to show some additional data: "Parent category" and "Subcategory." Then I took the data from those two columns and made a Pivot Table to better visualize the data. This chart easily shows which parent category did well and which ones did not.
![Parent Category Outcomes](https://user-images.githubusercontent.com/80054925/111880548-2aae1800-897a-11eb-8f9e-38b3a963961d.png)

  I then made another pivot table filtered it down to show only plays to see if plays did well. Based on this pivot table, I was able to determine that plays had more successful campaigns then failed. 
 ![Play Outcomes](https://user-images.githubusercontent.com/80054925/111880751-3d751c80-897b-11eb-9c3c-d6fb7b70616d.png)
 
  After seeing that play campaigns were doing good, I made a new pivot chart to see if theater campaigns were more successful at specific times of the year, which is shown here in this line chart. The chart shows that May had the most successful theater campaigns out of any month of the year.  
![Theater_Outcomes_vs Launch](https://user-images.githubusercontent.com/80054925/111882751-479c1880-8985-11eb-9b50-bda02045f457.png)

  I also wanted to see how well plays performed in May. So I filtered the chart from before down to subcatergory plays. Even though the chart didn't change much, it still shows that May was a good month for plays. 
![Play Outcomes Based on Launch Date](https://user-images.githubusercontent.com/80054925/111881450-63e88700-897e-11eb-9317-4aabd7ea47ab.png)

  Finally, I then wanted to visualize percentages of successful, failed, and canceled plays based on their funding goals. This line chart shows the relationship between goal-amount ranges and project percentages. 
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/80054925/111882783-74e8c680-8985-11eb-8a58-347527850e4a.png)

## Results

 Going off what was shown in the Outcomes Based on Launch Date pivot table, it is safe to say that May and June are really good times to launch a play campaign. I can also say that December is not a good time since their were more failed campagins then successful ones. 
 
 Plays on average that had a funding goal of $25,000 or higher are more likely to fail than succeed. 
 
 One limitation I found was the some of the ata was collected from different sources which varied the format. 
 
 Instead of a line chart for the Outcomes Based on Goal chart, a pie chart would also be acceptable here to show percentages. One would need to show successful rates and another would need to show failed rates. 
 
  
