# neovim-build
neovim-basic
building and running neovim on most platforms

clone neovim from github

git clone https://github.com/neovim/neovim.git

```cd neovim
```
(optional checkout the latest stable version)

```
git tag
```

```
mkdir .deps

mkdir build

cd .deps

cmake -G Ninja -DCMAKE_BUILD_TYPE=Release ../cmake.deps/

ninja

cd ..

cd build

cmake -G Ninja -DCMAKE_BUILD_TYPE=Release ..

ninja

sudo ninja install #or gsudo for windows or will need to run ninja install in the build directory from an elevated permission ie superuser or admin account
```
