# Overview of A Template Library

## Setting up repo

```bash
./bin/convert-repo "Your New Library" 3.2.1 2024-12-30 "Andy Curtis" "contactandyc@gmail.com" "linkedin.com/in/andycurtis"
```

Make sure to remove the .git and recreate your own repo
```bash
rm -rf .git
git init
git add .
```

## Building

### Build and Install
```bash
mkdir -p build
cd build
cmake ..
make
sudo make install
```

### Uninstall
```bash

```

### Build Tests and Test Coverage
```bash
mkdir -p build
cd build
cmake BUILD_TESTING=ON ENABLE_CODE_COVERAGE=ON ..
make
ctest
make coverage
```

