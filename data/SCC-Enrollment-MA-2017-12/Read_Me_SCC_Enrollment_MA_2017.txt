State County Contract Enrollment Data for Medicare Advantage

The State County Contract (SCC) Enrollment Data package for Medicare Advantage (MA)
organizations is a compressed file (using SecureZIP) consisting of the following files:

Read_Me_SCC_Enrollment_MA_2017.txt - this file
SCC_Enrollment_MA_YYYY_MM.csv - data file (where YYYY = year and MM = month)

The SCC_Enrollment_MA_YYYY_MM.csv file is a comma separated value (csv) text file 
containing MA enrollment data for the month and year described in the file name.
Text values in the file are surrounded by double a quote (") so that commas that are 
part of an organization name could be included. The data type of each column is shown 
in brackets ([]) below. The file contains the following columns (these column names
are included as the first row of data):

  County - [text] - The name of the county
  State - [text] - The two letter postal code for the state
  Contract ID - [text] - The contract identifier 
  Organization Name - [text] - The name of the organization
  Organization Type - [text] - The type of contract held by the organization with CMS 
  Plan Type - [text] - The type of plan offered to beneficiaries
  SSA Code - [text] - The Social Security state/county code
  FIPS Code - [text] - The Federal Information Processing Standard state/county code
  Enrolled - [text] - Number of beneficiaries enrolled by contract in the state/county (* = 10 or less)

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

  (1) The privacy laws of HIPAA have been interpreted to prohibit publishing 
  enrollment data with values of 10 or less. Consequently some enrollment data
  in this file have been set to blank because the enrollment was 10 or less. 

  (2) The data file contains more than 65,536 rows of data. This means that Microsoft
  Excel will not be able to import all of the data for viewing. All of the data 
  can be viewed in Microsoft Access or in a statistical package, such as SAS. 
 
  (3) This data file lists enrollees by their legal state and county of residence; this is the
  county used for payment purposes. For example, an individual who moved from Baltimore to 
  Los Angeles and enrolled in XYZ Insurance company of California would be paid at the
  Baltimore rate until the change of address was recorded in the Social Security system.
  Consequently, the XYZ enrollment records will include both the California counties in its 
  approved contract service area as well as the counties throughout the United States where XYZ   
  has enrollees. 

  Please note that enrollment in these out of service area counties is very often under
  10, which leads to the suppression of the numbers.  This file does not indicate which counties
  belong to the approved contract service area of a Medicare Advantage organization and which
  counties are outside of its service area. You may refer to the Medicare Advantage county service area
  file, which is available as a separate download, to identify the approved contract service areas for
  these organizations.  

  (4) Pilot contracts are excluded from this file. The aggregate enrollment for these contracts
  is available in the Monthly Contract and Enrollment Summary Report.