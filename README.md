# Pandavan
modprobe xt-HL
iptables -t mangle -A POSTROUTING -j TTL --ttl-set 65
iptables -t mangle -A PREROUTING -j TTL --ttl-set 65


/sbin/.magisk/img/.core/service.d
chmod +x your-script.sh

#!/system/bin/sh
# This script will be executed in post-fs-data mode

# Run the commands to set TTL to 64
iptables -t mangle -A POSTROUTING -j TTL --ttl-set 64
ip6tables -t mangle -A POSTROUTING -j TTL --ttl-set 64
