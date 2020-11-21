# uofa-parsons-backends(C/C++)
Currently, the backends(C/C++) for uofa-parsons package are basically based on python tutor backends.

# Preparing system environment(tested on Ubuntu 18.04 LTS)
```sh
sudo apt install -y apt-transport-https ca-certificates curl software-properties-common
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
sudo apt update
sudo apt install -y docker-ce
sudo apt-get install -y build-essential make gcc-4.8
sudo apt install nodejs

```

# Building C/C++ backends

```sh
export CC=gcc-4.8
make all
```

# Running HTTP server
```bash
# listening on 3000 when `local` given
node cokapi.js local
```

# Testing
```bash
python run_cpp_backend.py "int main() {int x=12345;}" c

```
# Reference
[The original backends in python tutor project](https://github.com/LearningProgramingOnline/visualization-online-python-tutor/tree/master/v4-cokapi)
