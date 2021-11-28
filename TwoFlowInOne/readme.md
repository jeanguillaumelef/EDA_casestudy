# Description
You have a domain where two input streams produce into one output stream.  
This does not means it is an issue but there is things to look at.  
Do all the outputs, no matter where they come from, have the same reason to change?  
Do they scale in the same way?  

## Do all the outputs, no matter where they come from, have the same reason to change?  
If not, it means that two things which changes for different reasons are put together.  
It is usually due to a mistake in the business flow.  
Example
In a car you have the following events: decelerated, accelerated, turned.
We would want to listen to those events so we can output speed changes.

So we would do something like this:
** insert diagram of linked event directly*

The error of linking directly linking "turned" events to 


## Do they scale in the same way?
When two inputs merges scaling needs to be assessed.
