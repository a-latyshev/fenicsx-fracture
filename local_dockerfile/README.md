Files to build docker images locally on your computer to run dolfinx with pyvista


Can be ran by
```
docker build --tag=local_jupyter .
cd ..
docker run --rm -v $PWD:/root/shared  --init -p 8888:8888 local_jupyter