.SUFFIXES: .c .o

COMPILE = $(CC) -g -O1 -Wall -D_FILE_OFFSET_BITS=64 -g -DDEBUG_FLAG
INC_PATH = -I/usr/include/fastcommon
LIB_PATH = -lfastcommon

ALL_PRGS = test_allocator test_skiplist test_multi_skiplist test_mblock test_blocked_queue

all: $(ALL_PRGS)
.c:
	$(COMPILE) -o $@ $< $(LIB_PATH) $(INC_PATH)
.c.o:
	$(COMPILE) -c -o $@ $<  $(INC_PATH)
clean:
	rm -f $(ALL_PRGS)

