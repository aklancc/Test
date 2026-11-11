# 🧸 Telegram

## 规则说明

本目录基于 [blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Shadowrocket/Telegram) 的 Telegram 规则整理，并补充了用户提供的域名及 IP 段。

## 规则统计

本仓库当前两个规则文件均为 **42 条**：

| 类型 | 数量 |
| ---- | ----: |
| DOMAIN | 2 |
| DOMAIN-KEYWORD | 1 |
| DOMAIN-SUFFIX | 23 |
| IP-ASN | 5 |
| IP-CIDR | 7 |
| IP-CIDR6 | 4 |
| **TOTAL** | **42** |

## 文件区别

- `Telegram.list`：IP 规则带 `no-resolve`。
- `Telegram_Resolve.list`：IP 规则不带 `no-resolve`。
- Shadowrocket 中通常二选一引用，不要同时引用。

## OpenBox 导入提示

OpenBox / sing-box 不支持 `IP-ASN` 规则，因此会忽略 5 条 IP-ASN 项。当前文件共 42 条，导入 OpenBox 后预计显示 **37 条**。这是规则类型兼容性差异，不代表其他规则丢失。

IPv6 网段已统一使用 `IP-CIDR6`。另外，`2001:b28:f23d::/48` 已由 `2001:b28:f23c::/47` 覆盖，因此已去除重复项。

## 上游来源

- [Telegram.list](https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Telegram/Telegram.list)
- [Telegram_Resolve.list](https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Telegram/Telegram_Resolve.list)
- [上游目录](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Shadowrocket/Telegram)
