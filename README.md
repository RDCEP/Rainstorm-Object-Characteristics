# Rainstorm-Object-Characteristics
Rainstorm Object Characteristics for Stage IV (2002-2011)

The .mat files contain the characteristics of the rainstorm objects constructed by the methods described in Chang et al. (2016), in the Stage IV data set. Each file contains rainstorm objects for each season, from 2002 to 2011. 

Since Stage IV data are known to be unreliable in the West Coast area, the region east of 114 W is excluded from the analysis.  

Time and location information: 

dvc_total: matrix containing date and hour for each time step. 
centroids_mean: cell vector containing the center location of the rainstorm at each time step. The center location is computed as the ‘center of gravity’ as described in Chang et al. 2016. Each coordinate is in (lat,long).

Storm characteristics: 

init_time: starting time step 

end_time: ending time step

To get the date and time for the starting and ending time step, run dvc_total(init_time,:) or dvc_total(end_time,:).

duration: number of time steps that individual rainstorms last. To compute the actual duration time multiply 3 (hours).

amount: sum of precip intensity at all grid cells (i.e. total depth). 

extent: total number of grid cells with positive (>0.1mm) precip intensity. To compute the actual area, multiply (16 km^2).

Reference
Chang, W., Stein, M. L., Wang, J., Kotamarthi, V. R. and Moyer, E. J. (2016) Changes in Spatio-temporal Precipitation Patterns in Changing Climate Conditions, Journal of Climate, 29 (23), 8355-8376
readme.txt
Displaying readme.txt.
