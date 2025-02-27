# data-analysis-project

The main file is "P4DS_A2_Data_Analysis_Project.ipynb" where the "P4DS_A2_Data_Analysis_Project.pdf" file is the pdf version of it where every coding field is compiled.

The Data

The data being used is gathered from Kaggle (https://www.kaggle.com/datasets/debashish311601/formula-1-official-data-19502022) and includes information about Formula One which is a motorsport where drivers compete against each other in open-wheel single-seater formula racing cars. Every year (season) consists of a given number of races where the first few drivers (the numbers may differ from year to year) win points toward the World Drivers' Championship (the higher a driver is placed, the more points they get). At the end of every season, the driver with the most points is named the World Champion.

The dataset being explored in this project consists of 14 files with detailed information about every season from 1950 to 2022. However, only three of these files are of interest in order to achieve the objectives of the project.

The first file is starting_grids.csv which includes information about the starting grids (starting race positions of the drivers) for every Grand Prix (race). The dataset has 9 columns:
 
 Car - The name of the car manufacturer the driver raced for
 Detail - Contains Starting-Grid value among all entries, showing this dataset contains information about the starting grids
 Driver - The name of the driver
 DriverCode - The name abbreviation of the driver
 Grand Prix - The name of the Grand Prix
 No - The racing number of the driver
 Pos - The starting position of the driver for the given Grand Prix
 Time - The qualifying time of the driver (drivers' grid places are determined by a qualifying session before the race and any potential
 penalties)
 Year - The year the given Grand Prix happened

The second file is race_details.csv which consists of information about the race results for all Grands Prix. The dataset has 11 columns:

 Pos - The position the driver finished the given Grand Prix at
 No - The racing number of the driver
 Driver - The name of the driver
 Car - The name of the car manufacturer the driver raced for
 Laps - The total amount of laps completed by the driver in the given Grand Prix
 Time/Retired - The total race time for the winner and the time difference to the winner for the rest of the drivers in the given Grand Prix
 PTS - Points won by the driver from the given Grand Prix
 Year - The year the given Grand Prix happened
 Grand Prix - The name of the Grand Prix
 Detail - Contains Race-Result value among all entries, showing this dataset contains information about the race results
 DriverCode - The name abbreviation of the driver
 
  The last file of interest is driver_standings.csv, containing information about the number of points earned by every driver and their corresponding positions in the Drivers' Championship at the end of every season (i.e. Driver Standings). The dataset has 7 columns:
  
 Pos - The position of the driver in the Driver Standings at the end of the given year
 Driver - The name of the driver
 Nationality - The abbreviation of the country the driver raced for
 Car - The name of the car manufacturer the driver raced for
 PTS - Total amount of points earned by the driver through the year
 DriverCode - The name abbreviation of the driver
 Year - The year the Driver Standings is for
 
 The author of the dataset (https://www.kaggle.com/debashish311601) states that the information in the dataset is taken from the official website of Formula One. Based on this statement, the information should be the most accurate possible. However, it cannot be trusted that the information comes from the official website of the sport indeed and even if this is the case, errors are still possible when transferring the data. Additionally, the information on the official Formula One website might be incorrect or missing in places itself, even though it should be the most reliable source. One quick glance at the starting_grid.csv and the race_details.csv files shows that the first one contains information about 5 races happened in 1950 while the second file contains information about 7 races happened in 1950, which shows that there is missing information in the datasets, indeed.
 
 When looking at the dataset on the Kaggle website (https://www.kaggle.com/datasets/debashish311601/formula-1-official-data-19502022), its usability is marked as 9.71 by the system. The dataset received a score of 100% on all the three main characteristics - Completeness, Credibility, Compatibility. All these measurements show that the dataset is well organised, well-documented and easy to understand and work with. Furthermore, short useful descriptions are included for every of the 14 files in the dataset and for the dataset itself, making the understanding of the purpose of the dataset very clear. Additionally, the features in every of the 14 datasets corresponds very well to their corresponding descriptions, which makes the work with them much easier. Overall, the dataset is well-structured and well-described, making it easy to work with.
 
 Project Aim and Objectives
 
 The beginning of Formula One dates back to 1950 and since then the sport has seen numerous Grand Prix winners and World Driver Champions. The aim of this project is to go through the rich sport's history and provide data analysis about some of the important aspects of the sport. Formula One has developed a lot during the years and is considered the pinnacle of the motorsports. The sport is very complicated and consists of many aspects. On one hand, the sport is one of the most technological sports in the world and teams consists of hundreds of people all contributing to constructing the fastest possible car. Usually the car performance is the biggest difference between the overall teams' and drivers' performances on track. On the other hand, however, the drivers' condition both physical and mental is also of huge importance and is often what makes the difference between teammates as they usually drive the same car in terms of performance. The motivation behind this data analysis project is to investigate whether there are some connections between drivers' race start positions and the following race results as well as between the number of race wins and the Drivers' Championship. Because the sport is so complex, the focus of this project is just on the pure race results and the points earned by the drivers toward the World Drivers' Championship. More precisely, the project takes into consideration the starting grid and the final race results for every Grand Prix as well as the final World Drivers' Championship for every season in order to achieve the project's objectives described below.
 
 Specific Objective(s)
 
 The current data analysis project aims to answer the following three questions (the project's objectives):
 
 Objective 1: Did one of the drivers starting a Grand Prix on the front row (1st or 2nd place) always win the race?
 
 Objective 2: Did the driver with the most wins during a season always win the World Drivers' Championship at the end of the year (the champion is the driver with the most points)?
 
 Objective 3: Did the number of races per season increase through the years? If so, did this lead to more race wins by the Champion or to having more race winners? Who is the driver won the most World Drivers' Championships and who is the driver won the most Grands Prix? Is this the same person?
