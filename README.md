# Welcome to the OCPI lab automation tutorial series

Step 0. Get the repository onto your computer!


To clone any repository, type:

```
git clone https://github.com/aisichenko/tutorial_series
```

## 1. Git and Jupyter

- basics of Jupyter
- basics of Git (add, commit, branches, merging)
- using a remote, such as Github.com
- merging issues

## 2. Python and how to use it

- Why Python
  - modular
  - open source packages
  - many packages for instrument control: [lightlab](https://github.com/lightwave-lab/lightlab) and [pymeasure](https://github.com/ralph-group/pymeasure)
- Ways to use Python
  - Pycharm or similar IDE
  - Jupyter notebooks --> the case for lab workflow and research life cycle

## 3. Lab control

- The idea of an instrument class i.e. "driver"
  - creating "instance" of an instrument and accessing its methods and settings
  - having multiple instruments, just define by the connection address
- Example of running a lab control "take data then analyze" experiment
  - in JupyterLab
- Advanced: asynchronous control
  - one-sample testing vs. systems-control
