# Louisville Bike Safety Analysis

## Requirments
 - Python 3.10.2
 - Google Chrome 10

## Set up

* Run git clone https://github.com/Mariahjocorso/Louisville_Bike_Safety_Analysis to clone the repository.
* In the Louisville Bike Safety Analysis directory, run ```python3 -m venv venv``` to create the virtual environment.Activate the newly created virtual environment. 
* From the directory run the following command:
    - if using Windows PowerShell: ```source venv\Scripts\Activate.ps1```
    - if using Linux or Mac with bash/zsh: ```source venv/bin/activate```
* [Python Venv Resource Help](https://docs.python.org/3/library/venv.html)
* [windows, Linux, Mac Venv Help](https://itnext.io/a-quick-guide-on-how-to-setup-a-python-virtual-environment-windows-linux-mac-bf662c2c77d3)
* Run pip install -r requirements.txt to install the required packages.

## Features
1. Loading data. 
    - Read TWO data files (JSON, CSV, Excel, etc.)
        - I read in two CSV files. I created two separet queries on Kentucky State Police's website. I originally pulled them in as excel files and converted the data into CSV to work with. 

2. Clean and operate on the data while combining them. 
    - The heart of data science is data wrangling and cleaning, so these features test that. This is where you would need to clean the set in order to merge them. Clean your data and perform a pandas merge with your two data sets, then calculate some new values based on the new data set.  
        - Dropping columns and changing column names, Combine the sets EXPAND

3. Visualize / Present your data. 

 - Make a Tableau dashboard to display your data
        - Here is a link to my profile to see all six vizulizations I made: https://public.tableau.com/app/profile/mariah.corso

    * [Injuries 2020 to 2021](https://public.tableau.com/views/BicyclistInjuries2020to2021/Injured1?:language=en-US&:display_count=n&:origin=viz_share_link)
    * [Deaths 2020 to 2021](https://public.tableau.com/views/BicyclistDeaths2020to2021/Deaths1?:language=en-US&:display_count=n&:origin=viz_share_link)
    * [Injuries 2021 to 2022](https://public.tableau.com/views/BicyclistInjuries2021to2022/Injured2?:language=en-US&:display_count=n&:origin=viz_share_link)
    * [Deaths 2021 to 2022](https://public.tableau.com/views/BicyclistDeaths2021to2022/Deaths2?:language=en-US&:display_count=n&:origin=viz_share_link)
    * [Hit&Runs 2020 to 2021](https://public.tableau.com/views/HitandRunInvolvingBicyclist2020to2021/HitRun1?:language=en-US&:display_count=n&:origin=viz_share_link)
    * [Hit&Runs 2021 to 2022](https://public.tableau.com/views/HitandRunInvolvingBicyclists2021to2022/HitRun2?:language=en-US&:display_count=n&:origin=viz_share_link)


4. Best practices.

- Utilize a virtual environment and include instructions in your README on how the user should set one up
    - I created a virtual environment and was able to run my project through it after cloning my git hub repo. I have included instructions on how to run my project through a virtual environment. 

5. Interpretation of your data. 
   - Annotate your code with markdown cells in Jupyter Notebook, write clear code comments, and have a well-written README.md.
        - See Explanation Section

## Explanation 
 - My partner has been Biking all around Louisville lately and did a survey with his bike group about which neighborhood's they felt most and least safe. This project does not include that survey but is inspired by it. I was able to obtain bicyclist collison data from Kentucky Sate Police's website.

![KSP Query](https://github.com/Mariahjocorso/Louisville_Bike_Safety_Analysis/blob/main/KSP_Query_Example.jpg)
 
    - These are the criteria that I used to pull the data sets. Once with 11/01/2020 to 11/01/2021 and then again for the dates 11/01/2021 to 11/01/2022. 
    - The data files were downloaded as Excel files but I only needed data from the Incident tab in the data set. I converted this tab ito a CSV file for each data set and used panda to load said data sets. 
    - From the merged data sets were were able to look at the data sets in parred down from and get a total of injuires and deaths from bicylicst and motor vehical collision.
    - The most revealing data are the heat maps that I created. This shows that while the greatest amount of incidents occur Downtown the most dangerous place to bike is the (West side) of the South end. This is where the plurality of death occur. 

## Improvements
    - I would like to incorporate the survey data that inspired this project.
    - Use hit and run data within the project to go along with the heat maps I made.
    - Lay my data points over a google map so that neighboorhood bounderies were defined