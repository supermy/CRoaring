#### 20211130


    For C, try:
    cc -march=native -O3 -std=c11  -o amalgamation_demo amalgamation_demo.c  && ./amalgamation_demo 

    For C++, try:
    c++ -march=native -O3 -std=c++11 -o amalgamation_demo amalgamation_demo.cpp  && ./amalgamation_demo 

    You can build a shared library with the following command:
    cc -march=native -O3 -std=c11 -shared -o libroaring.dylib -fPIC roaring.c

    add extern "C" 
    g++ -march=native -O3 -std=c++11 -shared -o libroaring++.dylib -fPIC cpp/roaring64map.hh 
    cp libroaring++.dylib /usr/local/lib/
