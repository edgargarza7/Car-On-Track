# How to Install Tensorflow on your AutoAuto Device

### For AutoAuto Fleet 1 Car

![AutoAuto Fleet 1 Car](https://autoauto-static-uploads.s3.amazonaws.com/d452293bcac14e65a3370c54e9027e79.JPG)

You first must SSH into your car to gain privileged access. On your [device page](https://labs.autoauto.ai/autopair/) click the yellow `i` button to see your device's "Info for Advanced Users". There you will find details for how to SSH into your device.

After you have gained SSH access, you can run the following commands on your device. Copy-paste each command into your SSH session to run the command on your device.

The following creates a new conda python environment with the required packages:
```bash
conda create --name tensorflow \
  python=3.5 \
  ipykernel=4.9.0 \
  h5py=2.7.1 \
  scipy=1.0.0 \
  pandas=0.23.4 \
  opencv=3.3.0 \
  matplotlib=2.1.2 \
  scikit-learn=0.19.2
```

Activate your new environment:
```bash
source activate tensorflow
```

Install some additional packages via `pip`:
```bash
pip install rpyc
```

Register your new environment so that it shows up in Jupyter:
```bash
sudo `which python` -m ipykernel install --name 'Python3.5_Tensorflow'
```

Finally, install Tensorflow:
```bash
pip install https://github.com/lhelontra/tensorflow-on-arm/releases/download/v1.12.0/tensorflow-1.12.0-cp35-none-linux_armv7l.whl
```

And reboot your device:
```bash
sudo reboot
```

After your device reboots, you will be ready to write & run programs that use Tensorflow.
