# CRUD Quiz

Use the solution to this afternoon's Property Tracker lab to answer the following questions. Please write your answers under each question, push the file to GitHub, and submit in the usual way.

## MVP Questions

In our Property Tracker application:

Q1. Where are we instantiating instances of the `Property` class?

Line 8 - 14 def initialize 

console.rb


Q2. Where are we defining the SQL that enables us to save the ruby `Property` object into the database?

In properties.sql file 


Q3. In `console.rb`, which lines modify the database?

Line 22(save), 33(delete)


Q4. Why do we not define the id of a `Property` object at the point we instantiate it (‘new it up’)?

The database assigns an id to the object

Q5. Where and how do we assign the id (that is generated by the database) to the ruby `Property` object?

In the first line of the initialize section (line 9)

Q6. Why do we put a guard (an `if` clause) on the `@id` attribute in the constructor?

It will only set an ID if one has not already been set

Q7. Why are some of the CRUD actions represented by instance methods, and others by class methods?

Sometimes you need to apply one action to many objects in a class. Others you only want to affect the instance you are calling it on.

Q8. What type of data structure is returned by calls to `db.exec_prepared()`? In the `save` method, how do we access the id from the returned data structure?

A pg type of array and hash. We access the id by using the square brackets

Q9. Why do we use prepared statements when performing database operations?

To protect your code from sql injection attacks

## Extension Questions

Look at the `find_by_id` and `find_by_address` methods in the `Property` class.

Q10. What do they take in as their arguments?

find_by_id takes in an integer id, and find_by_address takes in VARCHAR address

Q11. What are their return values?




