# `universalis`

Universal simulation model abstracting most important human systems' dynamics.

This model should, if properly adapted and given good enough starting data,
yield believable results no matter the historical era. It is however
first-and-foremost meant for representing contemporary systems.


## Key systems

**humans**: perhaps the most tricky part is modeling human behavior. This
can only be done to a limited extent. It's still crucial though to include
individual human agents, and track both their mental and physical state.

**organizations**: over time humans create institutions that help facilitate
achieving of common goals. Organizations can be thought of as being separate
from their individual members in many ways and should be modelled as such.

**infrastructure**: human-built structures and systems represented in
sufficient detail. Infrastructure is everything from buildings and roads to
global supply chains and the internet. 

**nature**: the natural world is represented both in the macro and the micro
scale. There's both a global circulation model component and individual
populations of different animal and plant species.


## Varying resolution

Most sub-models provide multiple high-level tweaks and settings, including
the ability to scale up or down resolution of some parts of the model. For
example the population generation process can be scaled down to create fewer
deeply simulated humans in order to raise overall simulation speed.


## General considerations

As with any modeling exercise, finding good abstractions is both very important
and possibly damning.

With the `universalis` model we try to deliver exciting results by finding the
right abstractions, but we also are wary of the limitations of any pre-defined
model. That's why this model is also built as self-extending, meaning there's
possibility for simulation agents to craft their own abstractions and impose
those on the world.


## Physical context

The Earth is represented as a collection of 2D equirectangular grids of varying
resolution.

Physical entities represent their location using a simplified coordinates
system placing them on the world grid.

Changes to things like earth crust, albedo, forests, etc. are recorded on the
relevant grids and can feed back into other systems.



