
ifneq ($(KERNELRELEASE),)

obj-m := globalmem.o

else

KERNELDIR :=/usr/src/linux-4.7
PWD := $(shell pwd)

all:
	$(MAKE) -C $(KERNELDIR) M=$(PWD) modules
clean:
	rm -f *.o *.ko *.mod.o *.mod.c  *.symverss

endif
