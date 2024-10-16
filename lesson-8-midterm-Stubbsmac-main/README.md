# CIS250_Create08_Midterm Project

You have been asked to create a database backend for a new zoo in town, Critter Country. Critter Country currently has no database system or documentation in place. Your goal is to create a set of documentation, and then use that documentation to create a database to help manage the zoo's information.

## Before Starting

1. Ensure that you have completed the practice assignment succesfully.
2. Complete the Practice Jupyter Notebook assignment.
3. Complete the Module 7 Create Assignment.
4. Watch the Miro tutorial video.

## Assignment Description

* After reviewing the provided context below, use Miro to construct an entity-relationship diagram to guide you in your table creation.
  * Review previous ERDs and our lesson on normalization to help in your creation of your ERD
* Use the provided Jupyter notebook to organize and execute scripts that will create, load, alter, retrieve, and drop the required database tables.
  * Feel free to add code/text cells to the notebook as needed.

## Assignment Requirements

* You must write all of your scripts in the Create file and check it into github.
* Export your completed ERD as a PDF and add it to your github repo
* You must script all DML and DDL operations as transactions with error handling.
* It is likely that everyone will have a different solution to the needs of this client. Because of this you will be graded on not only your results, but how well your solution adheres to the database principles we have discussed so far.
* You must use best practices in your scripts. Proper casing, spacing, and formatting are required.
* Your submitted file should show that you have ran the scripts that you are submitting.
* You must prefix your tables with cc_ (like cc_animal)

## Provided Context

### Data Points

The database will need to track the following information (at a minimum). This is not a list of tables and attributes. This is a rough list of data points that we need to ensure are covered. Read through the needs to the zoo and use this as a tool to design your solution.

* Animals
  * What is the animal
  * What is it’s name
  * How old is it
  * Where is it located
  * What does it eat
  * Who is it’s trainer
* Enclosures
  * What is the enclosure (name)
 What is the maximum and minimum temp of the enclosure (in
Fahrenheit)
  * What is the square footage of the enclosure
  * Which groundskeeper is responsible for the enclosure
* Employees
  * What is the employees name
  * What is their job category
  * What is their salary
  * Which shift are they? (day/night)

### Business Needs

The database will need to be able to handle queries that meet the following business needs:

1. When provided an enclosure ID, return which animals are located there?
2. When provided an employee ID, return which animals that employee
works with (trainers only)
3. Create a query, that when ran, will give each employee a 3% raise.
4. Create a query to delete an employee from the database when their ID
number is entered.
5. Create a query that shows all enclosure information, as well as the estimated average temperature of the enclosure (based on the min/max temperature)
   * Please research how to create and alias a calulated column using SQL SERVER syntax to get the average temperature. Do not use an aggregation.
6. Create a query that shows the average age for each type of animal (average age of all lions on one row, average age of all penguins on next row)
7. Create a query that shows the total salary cost of each job category (Critter Country wants to know how much it costs to pay all of their trainers, groundskeepers, etc..)

### Data Input

Critter County has the following data that needs added to the database. You can make up any unspecified information

* 5 trainers (make sure one of them doesn’t have any animals associated with them so that we can delete that trainer)
* 3 groundskeepers
* 1 director
* 2 food workers
* 5 enclosures (each enclosure only has one groundskeeper)
  * Waterworks
  * Sundown Sahara o Rowdy Rainforest o Polar Place
  * Windy Woods
* 3 Penguins (Polar place) (eats fish)
* 2 Lion (Sundown Sahara) (eats meat)
* 2 Parrots (Rowdy Rainforest) (eats fruit)
* 2 Bears (Windy Woods) (eats meat)
* 1 Polar Bear (Polar Place) (eats fish)
* 3 Sharks (Waterworks) (eats fish)
* 1 Snake (Rowdy Rainforest) (eats meat)
* 2 Coyotes (Windy Woods) (eats meat)
* 1 Rhino (Sahara Sundown) (eats plants)
* 2 Hippo (Waterworks) (eats plants)

## Tips

* Always include a WHERE condition when updateing and deleting data.
* Focus on developing a good ERD before you start scripting. It will make table creation go much faster!
* You do not need to put a comma between an attribute name and a datatype in a CREATE statement, just a space.
* Pay careful attention to the structure of Transaction scripts.
* If you get stuck, make a post in the Homework Help channel in Teams.
