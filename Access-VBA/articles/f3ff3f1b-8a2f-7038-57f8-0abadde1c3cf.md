
# Circular reference caused by <query reference>. (Error 3102)

You tried to execute a query that depends on itself for data. For example, this error occurs if you execute either of the following queries:

Query1



```
SELECT * FROM Employees, Query2;

```

Query2



```
SELECT * FROM Query1;


```

Redesign the queries to eliminate the dependency.
 **ACCESS SUPPORT RESOURCES**[Access for developers forum on MSDN](https://social.msdn.microsoft.com/Forums/office/en-US/home?forum=accessdev)[Access help on support.office.com](https://support.office.com/search/results?query=Access)[Access help on answers.microsoft.com](http://answers.microsoft.com/en-us/office/forum/access?page=1&amp;tab=question&amp;status=all&amp;auth=1)[Search for specific Access error codes on Bing](http://www.bing.com/)[Access forums on UtterAccess](http://www.utteraccess.com/forum/index.php?act=idx)[Access wiki on UtterAcess](http://www.utteraccess.com/forum/index.php?act=idx)[Access developer and VBA programming help center (FMS)](http://www.fmsinc.com/MicrosoftAccess/developer/)[Access posts on StackOverflow](http://stackoverflow.com/questions/tagged/ms-access)
