This reporitory contains codes related to my work over the summer of 2013 under the guidance of Prof. Anand Narayanan at IIST, Trivandrum, India.

Colors of quasars can be used to estimate their redshift. Richards et al (2001) studies the accuracy of this method. My work over the summer of 2013 was to reproduce these results. Putting together the original data set was harder than expected so i downloaded a more up-to-date data set by querying the DR9 using the limits on u, g, r, i & z magnitudes set by the original paper. Querying DR9 or DR10 for that matter was a bit taxing my system so it is suggested the query is run through SDSS CASjobs instead. The final data set ended up being a csv file ~20 MB in size with ~150,000 rows and 12 columns, so in hind sight, it was a bad decision letting firefox open this in the browser.

The sql query file is available in the directory under the same name. To understand the syntax, one should go through the SDSS Schema browser.

colors.png is the u-g, g-r, r-i and i-z color vs redshift plot.
colors.py is the python script to generate the figure. NOTE : pandas needs to be installed for the script to run.
colors_of _quasars.ipynb is an ipython notebook regarding the same.
you can access the ipython notebook using nbviewer at 
http://nbviewer.ipython.org/github/rahulporuri/quasar_colors/blob/master/colors_of_quasars.ipynb

work so far - 

* sql query
* downloaded data
* histogram of redshift
* python script, ipynb notebook and colors


to be done - 

* median color code
* template spectrum and simulated color-redshift relation
* variation from the median color