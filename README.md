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


### Legality of WWVB transmission ###

Transmitting on unlicensed frequencies is quite often an issue and should be
taken seriously. In USA legality of the same is coverted in [Understanding the FCC Regulations for Low-Power Non-Licensed Transmitters](https://transition.fcc.gov/Bureaus/Engineering_Technology/Documents/bulletins/oet63/oet63rev.pdf).
Short version is that you can do so as long as you keep it under 40 μV/m
measured at 300 meters. This device with its internal antenna is going to be
way under this limit.

If you plan to use it with external antenna, things get a bit trickier. I like
to use NIST's [Estimated Seasonal Signal Strength of WWVB, µV/m](https://www.nist.gov/system/files/documents/calibrations/sp432-02.pdf)
as a rule-of-the-thumb reference and as long as your watch synchronization
works only up to 10 meteres or so, you will be way under 40 µV/m as required
by FCC's rules and really unlikely to be causing any interference.

But, regardless of the rules, under no circumstances should you interfere with
official WWVB signal. This might not be encoded in rules, but it should be a
common sense.

As far as legality in other countries goes, do your own research.

---
*You can check my blog and other projects at [www.medo64.com](https://medo64.com/electronics/).*
