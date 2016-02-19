# cryo-toolbox
Public repo for Python modules which may be useful for parsing/plotting sea ice data (e.g. from NSIDC, seismic traces)

Overview of modules:
nsidc_sic is a way to visualize NSIDC sea ice concentration data for the south pole.
It assumes that the Basemap module has already been installed; if this is not the case, an easy way to install it is using the Anaconda distribution of Python.

demo script for NSIDC:
os.chdir("/directory/with/nsidc/files")
data, date = get_data_nsidc("filename")
plot_map_nsidc(data, date, show=True, contours=True)

This will generate a colour plot of SIC with contours for that file.
