
CFLAGS += -Wall 
LDFLAGS += -Map $(PWD)/sample.map
CFILES = main.c 

obj-m += sample.o
sample-objs := $(CFILES:.c=.o)

all:
		make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules

clean:
		make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean

