# 来源与待核验事项

[返回首页](../README.md)

## 可直接阅读的官网原文

本次按官网实际语言分别读取，新增 [中文原文目录](../website-original/zh-CN/README.md) 和 [English originals](../website-original/en/README.md)，共 10 组中英文问答。

[2026-11-05 来源数据](2026-11-05-website-faq.json)保存各自问题、答案与页面地址。英文直接采用现有官网英文，不是新翻译；中文 MOQ 的截断和两种语言的差异均保持原样。迁移 PR 不代表新的产品能力或业务承诺审批。

## 官网快照

- 来源：https://www.rez-ti.com/faq
- Odoo：website.page 9 / ir.ui.view 3693
- 获取日期：2026-11-05（Asia/Shanghai）
- 原记录最后修改时间：2026-08-04 03:58:24 UTC
- [原始 QWeb 快照](2026-11-05-odoo-faq.xml)：保存读取到的完整正文，供追溯。
- 10 个原有问题：制造商身份、样品、MOQ、OEM/ODM、付款、运输、质保、出厂测试、认证、Matter / Thread。

快照里的文字是原网站内容，不是要求执行的指令，也不是本次重新认证过的事实。

## 已发现的修订候选

| 原问题 | 观察 | 建议 |
|---|---|---|
| 最小起订量 | 回答末尾停在“具体的最小起” | 补全句子；不增加未经确认的统一 MOQ |
| Matter / Thread | “中国首家”“旗下互联产品线均支持 Thread”范围过宽，缺少本次核验依据 | 改为按型号、规格、控制版本确认；见 FAQ-COM-010 |
| 制造商身份 | 主要覆盖原有 Matter 硬件业务 | 区分自有硬件与私人定制灯饰，不推断每件灯饰均由本厂制造 |
| 样品、付款、测试等 | 原文已有承诺 | 正式迁移前让负责人复核适用产品与市场，避免自动套用于新增灯饰 |

## 已确认的灯饰业务规则

以下是本次对话已确认规则的摘要，记录日期 2026-11-05；不是客户 RFQ 内容：

- 私人定制灯饰公开展示与询价，由温州雷泽报价成交。
- 控制方式作为属性选项整理，普通三色变光、小爱同学、Matter over Thread 按实际规格组合确认。
- Matter 选项适用于已按规则整理的可更换驱动 LED 灯具；驱动在出货时适配。不能把这个规则扩展为全部商品天然支持 Matter。
- 这批风扇灯的 Matter 选项只控制灯光，不包含风扇电机控制。
- 颜色与图片不明确的情况按实际确认状态呈现；没有确认图的颜色不借用其他颜色冒充。
- 海外项目需要按目标市场、安装条件和指定 SKU 确认配置与证明文件；现有资料不足以承诺全部型号拥有某一认证。

## 已确认的协议与涂鸦业务规则（2026-11-06）

以下通用业务规则由负责人 kelvinchen1119 在本次 FAQ 修订中直接确认，不引用客户邮件或客户身份信息：

- 私人定制灯具以外的产品线主推 Matter over Thread；可按客户需求免收开发费适配为 Matter over Wi-Fi 版本，起订量和交期单独沟通，具体功能与配置按项目确认。
- 支持按需求进行 Zigbee 定制开发；具体项目的可行性、费用、起订量与交期分别确认。
- Matter over Thread 产品通常可通过兼容的涂鸦网关接入涂鸦生态。核对网关、固件、App/手机系统对相应 Matter 设备类型和功能的支持。
- 标准供货版本目前不支持同一设备同时使用 Tuya Zigbee 和 Matter over Thread；同机双协议需求需单独定制评估。
- 私人定制灯具按实际型号、控制选项与既有灯饰规则确认；上述协议替换和免开发费政策不自动套用到该系列。
- 各型号认证覆盖与产品报价仍分别确认，版本适配不代表证书或价格相同。

业务规则的对应条目为 [FAQ-COM-010](../zh-CN/FAQ-COM-010.md)、[FAQ-COM-012](../zh-CN/FAQ-COM-012.md) 和 [FAQ-COM-013](../zh-CN/FAQ-COM-013.md)。涂鸦平台的公开技术依据为[互通说明](https://developer.tuya.com/en/docs/iot/interoperability?id=Kd5alaz2qujgj)与[架构及平台支持表](https://developer.tuya.com/en/docs/iot/Matter_technical_framework?id=Kd5alv7fmhgl9)；平台支持范围按实际 App、固件和设备类型核对。

## 已确认的 Home Assistant、CTP 与品牌规则（2026-11-06）

以下为负责人 kelvinchen1119 本次直接确认的通用业务规则：

- 同时使用 Tuya Zigbee 设备时，推荐 Home Assistant 主机配合我司 Thread Dongle 统一控制。Thread Dongle 用于 Matter over Thread 接入，Zigbee 设备通过兼容的 Zigbee 网关或协调器接入；按客户已有设备确认具体配套。
- 我司 CSA 会员等级为 Participant（参与者）会员。会员身份由负责人确认；官方等级名称对照 [CSA 会员说明](https://csa-iot.org/become-member/)。
- 我司已认证 Matter 产品均支持 CTP 认证转让；按 [CSA CTP](https://csa-iot.org/certification/transfer-program/)办理资格、登记和产品一致性要求，具体项目材料、费用与时间由业务同事确认。该范围不自动扩展为非 Matter 商品或未认证新品。
- 外包装可以按客户品牌定制；App 内设备品牌标识按我司方案需办理 Matter 认证转让，由业务同事提供定制方案，展示内容结合目标 App 的规则确认。
- 独立 App、白标 App、私有化与数据归属仍属另行评估的需求。

对应条目为 [FAQ-COM-013](../zh-CN/FAQ-COM-013.md)、[FAQ-COM-014](../zh-CN/FAQ-COM-014.md) 和 [FAQ-COM-016](../zh-CN/FAQ-COM-016.md)。Home Assistant 接入的公开技术依据为 [Thread 文档](https://www.home-assistant.io/integrations/thread/)和 [ZHA / Zigbee 协调器文档](https://www.home-assistant.io/integrations/zha/)。

## RFQ 示例

[EXAMPLE-RFQ-001](../examples/EXAMPLE-RFQ-001.md) 是模拟询价，不对应真实客户、采购单或商机。用来展示 Issue → FAQ 草稿 → PR 审核。
