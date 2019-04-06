State County Penetration Data for Medicare Advantage

The State County Penetration Data package for Medicare Advantage (MA)
organizations is a compressed file (using SecureZIP) consisting of the following files:

Read_Me_SC_Penetration_MA.txt - this file
State_County_Penetration_MA_YYYY_MM.csv - data file (where YYYY = year and MM = month)

The State_County_Penetration_MA_YYYY_MM.csv file is a comma separated value (csv) text file 
containing county level eligible and MA enrollment data for the month and year described in 
the file name. Text values in the file are surrounded by double a quote (") so that commas 
that are part of an organization name could be included. The data type of each column is 
shown in brackets ([]) below. The file contains the following columns (these column names
are included as the first row of data):

  State Name - [text] - The name of the state
  County Name - [text] - The name of the county
  FIPSST - [text] - The Federal Information Processing Standard state code
  FIPSSNTY - [text] - The Federal Information Processing Standard county code
  FIPS - [text] - Concatinated Federal Information Processing Standard state/county code
  SSAST - [text] - The Social Security state code
  SSACNTY - [text] - The Social Security county code
  SSA - [text] - Concatinated Social Security state/county code
  Eligibles - [numeric] - The number of Medicare eligibles in the county
  Enrolled - [text] - The number of PDP enrollees in the county (* = 10 or less)
  Penetration - [numeric] - Derived field that equals the ratio of enrollees over eligibles 
     multiplied by 100
 

This file contains data for the following organization types (where there are active contracts): 

  Local CCP
  Regional CCP
  MSA 
  PFFS 
  Demonstrations 
  National PACE 
  1876 Cost 
  HCPP - 1833 Cost
  Employer Direct PFFS

Special Notes:

  (1) The eligible data contains some records that have not yet been associated with a 
  specific state and county or a county within a state. These records have been included
  within the data file with a State Name notation of "Pending State Designation" and County
  Name of "Pending County Designation".

  (2) The privacy laws of HIPAA have been interpreted to prohibit publishing 
  enrollment data with values of 10 or less. Consequently some enrollment data
  in this file has been set to an asterisk (*) because the enrollment was 10 or less.  
  The enrollment for each of these rows has been aggregated to the state level and is 
  presented in the "Pending County Designation" row for that state. 

  Data users may redistribute the average number of enrollees deleted among the cells 
  containing asterisks. For example, if a state had an enrollment count of 50 shown
  in the Pending County Designation row and had 25 cells containing asterisks, then a user 
  could assume that each asterisk cell had 2 enrollees. This average, while not 100% accurate, 
  is useful and can help with trend analysis. 

  (3) The penetration data is derived by dividing the number of enrollees by the number of 
  eligibles and multiplying the result by 100. This calculation has not be done in records
  where there the enrollment data has been suppressed because the enrollment was 10 or less.
  It has also not been performed on records where the elibibles were pending state or county 
  designation since any enrollment presented there was aggregated from other rows.

  (4) This data file lists enrollees by their legal state and county of residence; this is the
  county used for payment purposes by Medicare. For example, an individual who moved from Baltimore to 
  Los Angeles and enrolled in XYZ Health Plan of California would be paid at the
  Baltimore rate until the change of address was recorded in the Social Security system.
  Consequently, the XYZ enrollment records will include both the California counties in its 
  approved contract service area as well as the counties throughout the United States where XYZ   
  has enrollees. 

  (5) Pilot contracts are excluded from this file. The aggregate enrollment for these contracts
  is available in the Monthly Contract and Enrollment Summary Report.