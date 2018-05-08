**NOTE**: 

- This file is the Markdown used to generate the `README.pdf` at https://drive.google.com/drive/folders/1ns5l39SVS9OjJM8-ahHKgXOwguSFjjuo. 
- This repo is used as a public space for filing scidb issues, though the [SciDB forum](http://forum.paradigm4.com/) is probably a better option for the same. 

# Links

For SciDB 18.1 community edition,

- Get `.tgz` of source code [here](https://downloads.paradigm4.com/community/18.1/)
- Get installer script [here](https://downloads.paradigm4.com/community/18.1/install-scidb-ce.sh) (Get installer instructions [here](https://paradigm4.github.io/scidblog/scidb-installation/))
- Consult the [official docs](https://paradigm4.atlassian.net/wiki/spaces/scidb/pages)

# SciDB VM

This directory also contains a SciDB 18.1 Community Edition Virtual Machine for VirtualBox. The VMs use Ubuntu
14.04 with credentials as follows:

```sh
username: scidb
password: paradigm4
```

In addition to SciDB 18.1 CE, the VMs contain a few prototype plugins from P4Labs, the SciDBR
interface and RStudio server. There is very minimal data preloaded to save VM space. The directory
`/home/scidb` contains a few R scripts with basic demos and plots. We included small excerpts and
derivatives of the following datasets:

- The NASA MODIS Instrument: http://modis.gsfc.nasa.gov/
- The 1000 Genomes Project: http://www.1000genomes.org/
- The IHI 2012 Accelerometer Study: http://www.ess.tu-darmstadt.de/datasets/ihi_2012

These are provided for illustration purposes only.
EC2 AMIs with larger datasets and more example queries are also available upon request. If you’d like to
try out AMIs, the SciDB Enterprise Edition, have questions or need help with a particular use case, we’d
love to hear from you. Contact us via the following addresses:

# Contact us

For specific industry applications: 

- [LifeSciences@paradigm4.com](mailto:LifeSciences@paradigm4.com) 
- [FinancialMarkets@paradigm4.com](mailto:FinancialMarkets@paradigm4.com)

For general inquiries: 

- [info@paradigm4.com](mailto:info@paradigm4.com) 
- [SciDB forum](http://www.paradigm4.com/forum)
