# Dell_DVDStore_SQL
The Dell DVD  Store is an open source simulation of an online e-commerce site with different SQL implementations.

### Download and assemble a PostGRE SQL implementation of the Dell DVD Store data

The data can be downloaded from the [Dell DVD Store](https://linux.dell.com/dvdstore/). Make sure to download the ds21.tar.gz file and zipped file containing the correct implementation - in my case PostGRE SQL (ds21_postgresql.tar.gz).

I used an AWS large 2.2x instance and installed PostGRE SQL. Using `wget`, I downloaded both the above mentioned files to the instance. The zipped files can be unzipped as follows:

`tar xvzf <_filename_> -C <_file path_>`

> What does xvzf stand for? The 'x' tells the tar command to extract files. The 'v' tells tar to list all files one by one, and stands for 'verbose'. The 'z' command tells tar to uncompress the gzip file, and 'f' tells tar to expect a filename from you.

> What is the -C option for? The default location for tar to dump the uncompressed files is the current directory you are on (what you get by typing `pwd` on the command line). However, if you want to save these files at a different location, you get to specify that after the -C. So, it is used to change the directory where the uncompressed files will be stored.

For assembling the tables in Postgresql, make sure that the data_files folder is the 
