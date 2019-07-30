# pmon-ls1x
pmon for loongson1 cpu, such as loongson 1a/1b/1c

# toolchain:
http://ftp.loongnix.org/toolchain/gcc/release/CROSS_COMPILE/gcc-4.4.0-pmon.tgz

# compile:
	# first make pmoncfg
	cd tools/pmoncfg
	make
	cp pmoncfg /usr/bin
		
	# make pmon	
	cd zloader.${targetboard}
	make cfg
	make tgt=rom
