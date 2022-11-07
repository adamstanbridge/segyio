# segyio #

Modified segyio to work with REV 2 little-endian files

## Building ##

mkdir build
cd build
cmake .. -DCMAKE_BUILD_TYPE=Release -DBUILD_SHARED_LIBS=ON -DPYTHON_EXECUTABLE=/usr/bin/python3
make

## Minimum install ##

Install instructions specific to my environment!

cd build
sudo cp lib/libsegyio.so.0 /usr/local/lib
sudo ldconfig

cd ../python
sudo cp -r segyio /usr/local/lib/python3.8/dist-packages/
