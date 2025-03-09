# Population_Growth_Analysis_of_Banished
## **Idea & Motivation**
For this project, I have decided to look into how a settlement building game, Banished, handles population growth. My aim with this project, beyond analyzing a game I've played in an academic setting, is to gain insight on population growth models as a whole, an important problem with many real life applications. Population growth in Banished depends, among other non-negligible factors I have chosen to omit because they are only applicable many in-game years after the start of a new save file, on three major factors: The current adult population, as more people can give more births provided they aren't limited by other factors; the amount of food stockpiled, where if there isn't a surplus of food available, a famine will cause a sharp decline in population until food production is back in order; and the number of available housing, people in Banished cannot marry without available housing.
 
## **The Dataset**
I will collect the data on current population and available food as I play the game by interacting with a building which lists some important information about the settlement. I will repeat that interaction at the start of each in-game year. The number of available housing is near impossible to keep track of since new couples in Banished always need to move into an empty house, but I can draw some conclusions from the total number of housing I've built. Population in Banished is categorized into two main groups: Adults and children, and it will be important within my dataset to measure them separately.

  **Number of adults**: The game keeps track of this and I can access it through the building mentioned before.
  
  **Number of children**: Available in the same way as the number of adults. I will need to keep track of this separately to look for any decrease in population caused by a lack of children growing into adults while an aging population sees many deaths.

  **Children delta**: The change in the number of children year-to-year.

  **Adults delta**: The change in the number of adults year-to-year.

  **Stockpiled food**: The number of food units stored at the start of each year. Each person, whether they are a child or adult, needs to eat around 100 units of food every year in order to survive, otherwise they will starve. 

  **New Housing**: The amount of housing built in the previous year.
