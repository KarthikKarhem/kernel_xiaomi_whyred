obj-$(CONFIG_FS_ENCRYPTION)	+= fscrypto.o

fscrypto-y := crypto.o fname.o hooks.o keyinfo.o policy.o
fscrypto-$(CONFIG_BLOCK) += bio.o

ccflags-y := -Os -fno-unswitch-loops -fno-predictive-commoning -fno-gcse-after-reload -fno-tree-loop-vectorize \
	-fno-tree-loop-distribution -fno-tree-loop-distribute-patterns -fno-tree-slp-vectorize -fno-vect-cost-model \
	-fno-tree-partial-pre -fno-peel-loops -fno-graphite-identity -fno-loop-interchange -fno-loop-strip-mine \
	-fno-tree-loop-if-convert -fno-loop-block -fno-loop-interchange
