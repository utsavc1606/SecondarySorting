# SecondarySorting
Secondary sort in Mapreduce  With mapreduce framework, the keys are sorted but the values associated with each key  are not.  In order for the values to be sorted, we need to write code to perform what is  referred to a secondary sort. The input to the program is a bunch of employee attributes. The output required is department number (deptNo) in ascending order, and the employee last name,  first name and employee ID in descending order.  The recipe to get the effect of sorting by value is: 1) Make the key a composite of the natural key (deptNo) and the natural value (lName, fName and empNo).  2) The sort comparator should order by the composite key, that is, the natural key and natural  value. 3) The partitioner and grouping comparator for the composite key should consider only the natural key for partitioning and grouping.
