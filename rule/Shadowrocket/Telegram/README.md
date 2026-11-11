# 🧸 Telegram

## 规则说明

本目录基于 [blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Shadowrocket/Telegram) 的 Telegram 规则整理，并补充了用户提供的域名及 IP 段。

## 规则统计

本仓库当前两个规则文件均为 **43 条**：

| 类型 | 数量 |
| ---- | ----: |
| DOMAIN | 2 |
| DOMAIN-KEYWORD | 1 |
| DOMAIN-SUFFIX | 23 |
| IP-ASN | 5 |
| IP-CIDR | 7 |
| IP-CIDR6 | 5 |
| **TOTAL** | **43** |

## 文件区别

- `Telegram.list`：IP 规则带 `no-resolve`。
- `Telegram_Resolve.list`：IP 规则不带 `no-resolve`。
- Shadowrocket 中通常二选一引用，不要同时引用。

## OpenBox 导入提示

OpenBox 当前显示 **38 条**，与本文件的 43 条相差 5 条；这 5 条正好是 `IP-ASN` 规则。说明 OpenBox 导入时很可能没有计入或不支持这类规则。域名和 IP-CIDR/IP-CIDR6 规则仍保留，不建议为了凑数量而删除或改写有效规则。

如果 OpenBox 后续版本支持 `IP-ASN`，可再单独验证这 5 条是否能导入。

## 上游来源

- [Telegram.list](https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Telegram/Telegram.list)
- [Telegram_Resolve.list](https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Telegram/Telegram_Resolve.list)
- [上游目录](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Shadowrocket/Telegram)
