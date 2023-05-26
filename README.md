# Usage

```
  my-direct:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/my-direct.yaml"
    path: ./ruleset/my-direct.yaml
    interval: 86400
    
  my-proxy:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/my-proxy.yaml"
    path: ./ruleset/my-proxy.yaml
    interval: 86400
    
  my-reject:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/my-reject.yaml"
    path: ./ruleset/my-reject.yaml
    interval: 86400
   
  ChatGPT:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/bakasine/clash-rule/master/chatgpt.yaml"
    path: ./ruleset/chatgpt.yaml
    interval: 86400

```


```
rules:
  - RULE-SET,my-direct,DIRECT
  - RULE-SET,my-proxy,PROXY
  - RULE-SET,my-reject,REJECT
```
