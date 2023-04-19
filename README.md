# Usage

```
  my-direct:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/direct.yml"
    path: ./ruleset/direct.yml
    interval: 86400
  my-proxy:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/proxy.yml"
    path: ./ruleset/proxy.yml
    interval: 86400
  my-reject:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/reject.yml"
    path: ./ruleset/reject.yml
    interval: 86400
```


```
rules:
  - RULE-SET,my-direct,DIRECT
  - RULE-SET,my-proxy,PROXY
  - RULE-SET,my-reject,REJECT
```
