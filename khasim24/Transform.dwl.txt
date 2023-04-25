%dw 2.0
output application/json
/* In this i am going to explain about the function filter which will work on entire Array from all of the objects with in the array filter function filters and gives us the filtered results based on the condition that we have specified
*/
---
/* filter function will contain item&index item will contain the current object, index will be starting from zero in this payload i want only those items which is having "score">8 so i have used this condition */

payload filter ((item, index) -> item.score>8 )

/* In this condition i want only the web values which is not equals to null i have used this condition*/

//payload filter ((item, index) ->item.web != null )

/* in this condition i have used to print the index which is having >1 thats why i have used this condition*/

//payload filter ((item, index) ->index >1 )