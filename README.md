# pdkvabs - released under gpl v3.0
vanilla abstractions

(before use, put subfolder contents besides the util folder into main pdkvabs folder)

(also note that this is for personal use and VERY subject to change/renaming so I suggest this repo mainly for educational use)

## GENERAL
- dkattqpt - record attack locations in a soundfile
- dkautowah~ - automatic wah based on envelope following
- dkbangroute - route bangs with bangs
- dkbangsync - bang syncer
- dkbitred~ - audio-signal bit-reduction based off 3.Bit-Reduction by Alexander Torres Porres.
- dkbitcrush~ - bit-resolution/sample-rate reducer
- dkblkmn~ - generates blackman window according to input from 0 to 1.
- dkchangebang~ - bang when detecting changes in a signal
- dkcliktrak~ - click track/metronome
- dkdistort~ - distortion waveshaper
- dkdownsamp~ - audio-signal downsampler.
- dkfbdel~ - simple delay with fb
- dkfbvdel~ - simple delay with fb (signal delay time)
- dkfft/fftbinwipe~ - fft bin wiper ported from SuperCollider's PV_BinWipe
- dkfft/fftcomp~ - spectral compressor based on 5.Spectral-Compressor by Alexander Torres Porres.
- dkfft/fftconvolve~ - fft convolver
- dkfft/fftcross~ - spectral cross-synthesis based on 1.Cross-Synthesis by Alexander Torres Porres.
- dkfft/fftgain~ - spectral filter with traceable gain. 
- dkfft/fftgate~ - spectral gate (requires zexy). 
- dkfor - for loop
- dkfreqshift~ - frequency shifter via single sideband modulation
- dkgainenv~ - traceable gain envelope
- dkincwr~ - incremental tabwriter
- dkint~ - "typecast" signals to integer
- dkincwritepos~ - incremental tabwrite~ with sample position table
- dkkarplus~ - karplus-strong synth
- dkkeysend - send globally via prefixed key
- dkkeytonum - maps keys to numbers sequentially by row
- dkloopplay~ - synced looper based around tabplay~
- dkloopwin~ - signal-driven loop windowing
- dkmbang - multiple banger
- dkmbang_r - multiple banger (but randomly gated)
- dkmidirt - abstraction to handle midi real-time messages
- dknobu~ - sample chopper abstraction
- dknot - control-rate bitwise not
- dknotetomidi - note names (case-insensitive) to midi notes
- dkoneShotM - a one-shot sample player, left inlet takes a bang to trigger playback, right inlet takes a path for file. 
- dkoneShotS - stereo version 
- dkpaulstretch~ - slightly modified/cleaned up martin brinkmann's (mmb) small_paul1 paulstretcher for use as an abstraction. Unlike small_paul1, it rounds window sizes to the nearest power of 2 and accept signals as position input.
- dkpshift~ - rotating tape head pitchshifter
- dkphasevoc~ - a phase vocoder abstraction lifted from Miller Puckette's I07.phase.vocoder from the help files. Like tabread4~, hot signal inlet indexes by sample. First arg is array name, second is window size.
- dkphsrd~ - phasor sound reader abstraction
- dkpolargraph~ - graph a real fft analysis in polar coords
- dkpolyish1 - polyish abs with no note off
- dkpulsewidth~ - pulse width modulation
- dkroute2~ - one to two signal router
- dkscaledeg_van - borrowed from SuperCollider's Scale object. Maps scale degrees to midi notes. Arguments are scale and starting midi note. Vanilla version of my scaledeg external using tables
- dkselector - a row of 32 toggle boxes whose values are stored in an array (name passed by argument, requires cyclone) 
- dkseqgen1 - timed random sequence generator
- dksisascl~ - SIne SAmple SCaLer
- dksamptoms - samples to ms
- dksndchop~ - sound chopper
- dksndchopgrn~ - granular sound chopper
- dksndtrig~ - triggered sound player
- dksndtriggrn~ - triggered granular sound player
- dkspigot~ - control-rate spigot for audio signals
- dkspigot2~ - audio-rate spigot for audio signals
- dkstrippoly - a poly without noteoff messages (or zero velocity notes) 
- dkstutter~ - a delay-based stutter effect
- dkswitch2~ - choose between 2 different signal inputs
- dksyncloop - a synchronized looper. 
- dkswing - bang swinger
- dksyncb - synchronized banger
- dksyncf - synchronized floats
- dktport - a fancy counter with beats, subdivisions, and measures. 
- dktrigrd~ - triggered array reader
- dkoutput~ - output abstraction
- dkvancomp~ - vanilla compressor/limiter
- dkvandrk - vanilla drunk random number generator 
- dkvanphs~ - vanilla 3-delay line phaser/chorus effect 
- dkvgcld~ - vanille grain cloud
- dkvisclock - visual clock
- dkvmetrox - vanilla metro divider
- dkvmetrox - receiver for dkvemtrox
- dkvuzi - vanilla uzi/multiple banger
- dkvadsr~ - adsr envelope generator using vline~ based off Matt Davey's  diy-adsr~
- dkxor - control-rate bitwise xor

## COUNTER
- dktimedctr- on bang, output floats counting up to x 
- dkvanctr - vanilla counter (can go both up and down)

## DELAY-BASED
- dkchorus~ - chorus
- dkflanger~ - flanger
- dkphaser~ - phaser

## GATE
- dklegate - let through floats lesser or equal to x
- dkgegate - let through floats greater or equal to x
- dkrgate - let through anything x% of the time
- dknzgate - only let nonzero floats through

## GRANULAR
- dktrgrnstr~ - live granular stretcher (uses dksyncgrn~)
- dkxgrn~ -  granular stretcher
- dkloopgrn~ - granular synchronized looper based on dksyncgrn~

## FFT
- dkfftgate~ - spectral gating (above or below)
- dkfftconvolve~ - spectral non-partitioned convolution
- dkfftcross~ - spectral cross-synthesis
- dkfftdelay~ - spectral delay
- dkfftfilt~ - spectral filtering
- dkhannnorm~ - normalization for hann windowing (and overlapping) in an fft transform
- dkvanpaul~ - vanilla paulstretcher
- dkvanpvoc~ - vanilla phase vocoder

## FILTERS
- dkvap1o~ - first-order allpass filter (control inlet for cutoff)
- dkvap1os~ - first-order allpass filter (signal inlet for cutoff)
- dkvap1os~ - second-order allpass filter (control inlets for cutoff and q)
- dkvhp1o~ - first-order highpass filter (control inlet for cutoff)
- dkvhp1os~ - first-order highpass filter (signal inlet for cutoff)
- dkvlp1o~ - first-order lowpass filter (control inlet for cutoff)
- dkvlp1os~ - first-order lowpass filter (signal inlet for cutoff)
- dkvbp2o~ - second-order bandpass filter (control inlets for cutoff and q)
- dkvbr2o~ - second-order bandreject filter (control inlets for cutoff and q)
- dkvapcomb~ - allpass filter from two combs
- dkvfbcomb~ - feedback comb filter

## MARKOV
- dkvmarkov1o - vanilla first-order markov analysis/generator
- dkvmarkov2o - vanilla second-order markov analysis/generator

## MATH (AUDIO)
- dkcmult~ - multiplication of two complex signals. 
- dkcnorm~ - normalization of a complex. 
- dkcdiv~ - division of two complex signals.
- dkeq~ - equal to
- dkge~ - greater than or equal to
- dkgt~ - greater than
- dkle~ - less than or equal to
- dklt~ - less than
- dkne~ - not equal to
- dknum~ - signal to float
- dkrandom~ - abstraction simulating the output of the Max/MSP rand~ object.
- dkrange~ - range mapping (audio rate)

## MATH (CONTROL)
- dk0bltodec - binary list to base 10
- dkdecto0bl - base 10 to binary list
- dk2dto1d - 2d (x y) to 1d coords (successive rows of x) 
- dkaccum - running sum
- dkbpmtoms - bpm to ms
- dkdecrease - detect decreases 
- dkdrunk - a vanilla version of drunk
- dkdrunk2 - drunk with floats
- dkeqtemp - degree to equal temperament in Hz
- dkexp_r - reciprocal exponential
- dkfround - round float
- dkfdec - get decimal part of float
- dkfdectol - pass float if within decimal tolerance of int
- dkincrease - detect increases 
- dkmstosmp - ms to samples
- dknearest - floor to the nearest grain
- dknearest - round to the nearest grain
- dknearpow2 - rounds input to a power of 2
- dkrandi - random int within a given range
- dkrange - range mapping (control rate)
- dkrdiv - vanilla reverse division
- dkpow - vanilla reverse power
- dkrrand - random number in a given range
- dkrsub - vanilla reverse subtraction
- dkrunmax - running maximum
- dkrunmin - running minimum
- dkunit2ms - ms calculator
- dkunique - flag input as unique (or not)
- dkvavg - vanilla float averager
- dkvrgauss - vanilla random number generator with gaussian distribution (i think) using the Marsaglia polar method

## MODULATION
- dksfm~ - simple/signal-inlet (for mod idx) frequency modulation synthesis

## MUX
- dkvmux - dynamically patched version of input multiplexing
- dkvmux2/3/4/5/6/7/8 - vanilla multiplexer (control)

## OSC
- dkvanssimp~ - triggered single-sample impulse
- dktri~ - triangle oscillator

## REVERB
- dkschroeder1~ - a schroeder reverb (1-in,4-out)
- dkschroeder2~ - satrev chowning schroeder reverb (1-in, 2-out)

## PANNING
- dkcomppan~ - -4.5 dB panner (compromise panner)
- dkcospan~ - cosine-based equal-power panner
- dklinpan~ - linear panner
- dkstpan~ - stereo-to-stereo panning 

## PULSAR SYNTHESIS
- dkpulsar~ - pulsar synthesis (unwindowed)
- dkpulsar-hann~ - pulsar synthesis with hann window

## STRUCTURE
- pdkst-init - clear scalars and init iterating over given element
- pdkst-nth - get nth scalar of a structure 
- pdkst-textdefine - emulate [text define] methods for text struct member

## TEXT
- pdktext-getval - get value from associated key (treating text like a hash table)

## WINDOWING
- dkhamm~ - generates hamming window according to input 0 to 1. 
- dkhann~ - generates hann window according to input 0 to 1
- dkhannmaker - constructs hann window. args are array name where window is stored, window size, and overlap.
- dkhannnorm~ - normalizes an incoming signal according to hann window (usu. after an ifft~). args are window size and overlap.
- dktukeymaker - tukey window constructor. ideal for grain envelopes. 

## MISC
- dklogidy - abstraction to deal with default settings of logidy umi3

## NOT-VANILLA ABSTRACTIONS
- dkamixer~ - abstraction over ggee/shell to set volume with amixer (Linux only)
