src = $(wildcard ./*.cpp)
obj = $(patsubst %.cpp,%.o,$(src))
#obj = $(src:%.cpp=%.0)
target = app
xx = g++

$(target):$(obj)
	$(xx) $(obj) -o $(target)

%.o:%.cpp
	$(xx) -c $< -o $@

.PHONY:clean
clean:
	rm -rf $(obj) $(target)
