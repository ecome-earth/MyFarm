# MyFarm 
MyFarm is an open-source project, made to leverage the power of IT in the world of agriculture. IT is made to provide the farmer with helpful apps that boosts productivity and level up his farming experience. 

The App is split into different Sections:

# MyInventory
a place where the farmer can keep track of his inventory records and modify it according to his activities . see the estimated value and gather insights.

# Cashflow
a place where the farmer can keep track of his expenses and income, see further financial insights that gets linked to the expert and investor dashboard. 

# MyPlan
a place where the farmer can keep track of his project milestones made by the expert. 
Provides a mechanisme for the expert to create a Project Plan with Milestones and tasks. 
and provides the farmer with an interface to see his tasks and a way to validate them. 

# Plot
a farm overview with different regions highlighted on a map. that showcase the farm assets in a geographical manner.

# Entities
Database is represented by a Document-based schema. MongoDB will be used, the definition of the data types will be as following:


# User
id UUID
firstName String
lastName String
dob Timestamp
email String
phoneNumber String
address String
role Role
metadata String

# enum Role {FARMER, EXPERT, INVESTOR, ADMIN}


# Inventory

each user can be linked to an inventory
it contains all items. By Default the database should provide most of the items used by a farmer, with possiblity to create a custom item.

id UUID
metadata String
items Item[]




# Item
id UUID
name String
description String
price Double 
imageUrl String
metadata String

