```
Follow installation instaructions on dev.px4.io
Install mavros
git clone https://github.com/PX4/Firmware
cd Firmware
make posix_sitl_lpe gazebo_iris_opt_flow
```

```
in posix_configs/SITL/init/lpe/iris_opt_flow
comment out gpssim start
comment out param set LPE_GPS_ON 0 {no  longer available in newer firmware}
param set LPE_FUSION 242
param set LPE_FAKE_ORIGIN 1
```
