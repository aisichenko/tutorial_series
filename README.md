# Welcome to the OCPI lab automation tutorial series

Step 1. Get the repository onto your computer!

Because of security reasons, we use the UCSB organization. Because of the Single-Sign-On authentification, we have to do an extra step: setting up an SSH key for your computer.

We only need to do this once for every computer. Carefully follow these steps:

1. Go to your Github profile icon and select **Settings**.

2. Select **SSH and GPG keys**.

3. Click **New SSH key**. 

4. For **Title**, enter the name of your computer, such as andrei_macbook_air. Something specific to your computer.

5. For the **Key**, now that's the hard part - generating the SSH key. We'll do it once and that's it. Here's how.

6. 

  a. On Windows:

    * Open Git Bash and type `ssh-keygen -t rsa`
    * Press enter when it says Enter file...
    * No need for passphrase, press enter. Press enter again when prompted.
    * Type `cat ~/.ssh/id_rsa.pub`
    * Copy the output and paste in the Github "Key" box. Click **Add SSH key**. 

  b. On Mac

    * Open Terminal and type `ssh-keygen -t rsa -b 4096 -C "aisichenko@ucsb.edu"` using your email.
    * Press enter when it says Enter file...
    * No need for passphrase, press enter. Press enter again when prompted.
    * Type `pbcopy < ~/.ssh/id_rsa.pub` which will automatically copy the key. Paste it in the Github "Key" box. Click to **Add SSH key**.

7. Under Enable SSO, below your should see a button that says "Authorize" for the ucsb organization, click this. That's it.

To clone any repository in ucsb organization (and therefore in the ocpi team), type:

```
git clone git@github.com:ucsb/tutorial_series.git  
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
