## ambient_intelligence_second ##

# Description #

The purpose of the Project is to avoid drivers to take the wrong fuel. When a vehicle enters the energy station cameras recognize the vehicle from its number plate. A number of the plate of the vehicle has some information about the vehicle like, size, and energy type (diesel, gasoline, electric) Depending on this information, the vehicle navigates to the proper energy slot. 

# Installing #


# Running #

You can run the program with:

reasasoner > start reasoner

# How it's works #

In the ontology, there are five main classes which are; VehicleDataBase, Service, Spots, VehicleSize, VehicleType. 

VehicleDataBase has two subclasses; RegisteredVehicles, UnregisteredVehicles. these both subclasses has their instances, these instances are the vehicles. If the vehicle is registered system applies %10 of discount to the vehicle if the vehicle is unregistered vehicle system applies the normal price. 

VehicleSize has three subclasses; Big, Medium, and Small. The vehicle considering into three possible sizes, Depending on that size the energy storage of the vehicle is determined, 

If the vehicle is diesel and a big vehicle the system considers the energy storage as 71L. This storage value multiplied by 1.917 which is the diesel price in Italy per liter and the possible price to make full the big diesel car had been calculated which is 136 Euro. This calculation is made for; diesel small, diesel medium, gasoline small, gasoline medium, gasoline big, electric small, electric medium, and electric big vehicles. When the user enters the energy station they just need to select how amount of energy they would like to purchase, %25, %50, %75, or %100. Depends on the input from the user system multiplying this information with the 136 euro (if the vehicle is big and diesel vehicle) and the system calculates the price of the energy. If the vehicle is registered to the system, the system applies a %10 discount and shows discounted and not-discounted prices. If the vehicle is not registered to the system, the system just shows the normal price. 

VehicleType has three subclasses and represents the energy type of the vehicle it would Diesel, Gasoline, or Electric. 

Service has two subclasses; Discount and WaterWindshildWiper. The purpose is to provide %10 percent discount for registered vehicles and free windshield water filling for electric vehicles. 

Spots have two subclasses; SpotState and SpotType. SpotState has information about the availability of the spots to navigate the driver to the available one to provide a time consumption. SpotType is a data base about the spots, spot numbers 1-2-3-4 are electric spots, spot numbers 5-6-7-8 are gasoline spots and spot numbers 9-10-11-12 are electric spots. By the spot type, the driver can not take the wrong fuel type to their vehicle. 







# Flow Chart #

<img width="635" alt="Screen Shot 2023-01-25 at 22 54 18" src="https://user-images.githubusercontent.com/83571132/214700418-0dc0bb39-3a97-4036-9688-9e03311a72ac.png">


