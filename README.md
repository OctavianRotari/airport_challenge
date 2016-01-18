Airport Challenge
=================

Instructions
```
As an air traffic controller
So planes can land safely at my airport
I would like to instruct a plane to land

As an air traffic controller
So planes can take off safely from my airport
I would like to instruct a plane to take off

As an air traffic controller
So that I can avoid collisions
I want to prevent airplanes landing when my airport if full

As an air traffic controller
So that I can avoid accidents
I want to prevent airplanes landing or taking off when the weather is stormy

As an air traffic controller
So that I can ensure safe take off procedures
I want planes only to take off from the airport they are at

As the system designer
So that the software can be used for many different airports
I would like a default airport capacity that can be overridden as appropriate

As an air traffic controller
So the system is consistent and correctly reports plane status and location
I want to ensure a flying plane cannot take off and cannot be in an airport

As an air traffic controller
So the system is consistent and correctly reports plane status and location
I want to ensure a plane that is not flying cannot land and must be in an airport

As an air traffic controller
So the system is consistent and correctly reports plane status and location
I want to ensure a plane that has taken off from an airport is no longer in that airport
```

Solution

I solved this challenge creating 3 classes:

Airport
Plane
Weather
Airport class


initialize(put a number if the capacity is different than default) when you create an instance of airport you can specify a capacity otherwise it will be set to the constant DEFAULT_CAPACITY.

planes it returns the array of planes stored in the airport. 

land(plane) it instructs a plane to land at the airport if the airport is not full, the plane is flying, the weather is not stormy.

take_off(plane) it instructs a plane to take off from the airport if the plane is at the airport and the weather is not stormy. 
Plane class

stormy? it returns true 33% of times, false otherwise. It has been implemented with the Kernel method rand.
