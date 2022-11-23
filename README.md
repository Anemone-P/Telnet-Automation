# Telnet-Automation
Script to take a name from text, compare to CSV hashtable and output ip into a telnet connection with commands stored in a file. Further description in code comments.


# Powershell function that will connect to a modem via telnet and send the commands specified.
# Second portion will take a txt file with words in it and compare the words to a CSV file
# if any matches are found it will output the hashtable value of the word from the text file
# and then run the function, save the results, and also output results to a shell
# Originally created for connecting to RV50's but can handle any device that uses Telnet

requirements: 1. A txt file with words in it (Email.txt)
              2. A csv file with column 1 being names of routers and column 2 being their ip's (collector-lookup.csv)
              3. A txt file for outputting the results of name matching (matches.txt)
              4. A txt file for outputting the results of the telnet session (telnettest.txt)
              
File names can be whatever you want, just assign the -Path's to where you want the data
The intended purpose is to take an email body saved as a txt file and look for key words (names of modems) and then run the telnet script on any matches
This version ONLY works with a single modem match. Currently working on a multi-modem version
              
