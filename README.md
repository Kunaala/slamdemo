# slamdemo
## from hostmachine to send time over PTP
## -S for software timestamping

sudo ptp4l -i <interface name eg.enp0s31f6> -m   

## from host machine through nc <hostname> 7501 to test if timestamp_mode is from PTP
get_config_param 

set_config_param timestamp_mode TIME_FROM_PTP_1588  
## to reinitialize after settings
reinitialize         
