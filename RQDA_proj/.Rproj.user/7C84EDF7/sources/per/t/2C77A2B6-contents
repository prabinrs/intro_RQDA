# load libraries need(install if not installed)
if(!require("RQDA")) install.packages("RQDA",dependencies = c("Depends","Imports"))
library(RQDA)

# This should open RQDA Graphical Interface. if not run following command 
RQDA()

# Code deining, Coding and major setting will be done using graphical interface (please refer to Presentation)

# Understanding RQDA to code with in build help 
help(RQDA)
help("RQDATables")
help("RQDAQuery")

# Few useful inbuild functions
filesByCodes() # files contain codes with frequency 
getCaseIds(fid) # Retrieve the number of cases and the case name 
getCaseNames(caseID) # Return the names of the IDs
getCaseIds(fid) #Return the case Name or IDs
summaryCodings() # return coding frequencies 
getCodingTable() # get details on the codes
getCodingsByOne() # serach for specific code in the data. 
codingBySearch() # finding speciific text in file and apply specific code. 

# using SQL Query 
openProject("leaders.rqda")
Reviews <- RQDAQuery("SELECT file FROM source")

#export the codes with theme
coded_text2<-RQDAQuery("SELECT coding.cid AS codeID, coding.fid AS Filecode, source.name AS filename,
                       coding.seltext AS selectText, coding.memo AS memo, freecode.name AS Theme
                       FROM coding, freecode, source 
                       WHERE coding.cid = freecode.id AND coding.fid = source.id AND coding.status=1")

write.csv(coded_text2, "coded_with_theme.csv") #write to a CSV file to share. 

