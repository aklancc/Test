# 🧸 Telegram

## 规则说明

本目录基于 [blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Shadowrocket/Telegram) 的 Telegram 规则整理，并补充了用户提供的域名及 IP 段。

## 规则统计

本仓库当前两个规则文件均为 **44 条**：

| 类型 | 数量 |
| ---- | ----: |
| DOMAIN | 2 |
| DOMAIN-KEYWORD | 1 |
| DOMAIN-SUFFIX | 23 |
| IP-ASN | 5 |
| IP-CIDR | 9 |
| IP-CIDR6 | 4 |
| **TOTAL** | **44** |

## 文件区别

- `Telegram.list`：IP 规则带 `no-resolve`。
- `Telegram_Resolve.list`：IP 规则不带 `no-resolve`。
- Shadowrocket 中通常二选一引用，不要同时引用。

## 官方 IP 网段核对

已对照 [Telegram 官方公布的 CIDR 列表](https://core.telegram.org/resources/cidr.txt)，补充此前缺少的两个 IPv4 网段：

- `91.105.192.0/23`
- `185.76.151.0/24`

现有 `91.108.0.0/16` 已覆盖官方列出的多个 `91.108.*` 子网；现有 IPv6 网段也覆盖官方列表中的部分子网，因此没有重复添加。

## OpenBox 导入提示

这两个文件是 Shadowrocket 规则格式。OpenBox 对 `IP-ASN` 等规则类型的导入支持可能与 Shadowrocket 不同，实际显示条数应以 OpenBox 导入结果和日志为准，不应仅按文件总行数推算。

IPv6 网段已统一使用 `IP-CIDR6`。另外，`2001:b28:f23d::/48` 已由 `2001:b28:f23c::/47` 覆盖，因此已去除重复项。

## 上游来源

- [Telegram.list](https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Telegram/Telegram.list)
- [Telegram_Resolve.list](https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Telegram/Telegram_Resolve.list)
- [上游目录](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Shadowrocket/Telegram)
