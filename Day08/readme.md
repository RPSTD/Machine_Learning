### Machine Learning
## Python learning section

- When have to each value count of the age section, 
    - pd.value_counts(df["age"])

- when you want to get the list of the related column values or row values, use "list" function
    - list(df2.columns)
    - list(df2.index)

- when you want to reorder the values of the chart, use reindex() function.
    - df2.reindex([3,2,0,1])

- when you want to change the columns, 
    - df2.reindex(columns=["intake","name","age"])

- when you want to change the columns name, use it like this.
    - df2.columns=["intake no","fname","age value"]

### Use of mathplotlib library

- The representation of graph by using mathplotlib library
    - plt.plot(L1,L2)
    - plt.show()

- create a charts with labeled axis and columns
    - plt.figure(figsize=(10,4))
    - plt.plot(L1,L2)
    - plt.xlabel("Month")
    - plt.ylabel("Price")
    - plt.title("Price agains the months")
    - plt.show()

- Scatterplot representation
    - plt.scatter(data["Work.Exp"],data["Credit.Score"])
    - plt.xlabel("Work Experience")
    - plt.ylabel("Credit Score")
    - plt.title("Credit Score againts the work Experiance")

- Heatmap representation
    - import seaborn as sns
    - sns.heatmap(data2Frame, annot=True)
    - plt.show()