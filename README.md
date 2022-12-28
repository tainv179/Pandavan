# Pandavan

  iptables -t mangle -A POSTROUTING -j TTL --ttl-set 65
  iptables -t mangle -A POSTROUTING -o weth0 -j TTL --ttl-set 65
  iptables -t mangle -A PREROUTING -i weth0 -j TTL --ttl-set 65
  
  WAN no -ttl
