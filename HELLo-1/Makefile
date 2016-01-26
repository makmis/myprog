CC=gcc
DESTDIR=/usr/local/bin
VER=0.1
TARGET=hello-myprog

$(TARGET): *.c
	$(CC) -o $(TARGET) *.c

install:
	@install $(TARGET) $(DESTDIR)

uninstall: 
	@rm $(DESTDIR)/$(TARGET)

distrib:
	tar -czf $(TARGET)-$(VER).tar.gz *.c Makefile* configure.ac

clean:
	rm -rf autom4te.cache config.status config.log configure $(TARGET)
