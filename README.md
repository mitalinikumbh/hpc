openmp running:- cat > filename.cpp
                 g++ -o filename -fopenmap filename.cpp
                 ./filename

cuda:-  %%writefile filename.cpp
        %%script bash
        g++ -fopenmp filename.cpp -o filename
        !./filename
