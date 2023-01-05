# Pandavan
modprobe xt-HL
iptables -t mangle -A POSTROUTING -j TTL --ttl-set 65
iptables -t mangle -A PREROUTING -j TTL --ttl-set 65
