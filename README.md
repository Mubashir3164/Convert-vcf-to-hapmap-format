# Convert-vcf-to-hapmap-format
# Download tassel commandline version

Here is the guidline to install commandline interface of tassel version 5.0

https://bytebucket.org/tasseladmin/tassel-5-source/wiki/docs/Tassel5PipelineCLI.pdf?rev=eeb05c28894bf976c84bb110ec545647ab9a2f08

# Prerequisites

Java development kit 8.0 or later is required 
# Convert Vcf to Hapmap

After installing tassel, put your vcf file into your current working directory then run the following command to convert vcf format to hapmap

./run_pipeline.pl -Xms10g -Xmx40g -fork1 -vcf data.vcf -export outputfilename -exportType Hapmap

Here, Xms10g and Xmx40g are intial and maximum memory sizes, respectively. Modify it according to the memory of your computer. 
 
 The output file will be a hapmap file. 
 
Tassel also has a GUI, if the size of vcf file is not very big, then tassel GUI can be used for conversion. However, for large datasets tassel commandline is recommended. 

# Reference

Peter J. Bradbury, Zhiwu Zhang, Dallas E. Kroon, Terry M. Casstevens, Yogesh Ramdoss, Edward S. Buckler, TASSEL: software for association mapping of complex traits in diverse samples, Bioinformatics, Volume 23, Issue 19, 1 October 2007, Pages 2633–2635, https://doi.org/10.1093/bioinformatics/btm308
