# 🧸 Telegram

## 前言

Telegram 规则由《RULE GENERATOR 规则生成器》自动生成。

分流规则是互联网公共服务的域名和 IP 地址汇总，所有数据均收集自互联网公开信息。

## 规则统计

最后更新时间：2025-09-10 02:08:26

| 类型 | 数量 |
| ---- | ----: |
| DOMAIN | 2 |
| DOMAIN-KEYWORD | 1 |
| DOMAIN-SUFFIX | 22 |
| IP-ASN | 5 |
| IP-CIDR | 10 |
| TOTAL | 40 |

## Shadowrocket 使用说明

- `Telegram.list`：使用 `RULE-SET`。
- `Telegram_Resolve.list`：使用 `RULE-SET`。
- 两个文件的区别是 `Telegram.list` 的 IP-CIDR 规则带 `no-resolve`；`Telegram_Resolve.list` 不带。
- 建议二选一单独使用，不要同时引用。

## 上游规则

- [Telegram.list](https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Telegram/Telegram.list)
- [Telegram_Resolve.list](https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Telegram/Telegram_Resolve.list)
- [上游目录](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Shadowrocket/Telegram)
