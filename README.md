# Description
PoC Virtual Environment for Jupyter Remote Mode

## Steps

**STEP01**: create a virtual Python environment called avib:

```shell
python3 -m venv avib
```

**STEP02**: activate the python virtual environment:

```shell
source avib/bin/activate                                      
```

**STEP03**: install python dependencies inside the virtual python environment activated

```shell
pip3 install numpy
pip3 install pandas
pip3 install matplotlib
pip3 install jupyter
```

**STEP04**: start jupyter in remote mode, where ip is your local internal ip

```shell
jupyter notebook --no-browser --ip="192.168.0.250" --port=8888
```

**STEP05**: deactivate the virtual environment:

```shell
deactivate
```

Open the remote Jupyter url in port configured when stat the server:

```shell
http://192.168.0.250:8888/notebooks/samples/matplotlib.ipynb

```

![Remote Jupyter](captures/Remote_Jupyter.png "Remote Jupyter")
