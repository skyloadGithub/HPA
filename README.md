1) Harmony Progression Analyser (Vamp plugin package)

A. General Description

The Harmony Progression Analyser (HPA) is a key, chord and bass simultaneous estimation system that purely relies on machine learning techniques. It also uses a novel choromagram extraction (namely loudness based chromagram) method, which is inspired by loudness perception studies. Compared with other audio chord estimation (ACE) systems, HPA is fast and memory-efficient, achieving an excellent tradeoff between performance and memory and time efﬁciencies.

The release is the HPA vamp plugin (Win32/Linux32/Linux64/Mac versions) for Sonic Visualiser (http://www.sonicvisualiser.org/). The plugin has a user friendly interface and it targets on musicians who are less experienced with additional MATLAB run-time library installation. If you would like to use BATCH PROCESSING for a set of audio files, try our plugins on SONIC ANNOTATOR (http://www.omras2.org/SonicAnnotator).

For more details, the readers are referred to the following papers: 

------------------------------------------------------------------------------------------

Y. Ni, M. Mcvicar, R. Santos-Rodriguez, and T. De Bie. An end-to-end machine learning system for harmonic analysis of music. IEEE Transactions on Audio, Speech and Language Processing, 20(5):1771-1783, 2012.

Y. Ni, M. Mcvicar, R. Santos-Rodriguez, and T. De Bie. Harmony progression analyzer for mirex 2012. In Proceedings of Internal Society of Music Information Retrieval Conference (MIREX), 2012.

Y. Ni, M. Mcvicar, R. Santos-Rodriguez, and T. De Bie. Harmony progression analyzer for mirex 2011. In Proceedings of Internal Society of Music Information Retrieval Conference (MIREX), 2011.

------------------------------------------------------------------------------------------

If you use this software package in your scientific work, please cite as

Y. Ni, M. Mcvicar, R. Santos-Rodriguez, and T. De Bie. An end-to-end machine learning system for harmonic analysis of music. IEEE Transactions on Audio, Speech and Language Processing, 20(5):1771-1783, 2012.

B. Acknowledgement

This work is funded by the EPSRC grant (EP/G056447/1) and the PASCAL2 EU Network of Excellence. Particularly thanks are owing to C. Harte, for his chord labelling files and chord parsers; the labROSA group, for their sophisticated beat tracker; and Dr. M. Mauch, for kindly making the code of his Musical Probabilistic model available to us, as well as several helpful discussions on the evaluation of audio chord estimation systems. The HPA Vamp Plugin also makes use of the following libraries: FFTW3, Vamp plugin SDK and resample template. Many thanks to their authors. 

C. Contact 

For any problem w.r.t. this plugin, please contact Yizhao.Ni@googlemail.com.

D. Reference

1. Y. Ni, M. Mcvicar, R. Santos-Rodriguez, and T. De Bie. An end-to-end machine learning system for harmonic analysis of music. IEEE Transactions on Audio, Speech and Language Processing, 20(5):1771-1783, 2012.

2. Y. Ni, M. Mcvicar, R. Santos-Rodriguez, and T. De Bie. Harmony progression analyzer for mirex 2011. In Proceedings of Internal Society of Music Information Retrieval Conference (MIREX), 2011.

3. M. Mauch. Automatic chord transcription from audio using computational models of musical context.  Ph.D. dissertation, Queen Mary University of London, 2010.



2) Harmony Progression Analyser (Matlab package)

Harmony_Progression_Analyzer_Toolbox_ver1.2.zip includes the Matlab version of HPA. Since the software package is coded in Matlab, the user needs Matlab2008b or higher versions to run the program. The user can still run the system using old Matlab versions, but he/she may encounter warnings since the program uses containers.Map().

If the system is running on an Apple Macintosh computer, the user needs to run the script "code_compile_shell.m" first to compile the following Mex functions:

    ./Feature_extraction/HPSS_innerLoop.c
    ./HMM_model/bass_viterbiDecoder_c.c
    ./HMM_model/bass_viterbiDecoder_var_c.c
    ./HMM_model/key_viterbiDecoder_c.c
    ./HMM_model/key_viterbiDecoder_var_c.c
    ./HMM_model/viterbiDecoder_c.c

Please refer to READ_ME.txt in the toolbox for detaled instruction.
