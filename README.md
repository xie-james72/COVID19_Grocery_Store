# COVID19_Grocery_Store
This is just me writing down an idea before i forget. If someone makes it, let me know and I am more than 1000% down to help.

User: Optimizer app which takes in a grocery list and a store layout that optimizes your list to spend the least amount of time in the store
Store: Use customer data to observe purchasing trends to modify aisle-end and front displays to minimize customer interactions

Methodolody:
- Create an ideal customer, then layer on non-ideal behaviour and generate an ensemble model of customer movement

Data collection:
- Grid off a store and assign items a general location
- Generate obstacles to represent the aisles/displays
- Get a bunch of receipts and use those to create different customers

Assumptions to create the ideal condition:
1. Customers will follow an ordered list that is generated a priori to minimize total distance to complete a circuit
2. Customers will follow rules such as single-direction aisles
3. Customers will not impulse buy or purchase items not on their list
4. Customers know exactly where the items are
5. Shelf supplies are infinite
6. There are no other customers in the store

Relaxed Assumptions:
1. List ordering may not be ideal (slowly randomize list)
2. Customers may not follow rules if there is a shorter path
3. Customers may "wander"
4. Customers may search nearby an item. We will ignore the case of "completely unsure where something is"
5. Shelf supplies dwindle over time
  This last one is most critical for modelling aisle end displays which have less stock

Outputs:
- Distance distribution in a store that a customer traverses under ideal and non-ideal conditions
- Distance distributions due to physical rearrangements of items or placement of displays


https://link.springer.com/chapter/10.1007/978-3-642-15393-8_31
https://repository.upenn.edu/cgi/viewcontent.cgi?article=1593&context=statistics_papers
http://link.springer.com/article/10.1007/s10844-009-0113-8
