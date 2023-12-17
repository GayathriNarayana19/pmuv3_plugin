I have pushed the compiled object files and static libraries for ease of use. 

However, these are the compilation steps 

To Generate Object file
gcc —c pmuv3_plugin.c -I/home/ubuntu/linux/tools/lib/perf/include -o pmuv3_plugin.o 

To Generate static library
ar rcs pmuv3_plugin.a pmuv3_plugin.o

How libperf.a and libapi.a were compiled?

STEP 1: Clone this linux source repository.

git clone git://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git

STEP 2: Go to /linux/tools/lib/perf 
        make 
        
STEP 3: Go to /linux/perf/tools/lib/api
        make 

STEP 4: Copy libperf.a and libapi.a to the perf_cycle_codes directory 


