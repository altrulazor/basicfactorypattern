# basicfactorypattern
Playing around with basic factory pattern

###### The Factory Pattern
- The capability to choose classes at runtime

###### Basic principle
(1) public abstract class AbstractClass () { }

(2) public class ImplementationClass extends AbstractClass() { }

###### Implementation
<client>  ->  <factory> ShipFactory  ->  <abstract> Ship
- Ship *is parent, implements all basic attributes and behavior *
- UfoShip extends Ship
- MotorboatShip extends Ship
- SailingShip extends Ship

Client now accesses ShipFactory, ShipFactory returns a Ship.
Which ship (implementation) will get returned, is at this time undefined.
It can be randomly or programatically chosen during runtime.
This works, because all ships extend the base class "Ship" and thus fullfill all requirements set by Ship.

This is called abstraction.
When you just work with any kind of ship and don't need the specifcs: if you're sailing or motorboating.



Java 8

Created by Rainer Knabenbauer
