# Modified_swmmtoolkit_files
Fix some small problems when reading multi-variate water quality data using swmm.toolkit and pyswmm

When extracting multi-variate water quality results, there is only a POLLUT_CONC_0 in the original swmm.toolkit.shared_enum.py. The POLLUT_CONC_0 will work on the first defined pollutant, while it will result in failures when extracting extra pollutant simulation results. The shared_enum.py is modified here for this purpose.
