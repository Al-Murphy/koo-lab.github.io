# Server Management
<br>

#### VPN using Ubuntu 
$ sudo openfortivpn vpn.cshl.edu:443 -u \[username\] --trusted-cert \[token\]
<br>
<br>

#### ssh to server
$ ssh \[username\]@\[server-ip\]
<br>
<br>


#### Jupyter notebook

_Terminal on remote machine_

$ jupyter notebook --no-browser --port=8080

_Terminal on local machine_

$ ssh -N -L 8080:localhost:8080 \[username\]@\[server-ip\]

_Browser on local machine (need token from jupyter notebook on remote machine)_

$ localhost:8080 
<br>
<br>

#### GPU management

_Check processes on gpu_

$ nvidia-smi

_kill process on gpu_

$ sudo kill -9 \[PID\]

_Run a job on a specific GPU_

$ CUDA_VISIBLE_DEVICES=\[gpu\] python3 \[script.py\]
<br>
<br>

#### Setup environment for Tensorflow-gpu with cuda and cudnn

Using [pip](https://towardsdatascience.com/installing-nvidia-drivers-cuda-10-cudnn-for-tensorflow-2-1-on-ubuntu-18-04-lts-f1db8bff9ea)
or [anaconda](https://towardsdatascience.com/tensorflow-gpu-installation-made-easy-ubuntu-version-4260a52dd7b0)

<br>
<br>
<br>
<br>
