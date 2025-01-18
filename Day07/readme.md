### Machine learning
## How to work with data
- This stage mainly discuss how to use pandas library for machine learning purposes. 
- In Python we call this data set as Data Frames
- As Example we can put dictionary in normally like this. 
    - d={"name":["sahan","ashan","keshala"],"age":[25,27,30]}
- By using pandas we can respresent it is in a table
    - df=pd.DataFrame(d)
    -    	name	age
    -   0	sahan	25
    -   1	ashan	27
    -   2	keshala	30
- <table>
  <tr>
    <th> </th>
    <th>name</th>
     <th>age</th>
  </tr>
  <tr>
    <td>0</td>
    <td>sahan</td>
    <td>25</td>
  </tr>
  <tr>
    <td>1</td>
    <td>ashan</td>
    <td>keshala</td>
  </tr>
</table>

- When you have to get data from outside from the anaconda, you can use this path access.
    - df = pd.read_csv("file path with "\\")

- When you want to access/import the first few rows in the data set
    - df3=df.head()
- When you want to access/import the last few rows in the data set
    - df3= df.tail()

- When you have to represent it the data of column, or import the data of column in proper format, use "columns" keyword
    - kdudata.colomns
    - output: Index(['col1', 'col2', 'col3'], dtype='object')
- When you have to access/import specific column in the dataframe, direcly access the column name
    - kdudata["col1"]
    - output will be shows the that column data.
- When want to access/represent multiple columns, directly access the multiple columns inside of the [] brackets.
    - kdudata[["col1","col2"]]
    - output will be show the multiple columns.
- when want to access special element in the dataframe, use the "iloc" keyword with related location
    - kdudata.iloc[2,1] // 2,1 are the row and column of the request data
- when want to remove the data row from the data frame temperly, use "drop" keyword
    - ild.drop("a") // a is the row index of the dataframe.
    - output will be shows the dataframe instead of the index a row
 - when want to remove the multiple row
    - idl.drop(["a","b"])
- when you want to remove the row data from the dataframe in permantly, use "inplace=True" statement
    - idl.frop("a",inplace=True)
- when you have to access the columns of the data frame, additionally add the "axis=n" statement. Here n is the column number
    - idl.drop("col1",axis=1) // here col1 is the column name
- when want to generate a random data to the dataframe, use "np.random.random((5,2)),columns = ["A","B"] " statement
    - ce1= pd.DataFrame(np.random.random((5,2)),column= ["A","B"])
- when want to collab 2 dataframes together, use "concat([ce1,ce2])" function. //ce1 and c2 are the dataframes that need to collab
    pd.concat([ce1,ce2])
- when collabing 2 dataframes together, if we want to build the index in correct format, use keyword "ignore_index=True"
    - pd.concat([ce1,ce2], ignore_index=True)
- when want to collab columns together, 
    - pd.concat([ce1,ce2],axis=0)