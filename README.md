# Hadoop MapReduce Example
A simple MapReduce example for Hadoop using Python. This example is based on an Udacity course: Intro to Hadoop and MapReduce.<br>


Hadoop MapReduce is a programming model and processing engine designed for distributed processing of large datasets across clusters of computers.
It is a key component of the Apache Hadoop framework, which facilitates the storage and processing of vast amounts of data. <br>


MapReduce operates by breaking down tasks into two main phases: 
> The **"Map"** phase, where data is divided into smaller chunks and processed in parallel across multiple nodes, <br>
> and the **"Reduce"** phase, where the results from the Map phase are aggregated to produce the final output. <br>

This approach allows for efficient parallelization of computations, making it well-suited for handling massive datasets that would be impractical to process on a single machine. Hadoop MapReduce is widely used in the field of big data analytics and is known for its scalability and fault tolerance, making it a fundamental tool in the realm of distributed computing.




## Sample data

```
2012-01-01	09:00	San Jose	Men's Clothing	214.05	Amex
2012-01-01	09:00	Fort Worth	Women's Clothing	153.57	Visa
2012-01-01	09:00	San Diego	Music	66.08	Cash
2012-01-01	09:00	Pittsburgh	Pet Supplies	493.51	Discover
2012-01-01	09:00	Omaha	Children's Clothing	235.63	MasterCard
2012-01-01	09:00	Stockton	Men's Clothing	247.18	MasterCard
2012-01-01	09:00	Austin	Cameras	379.6	Visa
2012-01-01	09:00	New York	Consumer Electronics	296.8	Cash
2012-01-01	09:00	Corpus Christi	Toys	25.38	Discover
2012-01-01	09:00	Fort Worth	Toys	213.88	Visa
```

## Mapper
In the "Map" phase of Hadoop MapReduce, the input data is split into smaller parts, and each mapper independently processes a portion. A user-defined "map function" is applied to each piece of data, creating intermediate key-value pairs.

```
Men's Clothing	214.05
Women's Clothing	153.57
Music	66.08
Pet Supplies	493.51
Children's Clothing	235.63
Men's Clothing	247.18
Cameras	379.6
Consumer Electronics	296.8
Toys	25.38
Toys	213.88
```

## Reducer


