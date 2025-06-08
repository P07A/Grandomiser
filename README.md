# How to play Grandomiser
Press presentation mode which is located at the third of the bottom of the left corner.

# Solution of malfunction
Some computer may not work properly at first due to the patch `spat5.conv~ @channels 2`.

In this case, please check if `spat5.conv~ @channels 2` is still in the patch. It is located on the centre of the patch, between `8. Reverb` and `Resonance`. If not, close Grandomiser and reopen. Then `spat5.conv~ @channels 2` will reappear.

If you didn't install `spat5.conv~ @channels 2`, please install it from the link (https://forum.ircam.fr/projects/detail/spat/) and run the patch again.

If you don't want to install `spat5.conv~ @channels 2` or don't want to use reverb,
1. please remove the connection between `2. MIDI Volume` and the object `thru`
2. connect left output of `2. MIDI Volume` to both inputs, Left and Right channels of `Master Gain`
3. connect left output of `2. MIDI Volume` to the object `send midiInput`. (for recording MIDI)
4. disconnect `receive~ samplePlay` and connect it to the both Left and Right channels of `Master Gain`. (Granular synthesis volume)

---------------------------------------------
Even if you installed and it doesn't sound, it could be because of the reverb for some reason. Please try to move the dial `dry/wet` slightly.
