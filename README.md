# ViPErLEED-betatest
The most recent executables for the ViPErLEED package. The complete source code of the ViPErLEED package will be made available to the general public as soon as possible (i.e., after submission of relevant manuscripts).

The contents of this repository are solely intended for internal use, and should not be distributed without explicit consent. Please contact riva@iap.tuwien.ac.at in advance if you wish to redistribute any of the content. We are happy to officially include new users as beta testers.

You find the most recent release in the "Releases" section on the right. Each release is accompanied by a Change Log with the most recent changes, and contains:
- GUI: archive containing the graphical user interface (Windows >= 7, UNIX) and some example input files. Offers a LEED pattern preview, and exports a "pattern file" required by the spot tracker.
- tleedm: for LEED-IV calculations. This is usually only packed for UNIX. Performs LEED-IV calculations based on the TensErLEED package from input files. This creates quite a lot of files, so it is recommended to have an additional job script (see, e.g., example-job.sh) moving the input files and tleedm executable into a work folder and executing it there. When exiting, tleedm will create a "manifest" file, which is a list of files and folders that should be copied back.
- bookkeper: for keeping track of your calculations in a file "history.info". This is usually only packed for UNIX. See example-job.sh for an example of bookkeeper usage. Execute bookkeeper with flag "-c" for continuation jobs, i.e. to overwrite the POSCAR and VIBROCC input files in the main folder with the latest POSCAR_OUT and VIBROCC_OUT from the OUT folder.
- tensorleed: archive of the core TensErLEED [[Comput. Phys. Commun. **134**, 392 (2001)](https://doi.org/10.1016/S0010-4655(00)00209-5)], and related code. EEASiSSS [[Phys. Rev. B **76**, 195441 (2007)](https://doi.org/10.1103/PhysRevB.76.195441)] is distributed with kind permission from [John Rundgren](https://www.kth.se/profile/jru?l=en).
- doc: archive with the most recent documentation. Accessed from the ViPErLEED_doc link or by opening the ./doc/index file.

Please, use the "Issues" tab to open new issues should you encounter any bug, for new-feature requests, as well as for comments on usability of the package.

You can also open an Issue in case you would like executables packed for different operating systems.


