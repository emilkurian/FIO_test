# FIO_test

**Purpose** : Quick script to help automate FIO runs
**NOTE** : The script is very cobbled together, feel free to make changes

## Usage

Standard parameters are included in the script, but arguments can be passed in.

### command line arguements/parameters:

-d, --device: devices you would like to benchmark
-s, -- ize: size of FIO file genereated during benchmark
-o, --output: folder to save FIO output + CSV file if requested
-rw, --readwrite: (random or sequential)(read,write)
-n, --numjobs: number of jobs to run

**Examples**:

`python3 fioTest.py` 

Will run all the default values

`python3 fioTest.py fioTest.py -d /dev/sda -s 1G -o test_folder -n 16 -rw randread -c`

Will run random read testing on /dev/sda, with a file size of 1 GB, numjobs of 16, and save all output and a CSV of the data in a subfolder test_folder
