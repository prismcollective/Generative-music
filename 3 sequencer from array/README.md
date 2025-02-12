This project is a sequencer that takes notes from an array. It converts midi-style notes into frequencies with the expr object  (`pow(2, $f1/12)*440`)

It has a sine+noise+saw mix oscillator with a pluck-like envelope. There is also a delay. The bass is a supersaw. The hand movements control the band pass (`bp~`) filter on the bass, the mix of the saw in the melody, and the bass note.
