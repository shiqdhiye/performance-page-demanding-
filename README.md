# performance-page-demanding-

scenario of demand paged memory.
  
# Consider a scenario of demand paged memory. Page table is held in registers. It takes 8 milliseconds to service a page fault if an empty page is available or the replaced page is not modified and 20 milliseconds if the replaced page is modified. Memory access time is 100 nanoseconds. Assume that the page to be replaced is modified 70 percent of the time. Generate a solution to find maximum acceptable page-fault rate for access time that is not more than 200 nanoseconds.


#  solution 

# GIVEN DATA
1 Millisecond = 1,000,000 Nanoseconds

PAGE FAULT (EMPTY) = 8 M SEC , (8,000,000)
PAGE FAULT (REPALCEMENT) = 20  M SEC , (20 ,000 ,000)
MEMORY ACCES TIME (MAT) =100 NANO SEC,
PAGE REPLACEMENT PERCENTAGE = 70% = 70/100= (0.7)
AFFECT TIME ACCESS TIME (EAT)= 200 NANO SEC

EAT = (1-P) * MEMORY ACCESS TIME + P(PAGE FAULT)

PAGE FAULT= (PAGE FAULT * % OF  PAGE FAULT ) + PAGE REPLACEMENT * % PAGE REPLACEMENT )..
PAGE FUALT = 1-PAGE REPLACEMENT PERCENTAGE = 1-0.7= (0.3)
		    PAGE FAULT (EMPTY)= 0.3%

PAGE FAULT = (8,000,000 * 0.3 ) + (20,000,000 * 0.7) = 
		     
	        PAGE FAULT   =  2,400,000 + 14,000,000 = 16,400,000
EAT = (1-P) * MEMORY ACCESS TIME + P(PAGE FAULT) ...
		200 = (1 P) * 100 + p( 16,400,000)...
		200 =  100 – 100P + P16,400,000...	
		200 – 100 = P(16,400,000 – 100)...
		100 = P(16,399,900)..
		p = 100/16,399,900..
P = 6.09x10-6
