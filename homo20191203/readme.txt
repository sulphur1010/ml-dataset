The data structures in the following file are similar to those in the files shown on homo20191121, which I gave Mustaffa about the 5by5, 10by10, 15by15, 20by20 source and time files. 

=============== Test data =====================
test_source101by101_ascii.txt
test_time_surface101by101_ascii.txt

test_source100_ascii.txt stores 101*101 (10201) randomly generated source positions. Every 3 lines shows (z, x, y), where y is always zero and hence it is useless. 

test_time_surface101by101_ascii.txt stores the traveltime recorded at the surface. The total number of receivers is 501. Every time, read 501 lines, which corresponds to a source. We may read in such a way totally 10201 times, because we have 10201 sources. The source position corresponding to these 501 lines can be obtained from the test_source101by101_ascii.txt file.

 

