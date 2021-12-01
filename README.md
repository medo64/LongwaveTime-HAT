[Longwave Time HAT](https://medo64.com/longwavetime-hat/)
=========================================================

This HAT is essentially a variant of [Radio time station transmitter by Henner
Zeller](https://github.com/hzeller/txtempus) made into a PCB with an onboard
antenna.

By design (and due to darn physics), signal from onboard antenna will be VERY
weak. Mind you, this is by design as the primary use case for this device is
experimentation and it's not intended to compete with the official WWVB or DCF77
signal. The onboard antenna should have enough power to work with watch on top
of it and not much further.

Of course, with an external 60 kHz (WWVB) or 75 kHz (DCF77) antenna, the signal
will propagate a bit further but you should really only consider this if your
home is not covered with the official signal.

For software, I would again point you towards [Henner Zeller's repository](https://github.com/hzeller/txtempus).

---
*You can check my blog and other projects at [www.medo64.com](https://medo64.com/electronics/).*
