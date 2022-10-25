## Dependencies
```
# carla-simulator 0.9.10-2
https://github.com/carla-simulator/carla/releases

sudo mkdir /opt/carla-simulator
cd /opt/carla-simulator
sudo tar -xvf ~/Downloads/CARLA_0.9.10.1.tar.gz -C ./

# libflann 1.9.1
sudo apt install -y libflann1.9

# libboost 1.65.1
sudo apt install -y libboost1.65-all-dev

# VTK 6.3
sudo apt install -y libvtk6-dev libvtk6-qt-dev

# libpcl 1.8.1
sudo apt-get install -y libpcl-dev

```

```
cd /home/workspace/c3-project
cmake .
make
```

```
su - student // Ignore Permission Denied, if you see student@ you are good
cd /home/workspace/c3-project
./run_carla.sh
// Create new tab
cd /home/workspace/c3-project
./cloud_loc // Might have core dump on start up, just rerun if so. Crash doesn't happen more than a couple of times
```
