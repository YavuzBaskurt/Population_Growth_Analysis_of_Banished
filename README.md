# Population_Growth_Analysis_of_Banished
## **Idea & Motivation**
For this project, I have decided to look into how a settlement building game, Banished, handles population growth. My aim with this project, beyond analyzing a game I've played in an academic setting, is to gain insight on population growth models as a whole, an important problem with many real life applications. Population growth in Banished depends, among other non-negligible factors I have chosen to omit because they are only applicable many in-game years after the start of a new save file, on three major factors: The current adult population, as more people can give more births provided they aren't limited by other factors; the amount of food stockpiled, where if there isn't a surplus of food available, a famine will cause a sharp decline in population until food production is back in order; and the number of available housing, people in Banished cannot give birth without enough space.
 
## **The Dataset**
I will collect the data on current population and available food by interacting with a building which lists some important information about the settlement. For the number of available housing I can simply count the total number of houses, multiply it by 5 since I will only use housing units with a capacity of 5, and subtract from the existing population. Population in Banished is categorized into two main groups: Adults and children.

  **Number of adults**: The game keeps track of this and I can access it through a building available to me immediately.
  
  **Number of children**: Available in the same way as the number of adults. I will need to keep track of this separately to look for any decrease in population caused by a lack of children growing into adults while an aging population sees many deaths.

  **Adults delta**: The change in the number of adults year-to-year
