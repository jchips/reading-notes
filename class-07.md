# Class 7 notes

Constructors make creating objects simpler and table can be useful when sorting/organizing data in html.

## Domain Modeling

1. We need domain modeling because the model stores properties and methods that we can use repeatedly for different instances. It helps make our code more DRY.

## HTML Table Basics

1. Don't use tables for page layouts because it reduces the page accessibility, they make the code harder to write and understand when the whole layout is in a table, and tables are not automatically responsive meaning they are sized differently than semantic tags.
2.
    1. ```<th></th>``` for 'table header' fills a header row in a table.
    2. ```<tr>``` for 'table row' makes a row in the table.
    3. ```<td>``` for 'table data' fills the table rows. It's a table cell.

## Introducing Constructors

1. A constructor is a function that creates objects. It is useful when you have to make a whole bunch of objects.
2. They keyword ```this``` in objects refers to the object the particular code is inside. In a constructor, ```this``` binds properties and methods to the new object you create.

## Object Prototypes Using a Constructor

1. At my last job, Home Depot, the constructor is like a person working night staff (like me). The instances are each person. The prototypes are the tasks for example we do like stocking the shelves. Each person inherits the prototypes but we might use them differently.

## Things I want to know more about

I'm still a bit confused about what domain models are and how to define prototypes exactly.
