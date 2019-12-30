# CFG and LiGA Comparison

The script that downloads most of the available CFG data for a particular lectin is download_CFG.py and it enters the given term in the search tool of the CFG website. The results for the search are used to extract PSIDs or 'primescreen ID' which is something the CFG website used to keep track of all their data. The PSIDs can be used to download the available data on the given lectin.

The script that aligns the data for a lectin is align_CFG.py and it identifies three data storing formats CFG has used as it evolved over time. The glycan names of all the formats are converted to IUPAC condensed using IUPAC_converter.py and the three glycan orders are merged to form a fixed order for all three formats found in order.xlsx. Each CFG data file is then parsed, its format is identified, glycan array data is extracted and appended to this order. Heatmaps are generated once all the data is appended.

Glycan drawings are drawn by a script called draw_glycans.py which uses a tool called DrawGlycan-SNFG. Each glycan from glycans.csv is sent to the matlab scripts of their tool and an SVG format of the drawing is saved.

CFG raw data can be downloaded [here](https://drive.google.com/drive/folders/1vnQsgsB0Iv1wKDhFzHuAEhz78P1OTkrS?usp=sharing).

The tool used for drawing glycans is [DrawGlycan-SNFG](http://www.virtualglycome.org/DrawGlycan/).
