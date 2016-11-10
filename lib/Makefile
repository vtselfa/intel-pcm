# Copyright (c) 2014 Intel Corporation

all: libpcm.a

CXXFLAGS+= -Wall -O3 -std=c++0x -Wno-unknown-pragmas
vpath %.cpp ..

libpcm.a: msr.o cpucounters.o pci.o client_bw.o utils.o
	ar rcs $@ $^

clean:
	rm -rf *.a *.o


