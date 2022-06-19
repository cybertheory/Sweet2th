# Sweet2th
An API to track the location of nearby vending machines. This dataset is to be used on Apple and Google Maps. Please feel free to contribute to the dataset by using the API or Web App, email me about compensation to verify or collect data. (Under Construction)


## WEB APP


### Add, Verify and Retrieve data: 

# Docs

## Machine Object

### Attributes

UID - UUIDv4

Type:
- Coffee
- Drink
- Food+Drink
- Frozen Meals
- Premade Goods
- Drinks
- Sweets
- Ice-Cream

Payment_type = ['Card', 'Cash']

IsSmart - T or F
IsVerified - T or F
isReal - T or F
flagCount - 0

Owner=''

Brand=''

Id=""

Geolocation=""

Specific location description = ""

## API Endpoints

addMachine - constructor

endpoint:

getNearbyMachines - count, radius, location, returns count number of machine objects within a circular radius of location

endpoint:

updateMachine - uid,(new data)

endpoint:

flag - uid, flags machine as not real if flag is above 3 then machine has to be re-verified, updated. if reverified and not found the IsReal is set to false and machine is set to be deleted. 


