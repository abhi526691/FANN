<b>FANN</b> </br>
The Fast Artificial Neural Network Library (FANN) is a neural network library, which implements multilayer artificial neural networks in C with support for both fully connected and sparsely connected networks. It has a Python binding that allows you to use its functionality from within Python. 


<b>We are going to install the FANN library on Ubuntu and install the Python binding</b></br>
wget http://downloads.sourceforge.net/project/fann/fann/2.1.0beta/fann-2.1.0beta.zip</br>
sudo apt-get install unzip</br>
unzip fann-2.1.0beta.zip


<b>Configure, make and install the library:</b></br>
cd fann-2.2.0/</br>
sudo apt-get install gcc make</br>
./configure</br>
make</br>
sudo make install</br>


<b>Install the Python bindings:</b></br>
cd python/</br>
sudo apt-get install g++ python-dev swig</br>
sudo python setup.py install</br>


<b>The Python files are now located in a build directory. Copy them to a place where you can use them Eg</b></br>
cd build/lib.linux-i686-2.6/pyfann/</br>
cp libfann.py ~</br>
cp _libfann.so ~</br>


<b>And finally test that Python can now work with the library</b></br>
from pyfann import libfann</br>
print(dir(libfann))</br>
