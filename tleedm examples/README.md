This folder contains sets of example input files for tleedm.

The experimental IV data in EXPBEAMS files shown here may be unpublished. Please do *not* distribute these examples without express permission.

You find below a list of refence timings and expected results for the examples given, including which version of ViPErLEED was used on which machine.

### Fe2O3-012-1x1
* ViPErLEED: [v0.2.1](https://github.com/viperleed/viperleed-betatest/releases/tag/v0.2.1);
  Machine: Parallels Desktop VM (Ubuntu 20.04) on MacOS 11.2.3; 1 CPU (3.8 GHz Intel i5), 4 GB RAM; ifort compiler
    * First initialization [Segment: 0]: ~9 s
    * Reference [Segment: 1]: 1:37 h
    * Delta [Segment: 2] (3 cumulated runs): 34 m
    * Search [Segment: 3] (3 cumulated runs): 8:10 h
    * Total execution time (`RUN = 1-3`) [Segments: 0 1 11 2 3 31 12 2 3 31 12 2 3 31 12]: 10:25 h
    * R-factors: refcalc = 0.3889; superpos = 0.3725
    * Note: slightly worse R-factors due to an input problem (was meant for v0.3.0, used with v0.2.1 -> wrong bulk repeat), and a bug in bulk attachment (resolved in v0.5.0)
* ViPErLEED: [v0.4.0](https://github.com/viperleed/viperleed-betatest/releases/tag/v0.4.0);
  Machine: openSUSE Leap 15.2; 16 CPUs (2.1 GHz Intel Xeon E5-2620 v4), 125 GB RAM; ifort/mpifort compiler
    * First initialization [Segment: 0]: ~1 s
    * Reference [Segment: 1]: 13 m
    * Delta [Segment: 2] (3 cumulated runs): 9 m
    * Search [Segment: 3] (3 cumulated runs): 1:44 h
    * Total execution time (`RUN = 1-3`) [Segments: 0 1 11 2 3 31 12 2 3 31 12 2 3 31 12]: 2:12 h
    * R-factors: refcalc = 0.3856; superpos = 0.3691
    * Note: slightly worse R-factors due to a bug in bulk attachment (resolved in v0.5.0)
* ViPErLEED: [v0.5.0](https://github.com/viperleed/viperleed-betatest/releases/tag/v0.5.0);
  Machine: Windows Subsystem for Linux on Windows 10; 6 CPUs (3.8 GHz AMD Ryzen 5), 8 GB RAM; ifort/mpifort compiler
    * First initialization [Segment: 0]: ~1 s
    * Reference [Segment: 1]: 32 m
    * Delta [Segment: 2] (3 cumulated runs): 16 m
    * Search [Segment: 3] (3 cumulated runs): 2:31 h
    * Total execution time (`RUN = 1-3`) [Segments: 0 1 11 2 3 31 12 2 3 31 12 2 3 31 12]: 3:23 h
    * R-factors: refcalc = 0.3393; superpos = 0.3196
    * Note: With relatively high LMAX = 14 at 800 eV (due to increased default precision of PHASESHIFT_EPS) -> slower delta & search than previous versions
