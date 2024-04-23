openmp running:- cat > filename.cpp <br/>
                 g++ -o filename -fopenmap filename.cpp <br/>
                 ./filename <br/>

cuda:-  %%writefile filename.cpp <br/>
        %%script bash <br/>
        g++ -fopenmp filename.cpp -o filename <br/>
        !./filename <br/>
