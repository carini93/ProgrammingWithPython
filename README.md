# ProgrammingWithPython
 

  
## 1.1  Description of the Task 
You  get  (A)  4  training  datasets  and  (B)  one  test  dataset,  as  well  as  (C)  datasets  for  50  ideal  functions.  All  data 
respectively consists of x-y-pairs of values.   

 Your  task  is  to  write  a  Python-program  that  uses  training  data  to  choose  the  four  ideal  functions  which  are  the 
best fit out of the fifty provided (C). 
i) Afterwards, the program  must use the test data  provided (B) to   determine for each and every x-y-
pair  of  values  whether  or  not  they  can  be  assigned  to  the  four  chosen  ideal  functions;  if  so,  the 
program also needs to execute the mapping and save it together with the deviation at hand 
ii) All data must be visualized logically 
iii) Where possible, create/ compile suitable unit-test.
 
The criterion for choosing the ideal functions for the training function is how they minimize the sum of all y-
deviations  squared (Least-Square). 
The criterion for mapping the individual test case to the four ideal functions is that the existing maximum 
deviation of the calculated regression does not exceed the largest deviation between training dataset (A) and 
the ideal function (C) chosen for it by more than  factor  sqrt(2).
 
In order to give proof of your skills in Python related to this course, you need to adhere to certain criteria when 
solving the exercise; these criteria are subsequently described under ‘Details.’ 
 
 
## 1.2  Details 
You are given four training datasets in the form of csv-files.  Your Python program needs to be able to 
independently compile a SQLite database (file) ideally via sqlalchemy and load the training data into a single five-
column spreadsheet / table in the file. Its first column depicts the x-values of all functions.  Table 1, at the end of 
this subsection, shows you which structure your table is expected to have.  The fifty ideal functions, which are also 
provided  via  a  CSV-file,  must  be  loaded  into  another  table.  Likewise,  the  first  column  depicts  the  x-values, 
meaning  there  will  be  51  columns  overall.  Table  2,  at  end  of  this  subsection,  schematically  describes  what 
structure is expected. 
After  the  training  data  and  the  ideal  functions  have  been  loaded  into  the  database,  the  test  data  (B)  must  be 
loaded line-by-line from another CSV-file and – if it complies with the compiling criterion – matched to one of the 
four  functions  chosen  under  i  (subsection  above).  Afterwards,  the  results  need  to  be  saved  into  another  four-
column-table in the SQLite database. In accordance with table 3 at end of this subsection, this table contains four 
columns with x- and y-values as well as the corresponding chosen ideal function and the related deviation.     
Finally, the training data, the test data, the chosen ideal functions as well as the corresponding / assigned datasets 
are visualized under an appropriately chosen representation of the deviation.   
 
Please create a Python-program which also fulfills the following criteria:  
− Its design is sensibly object-oriented  
− It includes at least one inheritance  
− It includes standard- und user-defined exception handlings  
− For logical reasons, it makes use of Pandas’ packages as well as data visualization via Bokeh, sqlalchemy, 
as well as others 
− Write unit-tests for all useful elements 
− Your  code  needs  to  be  documented  in  its  entirety  and  also  include  Documentation  Strings,  known  as 
”docstrings“ 

[Code](https://github.com/carini93/ProgrammingWithPython/blob/master/ProgrammingWithPython.ipynb) : at this link you can find the python code created to solve the task.
