# Usage

```
  my-direct:
    type: http
    behavior: domain
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/tld-not-cn.txt"
    path: ./ruleset/my-direct.yaml
    interval: 86400
  my-proxy:
    type: http
    behavior: domain
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/tld-not-cn.txt"
    path: ./ruleset/my-proxy.yaml
    interval: 86400
  my-reject:
    type: http
    behavior: domain
    url: "https://cdn.jsdelivr.net/gh/Loyalsoldier/clash-rules@release/tld-not-cn.txt"
    path: ./ruleset/my-reject.yaml
    interval: 86400
```


```
rules:
  - RULE-SET,my-direct,DIRECT
  - RULE-SET,my-proxy,PROXY
  - RULE-SET,my-reject,REJECT
```