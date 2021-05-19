#  How to Add the Current Time to a Google Spreadsheet

**Google Spreadsheets** has always been one of my favorite tools. I was an early adopter (I quickly switched to the tool shortly after Google discontinued Google Notebook) and since then I've been happy to see all the hard work and hundreds of improvements the Google Docs team have been introducing.

![enter image description here](https://i.ibb.co/fkwDqPm/image.png)

# Files


Today's post is about two really cool Google Spreadsheet functions that allow you to always display the current date and time in your spreadsheet. This will become particularly useful if you use Google Spreadsheets to monitor your tasks and deliverables, plan your work week, track your finances, etc.

## =TEXT( NOW())

=TEXT( NOW()) is a highly-customizable official Google Spreadsheet function that returns the computer system date and time in a cell.

**Important note: The function value is updated when your document "re-calculates"**  which means that, unless you make any edits to the document, you are not going to see  _the current_  date and time. However if you plan to edit your document on a regular basis (to update the task statuses, for example), this is not going to be an issue.

The awesome thing about this function is that it has plenty of available parameters that allow to format the date and time in various ways):

-   See the current day, month and year:  _=TEXT( NOW() ; "yyyy-M-d" )_  returns  _2011-2-20_
-   See the current time (with seconds):  _=TEXT( NOW() ; "HH:mm:ss" )_  returns  _13:24:56_
-   See the current day of the week (and the number of the week in a month):  _=TEXT( NOW() ; "yyyy 'week' w" )_  returns  _2011 week 8_
-   See the current time and time zone:  _=TEXT( NOW() ; "HH:mm z" )_ returns _13:24 GMT+00:00_
-   Even see the current era!  _=TEXT( NOW() ; "yyyy G GGGG" )_  returns  _2011 AD Anno Domini_


Here's an awesome spreadsheet listing all the available parameters as well as the examples of usage.
![enter image description here](https://i.ibb.co/gF2tfCG/image.png)

## =GoogleClock()

If you plan to publish the spreadsheet to the web, the above function won't work as (like I have noted above), it is only updated when you edit the current spreadsheet (i.e. type/edit/delete a value in any cell). For published and rarely updated spreadsheets there is another useful function that can turn really helpful (it is undocumented but is included in the Google Spreadsheet formula builder. This is how I actually discovered it).

![enter image description here](https://i.ibb.co/CndcFfs/image.png)

If you use the _=GoogleClock()_  function in a spreadsheet, it will automatically update live whenever you view the spreadsheet (including shared viewing). Besides, if you publish a spreadsheet as a webpage, it will automatically update every 5 minutes.

The function always returns the current date and time in the following format (unless there are any parameters I am not aware of):

> m/dd/yyyy hh:mm:ss

![enter image description here](https://i.ibb.co/x6DZTt7/image.png)

Note: Here are similar functions for Microsoft Excel (also updated live). Want more? Here's a list of  Google Spreadsheet tricks that are easy to remember

Are you aware of any other time management functions in Google Spreadsheets? Please let us know!

note: 
1. copy file: https://docs.google.com/spreadsheets/d/1O8riV7cEe_rf-QyrlqeR9qo4tmAffAwIYLYt0h7jKRU/edit?usp=sharing
2. Source: [How to Add the Current Time to a Google Spreadsheet (makeuseof.com)](https://www.makeuseof.com/tag/add-current-time-google-spreadsheet/)
3. [Understanding Date/Time Formats (arcadiadata.com)](http://docs.arcadiadata.com/4.1.0/pages/topics/display-format-ref-format-date-time.html)
