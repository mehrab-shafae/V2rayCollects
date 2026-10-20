# V2RayCollects

[![Collect](https://github.com/mehrab-shafae/V2rayCollects/actions/workflows/Collector.yml/badge.svg)](https://github.com/mehrab-shafae/V2rayCollects/actions/workflows/Collector.yml)

## Introduction

The automation functions of this repository are all implemented based on `GitHub Actions`

Test the speed of each free node pool on the network and the nodes shared by bloggers to screen out relatively stable and high-speed nodes, and then import them into the warehouse for sharing records.

The speed measurement function is implemented in the `GitHub Actions` environment using [LiteSpeedTest](https://github.com/xxf098/LiteSpeedTest), so there are many nodes in the United States, which cannot well represent the node availability in the domestic network environment.

## 🚀 Usage

You can use the generated subscription links directly in your favorite proxy client. Copy the URL of the desired configuration, then add it as a remote subscription in your client.

### 🔹 V2Ray / Xray Subscription

| Output | Link |
|---|---|
| All nodes (Base64 subscription) | [Eternity.txt](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/Eternity.txt) |
| Raw node list | [EternityBase](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/EternityBase) |

### 🔹 Clash / Clash Meta

| Output | Link |
|---|---|
| Clash YAML configuration | [Eternity.yml](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/Eternity.yml) |
| Combined provider configuration | [provider-all.yml](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/update/provider/provider-all.yml) |

### 🔹 Merged Subscriptions

| Output | Link |
|---|---|
| Merged Base64 subscription | [sub_merge_base64.txt](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/sub_merge_base64.txt) |
| Merged YAML configuration | [sub_merge_yaml.yml](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/sub_merge_yaml.yml) |

### 🔹 Protocol-Specific Subscriptions

Prefer a subscription containing only a specific proxy protocol? Use the links below to import individual node lists.

| Protocol | Subscription |
|---|---|
| VMess | [VMess](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/splitted/vmess.txt) |
| VLESS | [VLESS](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/splitted/vless.txt) |
| Trojan | [Trojan](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/splitted/trojan.txt) |
| Shadowsocks | [Shadowsocks](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/splitted/ss.txt) |
| ShadowsocksR | [ShadowsocksR](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/splitted/ssr.txt) |

**How to use:** Copy the desired URL, add it as a remote subscription in your V2Ray/Xray-compatible client, and refresh it to fetch the latest nodes.

**Note:** Protocol-specific files may be empty if no working nodes of that protocol are available. These subscriptions contain public proxy nodes, whose availability and performance are not guaranteed.

### 📱 How to Use

1. Copy the subscription URL for your preferred client.
2. Open your proxy client and find **Add Subscription**, **Import from URL**, or **Remote Profile**.
3. Paste the URL and save it.
4. Update or refresh the subscription to download the latest configuration.

**Note:** These files are updated automatically by GitHub Actions. Availability and connection speed depend on the collected nodes and their providers. Public proxy nodes may be unreliable; avoid using them for sensitive traffic.

## Instructions & Usage

### Tips
- If you see an IP repeated more than once it's usually because of the different ports.
- (Group 2) Some free airports only provide 1GB of traffic or have limited time to use that's why I update the airport node every 2 hours. so if you want to use them set the auto-update option on your client to get fresh nodes.
- (Group 1) Other public nodes are more stable and will be updated every 12 hours.
- Depending on your internet provider and location, some nodes might not work.


### Ready to import (200 filtered nodes)
> Just import the following subscription link into the corresponding client. Use a client that atleast support ss + ssr + vmess + trojan.

Nodes filtered using speedtest measurement will be stored in following files:  

* Group 1 (Contains free public nodes)
- [Base64](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/Eternity)
- [Mixed](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/Eternity.txt)
- [Clash](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/Eternity.yml)

### Manual Subs Conversion
- If your client does not support the formats that provided here use below services to convert them to your client format (like surfboard)
> Services for online sub conversion: 
- [sub-web-modify](https://sub.v1.mk/)
- [bianyuan](https://bianyuan.xyz/)  

- **If you don't like the groups and rules that are already set, you can simply use bianyuan API like this::**  
> don't use this API for your personal airport subs! Pls run the subconverter locally
```
https://pub-api-1.bianyuan.xyz/sub?target=(OutputFormat)&url=(SubUrl)&insert=false

For Example:
(OutputFormat) = clash
(SubUrl) = https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/Eternity.yml

https://pub-api-1.bianyuan.xyz/sub?target=clash&url=https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/Eternity.yml&insert=false

Now you can use the link above to import the subs into your client
```

<br/>

## Node Information

### all nodes
merge nodes w/o dup: `4133`
- [Node link Mixed (V2ray)](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/sub_merge.txt)
- [Node link Yaml (Clash)](https://raw.githubusercontent.com/mahdibland/SSAggregator/master/sub/sub_merge_yaml.yml)

#### all nodes separated by protoctol
- [VMESS](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/splitted/vmess.txt)
- [TROJAN](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/splitted/trojan.txt)
- [SSR](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/splitted/ssr.txt)
- [SHADOWSOCKS](https://raw.githubusercontent.com/mehrab-shafae/V2rayCollects/master/sub/splitted/ss.txt)

### node sources
- [pojiezhiyuanjun/freev2](https://github.com/pojiezhiyuanjun/freev2), number of nodes: `66`
- [mahdibland/ShadowsocksAggregator](https://github.com/mahdibland/ShadowsocksAggregator), number of nodes: `200`
- [iwxf/free-v2ray](https://github.com/iwxf/free-v2ray), number of nodes: `39`
- [DoveBoy/Vmess-Actions](https://github.com/ldir92664/Vmess-Actions), number of nodes: `105`
- [gooooooooooooogle/Clash-Config](https://github.com/gooooooooooooogle/Clash-Config), number of nodes: `1`
- [ermaozi/get_subscribe](https://github.com/ermaozi/get_subscribe), number of nodes: `167`
- [wrfree/free](https://github.com/wrfree/free), number of nodes: `51`
- [anaer/Sub](https://github.com/anaer/Sub), number of nodes: `348`
- [Pawdroid/Free-servers](https://github.com/Pawdroid/Free-servers), number of nodes: `1`
- [misersun/config003-002](https://github.com/misersun/config003), number of nodes: `217`
- [mfuu/v2ray](https://github.com/mfuu/v2ray), number of nodes: `85`
- [freefq/free](https://github.com/freefq/free), number of nodes: `14`
- [xiyaowong/freeFQ](https://github.com/xiyaowong/freeFQ), number of nodes: `156`
- [YasserDivaR/pr0xy](https://github.com/YasserDivaR/pr0xy), number of nodes: `621`
- [peasoft/NoMoreWalls](https://github.com/peasoft/NoMoreWalls), number of nodes: `122`
- [mahdibland/get_v2](https://github.com/mahdibland/get_v2), number of nodes: `2353`
- [jikelonglie/meskell](https://github.com/jikelonglie/meskell), number of nodes: `9`
- [freebaipiao/freebaipiao](https://github.com/freebaipiao/freebaipiao), number of nodes: `6`
- [MOnday9907/v2ray](https://github.com/MOnday9907/v2ray), number of nodes: `8`
- [adminaliang/v2ray](https://github.com/adminaliang/v2ray), number of nodes: `16`
- [Jia-Pingwa/free-v2ray-merge](https://github.com/Jia-Pingwa/free-v2ray-merge), number of nodes: `327`
- [Lewis-1217/FreeNodes](https://github.com/Lewis-1217/FreeNodes), number of nodes: `39`
- [jiang.netlify.app](https://jiang.netlify.app), number of nodes: `63`
- [learnhard-cn/free_proxy_ss](https://github.com/learnhard-cn/free_proxy_ss), number of nodes: `116`
- [SnapdragonLee/SystemProxy](https://github.com/SnapdragonLee/SystemProxy), number of nodes: `232`
- [hermanb001/ProxyTest](https://github.com/hermanb001/ProxyTest), number of nodes: `1743`
- [LonUp/NodeList](https://github.com/LonUp/NodeList), number of nodes: `1451`

## Softwares

### Credit: 
- [alanbobs999](https://github.com/alanbobs999)
- [PersianBlocker](https://github.com/MasterKia/PersianBlocker)
- [iran-hosted-domains](https://github.com/bootmortis/iran-hosted-domains)
