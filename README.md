# Usage

```
  my-direct:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/my-direct.yml"
    path: ./ruleset/my-direct.yaml
    interval: 86400
    
  my-proxy:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/my-proxy.yml"
    path: ./ruleset/my-proxy.yaml
    interval: 86400
    
  my-reject:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/my-reject.yml"
    path: ./ruleset/my-reject.yaml
    interval: 86400

  my-chatgpt:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/chatgpt.yml"
    path: ./ruleset/chatgpt.yml
    interval: 86400
```


```
rules:
  - RULE-SET,my-direct,DIRECT
  - RULE-SET,my-proxy,PROXY
  - RULE-SET,my-reject,REJECT
  - RULE-SET,my-chatgpt,Chatgpt
```
