![](http://www.xcelrislabs.com/Images/Xcelris-An-Abellon-Company-Logo.png)

> #### _We make DNA speak.._





---

# Welcome to Xcelris Labs Ltd. GitHub Pages

###            (by Bioinformatics division)

---

### *prepare_taxa_charts.py*: Ultrafast program to generate publication ready taxonomic pie chart images from QIIME

![]( https://httpsimage.com/img/flowchart4.png)

* This script parses the pie_chart.html file (output from [`plot_taxa_summary.py`](http://qiime.org/scripts/plot_taxa_summary.html))

* Maps the pie chart and legend image names to corresponding samples.

* Copies the files to user defined directory

* Rename the files according to sample ids

* Merges the pie charts and legends

---

## Usage

 `python prepare_taxa_charts.py -p pie_charts.html -c /charts_folder
-o user_defined_output_folder`

---

## List of Python modules used 

1. [fnmatch](https://docs.python.org/2/library/fnmatch.html)
2. [getopt](https://docs.python.org/2/library/getopt.html)
3. [os](https://docs.python.org/2/library/os.html)
4. [PIL](http://www.pythonware.com/products/pil)
5. [shutil](https://docs.python.org/2/library/shutil.html)
6. [sys](https://docs.python.org/2/library/sys.html)
7. [re](https://docs.python.org/2/library/re.html)
8. [timeit](https://docs.python.org/2/library/timeit.html)
 

---

## Important Note

Prerequisites for `prepare_taxa_charts.py`:

1. Python v2.7. The program will not work with Python v3. Python v2.7 was chosen as it is stable.

2. Legend files should be generated in `png` format (default is pdf). This could be achieved by running the script `plot_taxa_summary.py` with the option `-t/--type_of_file` as `png`. Given below is an example:

`plot_taxa_summary.py -i phylum.txt -l phylum -c pie -o phylum_charts/ -t png`

** Note: High resolution images can be generated using the `-d`, `--dpi` option for the script `plot_taxa_summary.py`. See below example (setting the dpi to 100 produce good quality images):

`plot_taxa_summary.py -i phylum.txt -l phylum -c pie -o phylum_charts/ -t png -d 100`

---

## License

This script is released under GNU GENERAL PUBLIC LICENSE, v3, 29 June 2007

---

## Development and Maintenance

Developed by - Vijay Lakhujani

vijay.lakhujani@xcelrislabs.com **[Project Scientist, Bioinformatics]**

Maintained by @Xcelris-Labs-Ltd on GitHub.

---

## Correspondance

chandan.badapanda@xcelrislabs.com **[Associate General Manager, Bioinformatics]**

[Xcelris Labs Ltd. &#169;](http://www.xcelrisgenomics.com/ContactUs.html)