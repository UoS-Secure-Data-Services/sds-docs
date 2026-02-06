# Installing packages in the DSH machine

There is a proxy setup in the DSH allowing users to download a set of Python pypi and R's CRAN packages.

## Python 

Here is a list of packages whitelisted for use in the DSH

+ contourpy
+ cycler
+ fonttools
+ duckdb
+ kiwisolver
+ matplotlib
+ numpy
+ packaging
+ pandas
+ pillow
+ pyparsing
+ python-dateutil
+ pytz
+ six
+ tzdata

## R

Here are a list of CRAN packages whitelisted for use in the DSH

!!! note
    Some of the packages may not install correctly in Linux without
	installing additional packages. These can be installed with
	'sudo apt install <package name>' in Ubuntu.
	These packages are pre-built for Windows (binaries), so this is not a problem.

+ cli
+ data.table
+ remotes
+ ggplot2
+ glue
+ cpp11
+ farver
+ labeling
+ R6
+ RColorBrewer
+ viridisLite
+ gtable
+ isoband
+ lifecycle
+ rlang
+ S7
+ scales
+ vctrs
+ withr
