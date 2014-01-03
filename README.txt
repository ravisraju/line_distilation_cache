This is an Implementation of Distill cache in Simple Scalar

Environment Requirements -

Ubunutu 13.04
Simple Scalar Tool

Setting up simple scalar

cd simplesim-3.0
Run make config-alpha
Run make all

Make sure there are no errors in the make command

working_dir_project is the folder where the benchmarks and runscripts are present

To run the benchmarks, 

cd working_dir_project
./my_run_1
./my_run_2
./my_run_3
./my_run_4
./my_run_5

Each command runs 4 of the benchmarks. For the sake of convenience and running parallely in two machines, we have split the runscripts. 


script			benchmarks run in the script

my_run_1  -   "ammp" "applu" "apsi" "art"
my_run_2  -   "bzip2" "crafty" "equake" "fma3d" 
my_run_3  -   "galgel" "gap" "gcc" "gzip" 
my_run_4  -   "lucas" "mcf" "mesa" "mgrid" 
my_run_5  -   "parser" "swim" "twolf" "vortex" "vpr"


The script runs 4 different configurations for each benchmark. Hence 21 * 4 combinations are run and the output logs are stored in the corresponding benchmark directories.

Report is attached in the main folder itself.