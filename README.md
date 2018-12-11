**ParseVissimOutput_Fzp_Rsr.py**

**2 functions _parseFzp_ and _parseRsr_ included**
###
*parseFzp(fileNames, currentDate)*

A python function for parsing PTV VISSIM vehicle trajectory outputs.
The main purpose of using this function is as follows:

1. remove the commentary content from the beginning of fzp file (VISSIM vehicle record outputs)
2. set up the header row properly
3. Add three columes: X, Y, Z coordinates for "Position" (an attribute in vehichle records)
4. save the outputs into .csv file for further aggregation or analysis

###
*parseRsr(fileNames, currentDate)*

A python function for parsing raw PTV VISSIM vehicle travel time outputs.
The main purpose of using this script is as follows:

1. remove the commentary content from the beginning of rsr file.
2. Add proper headers including the time instant each vehicle reaching the upstream and downstream boundary.
3. Save the outputs into .csv file for further aggregation or analysis
###
The main functions reads all the fzp and rsr file in the current directory.
