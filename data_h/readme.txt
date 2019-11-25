============== Velocity model =================
vz_ascii.txt

vz_ascii.txt stores the homogeneous velocity model (vp=2km/s). 
The total number of grids along the lateral direction is 501, and the total number along the vertical direction is 501.
The grid spacings along the lateral and vertical directions are 0.01km. 
The first grid coordinates along the lateral and vertical directions z0=0km and x0=0km. 
Because the grids are sampled regularly, we may calculate the positon of a selected gird easily. 


In vz_ascii.txt, the velocity valuables are stored in a long column. The first 501 numbers are the velocity valuables along the leftest column of the velocity matrix (501 by 501). The next 501 numbers are those along the second left column (from left) of the velocity matrix. 


============== Training data ===============
source5by5_ascii.txt
time_surface5by5_ascii.txt


source10by10_ascii.txt
time_surface10by10_ascii.txt


source15by15_ascii.txt
time_surface15by15_ascii.txt


source20by20_ascii.txt
time_surface20by20_ascii.txt


The data structure is explained as follows.
For example, the first set of files: source5by5_ascii.txt and time_surface5by5_ascii.txt.
Here, 5by5 means the total number of shots are 5*5=25, the first and second 5 denote the numbers along z and x, respectively.
The source5by5_ascii.txt stores the source positions. In this file, each line stores (z, x, y), where y is always zero, so we may disregard it.

time_surface5by5_ascii.txt stores the traveltime recorded at surface. Here, 5by5 corresponds to the source file "source5by5_ascii.txt".
In time_surface5by5_ascii.txt, the traveltimes are stored in a long column as before. 
Because we have 501 receivers at surface, the first 501 numbers in time_surface5by5_ascii.txt correspond to the first source position (z, x, y) in source5by5_ascii.txt.
The next 501 numbers in time_surface5by5_ascii.txt correspond to the next source position in source5by5_ascii.txt.


The other files can be understood by analogy with my above explanation. Please note that the total number of receivers (501) is not changed. 

Note that in all the above source files, the source positions are generated regularly.  


=============== Test data =====================
test_source100_ascii.txt
test_time_surface_ascii.txt

test_source100_ascii.txt stores 100 randomly generated source positions. Its structure can be known by analogy with source5by5_ascii.txt.
test_time_surface_ascii.txt stores the traveltime recorded at the surface. The total number of receivers is 501. Its structure can be known by analogy with time_surface5by5_ascii.txt.
 

