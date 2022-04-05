# What is LINQ ?

---

***(Language Integrated Query) is uniform query syntax in C# to retrieve data from different sources and formats . It is integrated in C# , thereby eliminating the mismatch between programming languages and databases , as well as providing a single querying interface for different types of data sources .***


***For a developer who writes queries , the most visible "language-integrated" part of LINQ is the query expression. Query expressions are written in a declarative query syntax. By using query syntax, you can perform filtering, ordering, and grouping operations on data sources with a minimum of code. You use the same basic query expression patterns to query and transform data in SQL databases, ADO.NET Datasets, XML documents and streams, and .NET collections.***


***LINQ queries return results as objects. It enables you to uses object-oriented approach on the result set and not to worry about transforming different formats of results into objects.***


![IMG]https://www.tutorialsteacher.com/Content/images/linq/linq-usage.PNG)

![IMG](https://www.tutorialsteacher.com/Content/images/linq/linq-execution.PNG)


**example shows the complete query operation :**

```
// Specify the data source.
int[] scores = { 97, 92, 81, 60 };

// Define the query expression.
IEnumerable<int> scoreQuery =
    from score in scores
    where score > 80
    select score;

// Execute the query.
foreach (int i in scoreQuery)
{
    Console.Write(i + " ");
}

// Output: 97 92 81

```

---

## What is Query ?

---

***An expression that retrieves data from a data source. Queries are usually expressed in a specialized query language. Different languages have been developed over time for the various types of data sources, for example SQL for relational databases and XQuery for XML.***

---

### Three Parts of a Query Operation :

---

1. **Obtain the data source.**

2. **Create the query.**

3. **Execute the query.**


***Data Sources :***

```
// Create a data source from an XML document.
// using System.Xml.Linq;
XElement contacts = XElement.Load(@"c:\myContactList.xml");

```

---

#### Basic LINQ Query Operations :

- **Obtaining a Data Source**

```
//queryAllCustomers is an IEnumerable<Customer>
var queryAllCustomers = from cust in customers
                        select cust;
```

- **Filtering**

```
var queryLondonCustomers = from cust in customers
                           where cust.City == "London"
                           select cust;
```

- **Ordering**

```
var queryLondonCustomers3 =
    from cust in customers
    where cust.City == "London"
    orderby cust.Name ascending
    select cust;
```

- **Grouping**

```
// queryCustomersByCity is an IEnumerable<IGrouping<string, Customer>>
  var queryCustomersByCity =
      from cust in customers
      group cust by cust.City;

  // customerGroup is an IGrouping<string, Customer>
  foreach (var customerGroup in queryCustomersByCity)
  {
      Console.WriteLine(customerGroup.Key);
      foreach (Customer customer in customerGroup)
      {
          Console.WriteLine("    {0}", customer.Name);
      }
  }
```

- **Joining**

```
var innerJoinQuery =
    from cust in customers
    join dist in distributors on cust.City equals dist.City
    select new { CustomerName = cust.Name, DistributorName = dist.Name };
```

- **Selecting**



