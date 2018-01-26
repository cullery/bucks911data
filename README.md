# bucks911data
911 data for Bucks County Pennsylvania provided by the county's emergency communications department in 2017.
The raw data original text files are in the Records folder, one for ambulance calls and one for police calls in their respective folders. 
I've included the csv files for both so you'll see what it should look like once its finished.
Here's how the script works:
Open the folder labeled "Dispatch Records" where you'll see another dispatch records folder.
Open this second folder to find the parse.py file, .DS_Store file, incidents folder and a results folder.
Copy the raw text files (you can do ambulance and police together or one at a time) and copy them into the incidents folder.
Open your Python shell and run the parse.py file. 
A CSV file for each text file will appear in the results folder. 
Due to an error I haven't worked out, the csv will add a blank line between each call. 
I've found the easiest way to solve this is to open a jupyter notebook. 

import pandas as pd
df=pd.read_csv("911 data file path")
df.to_csv("destination)

Once you open your spreadsheet, the blank spaces should be removed and you're good to go. 
When you read the file in pandas, I believe every column is read as a string. There's a way to fix it, but I'm not totally sure how yet.
I recommend reviewing the script, playing around with it, and file your own right to know with your local equivalent authorities and see what you can do. 

