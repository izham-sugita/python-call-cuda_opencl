This work is based from the blog:
http://bikulov.org/blog/2013/10/01/using-cuda-c-plus-plus-functions-in-python-via-star-dot-so-and-ctypes/

Special thanks to Dmitry Bikulov!

I added the functions inside list_devices.cpp into the sample Python script.
list_devices.cpp contains code for listing all OpenCL devices on your platform. The code used Boost.Compute 
library, which is absolutely awesome!!

To use the examples, just compile the cpp codes to .so file.
$g++ -fPIC -shared helloworld.cpp -o helloworld.so
$g++ -fPIC -shared -I /usr/where/yourBoost.Computer list_devices.cpp -o list_devices -lOpenCL


