all: tp2_video1.pgr tp2_video2.pgr

CC=gcc
CFLAGS= -I./libvideo/ -I. -I/usr/include
LDFLAGS= -L./opencv2/core -L./libvideo/ -lvideo -lopencv_highgui -lopencv_core -lm




%.pgr: %.o
	$(CC) $(CFLAGS) $< -o $@  $(LDFLAGS)

%.o: %.c
	$(CC) $(CFLAGS)  $< -c -o $@


clean:
	rm -rf *.o *.pgr
