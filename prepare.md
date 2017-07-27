## in ubuntu 17.04
### install some packages
```
sudo apt install z3 python-z3 fuse libfuse-dev python-fuse
```

### install cpython
```
pip install Cython --install-option="--no-cython-compile"
export PATH=$PATH:~/.local/bin
cd ~/.local/bin
ln -s cython cypthon2
ln -s cythonize cythonize2
```

### try it
```
make all prod   //compile success
python2 yav_xv6_main.py -o max_read=4096 -o max_write=4096 -s a -- /dev/sXX //mount failed
make verify     // verify failed
```

