### clion将cpp工程修改为c工程
参考[How to create a C project with CLion](http://stackoverflow.com/questions/26177390/how-to-create-a-c-project-with-clion)修改CMakeLists.txt，将

```sh
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
```
替换为

```sh
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Werror")
```
然后重命名main.cpp为main.c
