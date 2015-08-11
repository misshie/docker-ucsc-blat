# Docker containers for UCSC BLAT servers with reference genomes, human hg19, hg38 and mouse mm10

## Running containers

```shell
$ sudo docker run -it -p 55519:55519 misshie/ucsc-blat-hg19
$ sudo docker run -it -p 55538:55538 misshie/ucsc-blat-hg38
$ sudo docker run -it -p 55538:55538 misshie/ucsc-blat-mm10
```

Note that it takes servers for several minuites to prepare k-mer indices.

## Query

You have to install gfServer locally

```shell
$ wget http://hgdownload.cse.ucsc.edu/admin/exe/linux.x86_64/blat/gfServer
```

And try command for queries. See http://hgdownload.cse.ucsc.edu/admin/exe/linux.x86_64/blat/

For example, you can see the server status by the following command: ```gfServer status localhost 55519```.

## Copyright
**Copyright**: (c) 2014 MISHIMA, Hiroyuki (hmishima at nagasaki-u.ac.jp / Twitter: @mishima_eng (in English) and @mishimahryk (in Japanese) 

**License**: The MIT license

