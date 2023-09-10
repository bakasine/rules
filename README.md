# Usage

## clash

```
proxy-groups:
  - name: "CHATGPT"
    type: select
    proxies:
      - YOUR_PROXY

  - name: "Bilibili"
    type: select
    proxies:
      - YOUR_PROXY

rule-providers:
  bilibili:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/bakasine/rules/master/clash/bilibili.yaml"
    path: ./ruleset/bilibili.yaml
    interval: 86400 
 
  my-direct:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/bakasine/rules/master/clash/my-direct.yaml"
    path: ./ruleset/my-direct.yaml
    interval: 86400
    
  my-proxy:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/bakasine/rules/master/clash/my-proxy.yaml"
    path: ./ruleset/my-proxy.yaml
    interval: 86400
    
  my-reject:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/bakasine/rules/master/clash/my-reject.yaml"
    path: ./ruleset/my-reject.yaml
    interval: 86400
   
  ChatGPT:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/bakasine/rules/master/clash/chatgpt.yaml"
    path: ./ruleset/chatgpt.yaml
    interval: 86400

  MIUI:
    type: http
    behavior: classical
    url: "https://raw.githubusercontent.com/bakasine/rules/master/clash/miui.yaml"
    path: ./ruleset/miui.yaml
    interval: 86400

rules:
  - RULE-SET,bilibili,Bilibili
  - RULE-SET,my-direct,DIRECT
  - RULE-SET,my-proxy,PROXY
  - RULE-SET,my-reject,REJECT
  - RULE-SET,ChatGPT,CHATGPT
  - RULE-SET,MIUI,REJECT
```

## Quantumult X

```
[policy]
static=CHATGPT, YOUR_PROXY, YOUR_PROXY2
[filter_remote]
https://raw.githubusercontent.com/bakasine/rules/master/quantumultx/direct.list, tag=my-direct, update-interval=43200, enabled=true
https://raw.githubusercontent.com/bakasine/rules/master/quantumultx/proxy.list, tag=my-proxy, update-interval=43200, enabled=true
https://raw.githubusercontent.com/bakasine/rules/master/quantumultx/reject.list, tag=my-reject, update-interval=43200, enabled=true
https://raw.githubusercontent.com/bakasine/rules/master/quantumultx/chatgpt.list, tag=chatgpt, update-interval=43200, enabled=true, force-policy=CHATGPT

```
