# VIC-1214-Reloaded
Reimplementation of a voice synthesizer board I built in 1981.

The voice synthsizer is a user-port peripheral based on
a circuit design from the original Radio Shack/GI
data sheet (my original design), an article in BYTE (and
for which I can't find the reference; I only have the scan),
a circuit in the Commodore 64 Interfacing Blue Book (which
had a nice test program), and the retroSpeak circuit from
jbeuckm (albeit an add-on for a Raspberry Pi, but one which
uses an external clock rather than a crystal).

The Canonical List of Commodore Products lists a VIC-1214
Speech Synthesizer cartridge, but I have not been able to
locate any information on it. Several 3rd party companies
made an expansion port cartridge synthisizer such as the
VicTalker (SSI263 chip), the Adman (SP0256), the
Chatterbox, and the PPP SpeakEasy (SSI).

This version uses a replacable TTL oscillator rather than
a crystal, using the coupling circuit from jbeuckm's design,
albeit is not tested yet.
