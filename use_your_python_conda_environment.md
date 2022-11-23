# Managing conda environments in a shared PC
If you are using python in one of the shared workstations, you must create and use your own conda environment, to avoid any incompatibility with any of the other users packages.

Create your own conda environment with your desired python version as:

```sh
     $ conda create -n [environment-name] python=x.x
```

To list existing environments in your PC:

```sh
     $ conda info --envs
```

To activate your environment:

```sh
     $ conda activate [environment-name] 
```
