# abc2midi_shared
Modify the MIDI project by James Allwright so that it can be used as a shared library.
Only changed the converting from abc notation to midi part. Compile it like (or some else settings you want):

gcc -shared -o abc2midi.dll -lm parseabc.o store.o genmidi.o midifile.o queues.o parser2.o stresspat.o music_utils.o

after generating all the '.o' files by gcc command (or any compiler you choose).
