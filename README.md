

nodejs-gui是一个强大的Argo隧道部署工具，专为PaaS平台和游戏玩具平台设计。它支持多种代理协议（VLESS、VMess、Trojan等），并集成了哪吒探针功能。

docker pull ghcr.io/baggio1024/mynode:latest


const ARGO_DOMAIN = process.env.ARGO_DOMAIN || '';          // 固定隧道域名,留空即启用临时隧道
const ARGO_AUTH = process.env.ARGO_AUTH || '';              // 固定隧道密钥json或token,留空即启用临时隧道,json获取地址：https://json.zone.id
const NAME = process.env.NAME || '';    
const SUB_PATH = process.env.SUB_PATH || 'mysub';       // 订阅路径


const CFIP = process.env.CFIP || 'saas.sin.fan';            // 节点优选域名或优选ip  
const CFPORT = process.env.CFPORT || 443;                   // 节点优选域名或优选ip对应的端口
