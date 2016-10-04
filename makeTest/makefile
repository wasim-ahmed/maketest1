
VPATH = src1;src2

all:test.exe

test.exe:test.o test1.o test2.o
	g++ -o test.exe test.o test1.o test2.o

test.o:test.cpp
	g++ -c $^ -I /makeTest
	
test1.o:test1.cpp
	g++ -c $^
	
test2.o:test2.cpp
	g++ -c $^
	
clean:
	del test.exe test.o test1.o test2.o
	$(info cleaning)