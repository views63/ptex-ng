#
# Copyright (c) 2016 Clerk Ma
#
# You may freely use, modify and/or distribute this file.
#

CC = gcc
AR = ar
CFLAGS = -c -O2 -Wno-unused-result -I. -I../../../libs/freetype2/freetype2 -Isrc

objects = \
	otfdrive.o\
	otferror.o\
	otfopen.o

libotf.a: $(objects)
	$(AR) rc libotf.a $(objects)

otfdrive.o: src/otfdrive.c
	$(CC) $(CFLAGS) src/otfdrive.c

otferror.o: src/otferror.c
	$(CC) $(CFLAGS) src/otferror.c

otfopen.o: src/otfopen.c
	$(CC) $(CFLAGS) src/otfopen.c

.PHONY: clean

clean:
	rm aptex ptex-ng *.o
