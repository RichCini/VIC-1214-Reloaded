# VIC-1214-Reloaded
Reimplementation of a voice synthesizer board I built in 1981.

The voice synthsizer is a user-port peripheral based on
a circuit design from the original Radio Shack/GI
data sheet (my original design), an article in BYTE (and
for which I can't find the reference; I only have the scan),
and a circuit in the Commodore 64 Interfacing Blue Book (which
had a nice test program). There is a project called retroSpeak
from jbeuckm (albeit an add-on for a Raspberry Pi) that uses an
external programmable clock rather than a crystal.

The Canonical List of Commodore Products lists a VIC-1214
Speech Synthesizer cartridge, but I have not been able to
locate any information on it. Several 3rd party companies
made an expansion port cartridge synthisizer such as the
VicTalker (SSI263 chip), the Adman (SP0256), the
Chatterbox, and the PPP SpeakEasy (SSI).

I tried a using a replacable TTL oscillator rather than
a crystal with the coupling circuit from jbeuckm's design,
but it didn't work. I suspect that the signal phase is
wrong, but until I test it with my Silgent waveform
generator, I won't know. I think it needs an inverted
clock in order to work. So, the existing design uses
the tried-and-true crystal for now. Changing the crystal
frequency will change the pitch of the voice, so even a
colorburst crystal (3.59MHz) will work.

I had a few sample boards made and it works flawlessly with
the LM386 amplifier. Glad to see it worked the first time!
