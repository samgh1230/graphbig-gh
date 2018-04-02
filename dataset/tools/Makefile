CXX=g++ -std=gnu++11
CXXFLAGS=-O3 

EXECUTABLE=randgen
SOURCES=$(addsuffix .cpp, $(EXECUTABLE))

all: $(SOURCES) $(EXECUTABLE)

$(EXECUTABLE): $(SOURCES) 
		$(CXX) $(CXXFLAGS) $@.cpp -o $@

run: $(SOURCES) $(EXECUTABLE)
	./randgen 1000 10000 > id.rand

clean:
	@rm -rf $(EXECUTABLE) *.o id.rand
