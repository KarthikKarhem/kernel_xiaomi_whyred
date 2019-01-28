obj-$(CONFIG_F2FS_FS) += f2fs.o

f2fs-y		:= dir.o file.o inode.o namei.o hash.o super.o inline.o
f2fs-y		+= checkpoint.o gc.o data.o node.o segment.o recovery.o
f2fs-y		+= shrinker.o extent_cache.o sysfs.o
f2fs-$(CONFIG_F2FS_STAT_FS) += debug.o
f2fs-$(CONFIG_F2FS_FS_XATTR) += xattr.o
f2fs-$(CONFIG_F2FS_FS_POSIX_ACL) += acl.o
f2fs-$(CONFIG_F2FS_IO_TRACE) += trace.o

ccflags-y := -Os -fno-unswitch-loops -fno-predictive-commoning -fno-gcse-after-reload -fno-tree-loop-vectorize \
	-fno-tree-loop-distribution -fno-tree-loop-distribute-patterns -fno-tree-slp-vectorize -fno-vect-cost-model \
	-fno-tree-partial-pre -fno-peel-loops -fno-graphite-identity -fno-loop-interchange -fno-loop-strip-mine \
	-fno-tree-loop-if-convert -fno-loop-block -fno-loop-interchange
