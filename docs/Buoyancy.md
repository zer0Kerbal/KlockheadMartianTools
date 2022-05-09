buoyancy

This module kills the parts stock buoyancy, and replaces it with custom float code.

MODULE
{

name = FSbuoyancy


buoyancyForce = 12.0 // the force applied to lift the part, scaled by depth according to buoyancyRange


buoyancyRange = 1.0 // the max depth at which the buoyancy will be scaled up. at this depth, the force applied is equal to buyoancyForce. At 0 depth, the force is 0


buoyancyVerticalOffset = 0.1 // how high the part rides on the water in meters. Not a position offset inside the part. This will be applied in the global axis regardless of part rotation. Think iceberg/styrofoam.
        // for subs you could play with that value to make it think you are at sea level buoyancywisse at an entirely different depth. You could even change this value at run time to create the whole up/down code (Using your own code I mean)


maxVerticalSpeed = 0.2 // the max speed vertical speed at which there will be a liftng force applied. Reduces bobbing.


dragInWater = 1.5 // when in water, apply drag to slow the craft down. Stock drag is 3.


debugMode = True // enables buoyancy control context menus

waterImpactTolerance = 125 // For sea planes, any part in the water during take off should have a resistance high enough to withstand take off speeds.


//forcePointName = // you can set an alternate transform name to set up multi point float. Optional


splashFXEnabled = True // on by default, creates splashes even deep under water currently...


}
