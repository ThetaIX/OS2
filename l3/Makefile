
obj-m += tsu_module.o
PWD := $(shell pwd)
KERNELDIR := /lib/modules/$(shell uname -r)/build

#KERNELDIR ?= /nix/store/xghkfwzs1zg3921qhhlzjpqq4cmczaf8-linux-6.6.64-dev/lib/modules/6.6.64/build

all:
  make -C $(KERNELDIR) M=$(PWD) modules

clean:
  make -C $(KERNELDIR) M=$(PWD) clean
