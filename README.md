#### About the script:

This script parses the `pie_chart.html` file coming from `plot_taxa_summary.py` script from QIIME (for details, visit http://qiime.org/scripts/plot_taxa_summary.html.) and do the following:
  
1.Maps the pie chart and legend image names to corresponding samples.

2.Copies the files to user defined directory

3.Rename the files according to sample ids

4.Merges the pie charts and legends   


#### List of Python modules used in `merge_QIIME_images.py`

| S. No.        | Module        |
| ------------- |:-------------:|
| 1             |  fnmatch      |
| 2             |    os         |
| 3             | getopt        |
| 4             | PIL           |
| 5             | re            |
| 6             | shutil        |
| 7             | sys           |



#### Usage:
`merge_QIIME_images.py -p path_to_pie_charts.html -c path_to_charts_folder -o output_path_to_final_images`

#### Important Note:
Prerequisites for `merge_QIIME_images.py`

1. Python version 2.7

2. The legend files should be generated in png format (default is pdf). This could be achieved by running the script `plot_taxa_summary.py` with the option `-t/--type_of_file as png`. Given below is an example:

`plot_taxa_summary.py -i phylum.txt -l phylum -c pie -o phylum_charts/ -t png`

#### License
This script is released under GNU GENERAL PUBLIC LICENSE, v3, 29 June 2007

#### Author:
Vijay Lakhujani  (c) 2016 | Xcleris Labs Ltd.
