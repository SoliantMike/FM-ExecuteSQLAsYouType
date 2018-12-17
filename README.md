Search As You Type Using ExecuteSQL 
==================================

FileMaker introduced a very different kind of function with the ExecuteSQL function. First introduced in FileMaker 12, it allows you to perform “select” queries against your FileMaker data, as opposed to the more familiar “Find” functionality available in FileMaker. SQL (Structured Query Language) is a standard used with other, more traditional, database servers. Straightforward SELECTS on indexed data is blazing fast and efficient and allows for constructing relationships in SQL that do not necessarily exist in your application otherwise.  

This is all nothing new, and there have been many useful techniques that have been demonstrated since its introduction. This sample file will demonstrate yet another technique.  

<b>The Technique</b> 

In this example, we will attach a script trigger to global field that will fire on every keystroke. The script will then perform an ExecuteSQL to build a list of IDs that relate to the table we want to show results from. Once we have a list of IDs, we can enter those in a global field, where it will act as a multi-key relationship to show related records in a portal. 

View the script in the open example file to discover how to build a dynamic list of all text fields in a table, and then dynamically build an AND query to return a list of primary keys (IDs) to use in a standard FileMaker portal to display results. Sample data included for demonstration purposes.

