auto_link.py
=============

Define the auto link policies between different waveguide type.

For example:

``(type(WG.STRIP.C.WIRE) >> type(WG.STRIP.C.WIRE), fpt.StraightPrefer(WG.STRIP.C.WIRE), fpt.BendUsing(WG.STRIP.C.WIRE.BEND_EULER))``

It means that when the start and end waveguide are both ``WG.STRIP.C.WIRE``, the automated waveguide type for routing will be ``WG.STRIP.C.WIRE`` and an automated bend ``WG.STRIP.C.WIRE.BEND_EULER`` will be added.


Users are allowed to define and set ``DEFAULT`` to their own specific linking policy.

