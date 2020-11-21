# uofa-parsons-backends
Currently, the backends for uofa-parsons package are basically based on python tutor backends.

# Prepare system environment( tested on Ubuntu 18.04 LTS )
```
sudo apt install -y apt-transport-https ca-certificates curl software-properties-common
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
sudo apt update
sudo apt install -y docker-ce
sudo apt-get install -y build-essential make gcc-4.8
```

# Build C/C++ backends

```
export CC=gcc-4.8
make all
```

# Test
```
python run_cpp_backend.py "int main() {int x=12345;}" c

```
