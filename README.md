# Programming Assignment 3

## Goal: Learn to work with arrays.

For this project, I will provide you with a list of names and ID numbers, in a .txt file with the format

```
Annabelle Jeffries: 167882703
Geoffrey Jefferson: 212734569
```
This data is critical for your company, but for security purposed you can't just share the entire list with the office. You need to build a program called `DataBaseManager` which contains the list as an array of `String` types and has the following functionality:

1) Sales managers need to be able to look up ID numbers based on Customer names. So, it needs a method called `nameToID` which takes a customer's `Name` and returns both their location in the list and their `ID_number`. 
2) Customer Service repts needs to able to look up names based on ID Numbers. So, it needs a method called `IDtoName` which takes a customer's `ID_number` and returns their `Name`. 
3) The CEO wants the list in alphabetical order by `Name` but COO wants it ordered in increasing order by `ID_number` so you need two sort methods `nameSort` and `iDSort` which take the entire data base and sort it based on the desired criterion and print it with one entry per line.
4) You need methods which list only customer names (for Sales Managers), and only their ID numbers (for Customer Service Reps), so you need two methods: `getNames` and `getIDNumbers` which take the entire database as a parameter and return the array of `Names` and the array of `ID_numbers`, respectively. 

## Implementation Guidelines

- Your program should contain an array of strings called `database`. Each element of the `database` array should be a string which contains 1 line of the .txt document. You will not need to add contents to this file, so the array can be exactly as long as the number of lines of the .txt document. 
- The main method of the program creates the user experience. It should ask the user whether they are a Sales Manager, Customer Service Rep, CEO or COO. Based on their response it should list the options they can perform:

| Title | Options |
| ------| ---------|
| Sales Manager | Name to ID, get Names |
|Customer Service | ID to Name, get IDs|
|CEO | Name to ID, ID to Name, get IDs, get Names, sort by Name|
|COO | Name to ID, ID to Name, get IDs, get Names, sort by ID|

 - Good programs print welcome messages, so make sure your main method leads the user through using the program. 
 - If an ID or name is not present in the list when using `nameToID` or `iDToName`, then the program should print an error message and ask the user again what option they'd like. 

## Examples:

Suppose the database is:

```
Annabelle Jeffries: 167882703
Geoffrey Jefferson: 212734569
Julio Marquez: 156789321
Xuan Xuan: 987095612
```

Then an interaction might look like:

```
Welcome to Database manager! Are you a (1) Sales Manager, (2) Customer Service Rep, (3) CEO, or (4) COO? 2
Great! Welcome Customer Service Rep. Would you like to: 
(1) Get a customer name,
(2) get the list of all customer IDs? 2
Here you go:
167882703
212734569
156789321
987095612
```

Another example:

```
Welcome to Database manager! Are you a (1) Sales Manager, (2) Customer Service Rep, (3) CEO, or (4) COO? 3
Great! Welcome CEO. Would you like to: 
(1) Get a customer name, 
(2) Get a customer ID, 
(3) print the list of all ID numbers, 
(4) print the list of all Names,
(5) print the entire database in alphabetical order? 2
Great! Please enter the customer name: Josh Stangle
That is not a known customer. 
Would you like to: 
(1) Get a customer name, 
(2) Get a customer ID, 
(3) print the list of all ID numbers, 
(4) print the list of all Names,
(5) print the entire database in alphabetical order? 2
Great! Please enter the customer name: Geoffrey Jefferson
Their ID number is: 212734569
```

## Hint/Help
One thing you may wish to do is split your strings around the `: ` object. You can do this manually, and it isn't too hard. But, you may find the 'split' method in the String class useful. You can find it in the documentation [here](https://docs.oracle.com/javase/7/docs/api/java/lang/String.html). You can also look up the `split` method from some other resource, but please share with me any resources you use in a comment. 

## Submitting the Assignment

When you're done, you can upload your files to this Repo and commit the changes.

Click Add files at the top right of the Repo page.

There are two options:

A) Click "Add Files" to create new Java files in the repo manually. Create a new file with name `Encryptor` You can re-type or copy paste your code into those files.

B) Click "Upload Files" to just upload the `.java` files you already created. Navigate to the src folder on your computer and upload `Encryptor.java`

Once you've created the file you want, or uploaded them, navigate to the bottom of the Page and hit "Commit changes". Ensure "Commit directly to the main branch." is selected.


