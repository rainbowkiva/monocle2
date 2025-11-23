
BUG Fix: 
=======================
1. 修改order_cells.R文件中mst_traversal <- graph.dfs(dp_mst, root=root_cell, neimode = "all", unreachable=FALSE, father=TRUE)的neimode为mode，解决了函数"The neimode argument of dfs() was deprecated in igraph 1.3.0 and is now defunct."的报错；
2. 修改order_cells.R文件中所有suppressWarnings(nei的nei为.nei，解决了函数"Error:!nei()was deprecated in igraph 2.1.0 and is now defunct.Please use.nei()instead."的报错；
3. 修改BEAM.R文件中suppressWarnings(.nei(branch_cell))的nei为.nei，解决了函数"Error:!nei()was deprecated in igraph 2.1.0 and is now defunct.Please use.nei()instead."的报错；
4. 修改DESCRIPTION文件，第一行添加"Encoding: UTF-8"行，解决了安装包时"Error : DESCRIPTION文件无效 没有这种编码"的报错。


MONOCLE
=======================
Monocle is an analysis toolkit for single-cell RNA-Seq experiments.  To use this package, you 
will need the R statistical computing environment (version 3.0 or later)
and several packages available through Bioconductor and CRAN.

We highly recommend installation of Monocle through the bioconductor project. 
See here for details:

https://bioconductor.org/packages/release/bioc/html/monocle.html

News and announcements for the Monocle project will appear here:

http://cole-trapnell-lab.github.io/monocle-release/

This release supports Mac OS X and Linux. Windows may support this 
build, but Monocle has not been tested on Windows yet.
