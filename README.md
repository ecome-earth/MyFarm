# MyFarm

MyFarm is an innovative open-source project designed to integrate Information Technology into the realm of agriculture, enhancing the farming experience and boosting productivity. The application is thoughtfully divided into various sections to cater to different aspects of farming.

## MyInventory

MyInventory serves as a centralized hub where farmers can meticulously manage their inventory records. It offers a seamless interface to modify records based on farming activities, provides insights into the estimated value of inventory, and facilitates efficient record-keeping.

## Cashflow

The Cashflow section empowers farmers to keep a detailed record of their expenses and income. Beyond simple tracking, this feature provides valuable financial insights that are seamlessly linked to expert and investor dashboards.

## MyPlan

MyPlan acts as a dynamic project management tool, allowing farmers to track project milestones set by experts. The system facilitates experts in creating detailed project plans with milestones and tasks, while farmers can interact with the interface to view and validate their assigned tasks.

## Plot

The Plot section offers farmers a comprehensive overview of their farm in a geographical context. Through an interactive map, different regions are highlighted to showcase farm assets, aiding in efficient farm management.

## Entities

The database is represented by a document-based schema, utilizing MongoDB. The data types and definitions are as follows:

### User

- **id**: UUID
- **firstName**: String
- **lastName**: String
- **dob**: Timestamp
- **email**: String
- **phoneNumber**: String
- **address**: String
- **role**: Role
- **metadata**: String

   #### Enum Role {FARMER, EXPERT, INVESTOR, ADMIN}

### Inventory

Each user can be linked to an inventory containing all items. The database comes pre-loaded with default farming items, but users have the flexibility to create custom items.

- **id**: UUID
- **metadata**: String
- **items**: Item[]

### Item

- **id**: UUID
- **name**: String
- **description**: String
- **price**: Double
- **imageUrl**: String
- **metadata**: String

This structured approach to MyFarm ensures a user-friendly, efficient, and adaptable platform for farmers, experts, and investors alike. The integration of MongoDB and the outlined data model guarantees a robust foundation for seamless data management within the agricultural domain.
