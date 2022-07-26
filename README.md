# Programming Assignment 3

## Goal: Learn to work with arrays.

For this project, I will provide you with a list of names and ID numbers, in a .csv file with the format

```
Annabelle Jeffries: 167882703
Geoffrey Jefferson: 212734569
```
This data is critical for your company, but for security purposed you can't just share the entire list with the office. You need to build a program called `DataBaseManager` which contains the list as an array of `String` types and has the following functionality:

1) Sales managers need to be able to look up ID numbers based on Customer names. So, it needs a method called `nameToID` which takes a customer's `Name` and returns both their location in the list and their `ID_number`. 
2) Customer Service repts needs to able to look up names based on ID Numbers. So, it needs a method called `IDtoName` which takes a customer's `ID_number` and returns their `Name`. 
3) Your manager wants the list in alphabetical order by `Name` but their boss wants it ordered in increasing order by `ID_number` so you need two sort methods `nameSort` and `iDSort` which take the entire data base and sort it based on the desired criterion.
4) You need methods which list only customer names, and only their ID numbers, so you need two methods: `getNames` and `getIDNumbers` which take the entire database as a parameter and return the array of `Names` and the array of `ID_numbers`, respectively. 


## Submitting the Assignment

When you're done, you can upload your files to this Repo and commit the changes.

Click Add files at the top right of the Repo page.

There are two options:

A) Click "Add Files" to create new Java files in the repo manually. Create a new file with name `Encryptor` You can re-type or copy paste your code into those files.

B) Click "Upload Files" to just upload the `.java` files you already created. Navigate to the src folder on your computer and upload `Encryptor.java`

Once you've created the file you want, or uploaded them, navigate to the bottom of the Page and hit "Commit changes". Ensure "Commit directly to the main branch." is selected.


