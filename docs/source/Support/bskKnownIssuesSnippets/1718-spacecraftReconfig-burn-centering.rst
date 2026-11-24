- In Basilisk ``2.12.2`` and earlier, :ref:`spacecraftReconfig` truncated the per-thruster half-burn time
  ``thrustOnTime / (2 * numThrusters)`` to whole seconds when deciding when to start a burn, while the burn end
  used the exact value. Each burn could start up to about one second late and was not centered on the
  impulsive burn time (#1718). This is fixed in the current release.
