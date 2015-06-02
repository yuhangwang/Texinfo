# Texinfo
**GNU Texinfo**

This is an unofficial verbatim redistribution of the binary&source form of the  GNU Texinfo package under its open source license (GPL 3.0) terms (see the LICENSE file).

This redistribution is under the same license as the original.

Please visit the official website for more details: http://www.gnu.org/software/texinfo

## Download
You can download the compiled binary files at the [release page](https://github.com/yuhangwang/Texinfo/releases).

## Compilation notes
### Compilation environment
* CentOS 6.6
* x86_64 architecture
* Compiler: gcc version 4.4.7 20120313 (Red Hat 4.4.7-11)

### Compilation steps
#### Version: 8.6.4
```bash
wget http://ftp.gnu.org/gnu/texinfo/texinfo-5.2.tar.gz
tar zxvf texinfo-5.2.tar.gz
mkdir build_texinfo-5.2
cd build_texinfo-5.2
../texinfo-5.2/configure --prefix=/home/steven/install/texinfo/5.2--enable-threads=posix 
make -j10
make check -j10 | tee QualityVerification.txt
make install
```

### Quality verification
See the "QualityVerification.txt" for the output of "make check".