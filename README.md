# CFG and LiGA Comparison

Python scripts used in [Genetically Encoded, Multivalent Liquid Glycan Array (LiGA)](https://www.biorxiv.org/content/10.1101/2020.03.24.997536v1).

### Script use:

```shell
cd python_scripts
python3 script_name.py
```

### Scripts:

``download_cfg.py`` searchs terms on the CFG website and downloads the resulting XLSX files.

``align_CFG.py`` aligns the downloaded XLSX files into single CSV files.

``download_all_CFG.py`` downloads all the XLSX files from the CFG website.

``IUPAC_converter.py`` is a library for converting CFG glycans to standard IUPAC.

``draw_glycans.py`` uses [DrawGlycan-SNFG](http://www.virtualglycome.org/DrawGlycan/) and Matlab to glycans.

### Data inputs:

``terms.csv`` takes terms to be searched and aligned.

``glycans.csv`` takes glycans to be drawn.

### Requirements:

```shell
pip3 install -r requirements.txt
```

* pandas
* numpy
* urllib
* matlab (Requires Matlab installation)
