# Pandavan

  iptables -t mangle -A POSTROUTING -j TTL --ttl-set 65
  iptables -t mangle -A POSTROUTING -o weth0 -j TTL --ttl-set 64
  iptables -t mangle -A PREROUTING -o weth0 -j TTL --ttl-set 64
  
  WAN no -ttl
