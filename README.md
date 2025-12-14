This app is for Coursera Working with Data course final project submission

Goal is to :
When users access the menu page of the Little Lemon app, they’ll find a full list of all items offered by the restaurant. But if a user only wants to view a specific category, rather than navigating through everything or finding a particular dish by name, they will be able to filter data with filters and also from the search bar

This was the requirement:

1.  Implement a transaction that executes a SQL statement to filter the menu by the combination of two criteria: a query string and a list of selected categories.

The query string should be matched against the menu item titles to see if it's a substring contained within.

For example, if there are four items in the database with titles: 'pizza, 'pasta', 'french fries' and 'salad', the query 'a' should return 'pizza' 'pasta' and 'salad', but not 'french fries', since the latter does not contain any 'a' substring anywhere in the sequence of characters.

The activeCategories parameter represents an array of selected categories from the filter component. All results should belong to an active category to be retrieved.

For instance, if 'pizza' and 'pasta' belong to the 'Main Dishes' category and 'french fries' and 'salad' to the 'Sides' category, a value of ['Main Dishes'] for active categories should only return 'pizza' and 'pasta'.

2.  Alter the SQL statement to support filtering by both criteria at the same time.

That means if the query string is 'a' and the active category 'Main Dishes', the SQL statement should return only 'pizza' and 'pasta'.

The 'french fries' option is excluded because it's part of a different category and 'salad' is excluded due to the same reason, even though the query 'a' is a substring of 'salad', so the combination of the two filters should be linked with the AND SQL keyword.
