# 审核记录：GPT 充值银行卡被拒

审核日期：2026-05-10

审核对象：

- `_working/ready-to-publish/gpt-chongzhi-yinhangka-bei-ju/draft/article.md`
- `_working/ready-to-publish/gpt-chongzhi-yinhangka-bei-ju/source/article.html`

## 规则检查

1. 搜索意图边界：通过。正文聚焦“银行卡被拒后的扣款状态、重试边界和换方式”，没有扩写成价格、套餐、微信/支付宝或泛充值教程。
2. GPTC.cc 站点定位：通过。品牌、CTA、canonical、OG、JSON-LD 均使用 GPTC.cc / `https://www.gptc.cc/`，没有混用其他站点品牌。
3. 故障处理剧本：通过。前三个 H2 依次处理失败状态、无扣款排查、预授权/待处理边界；CTA 放在用户需要换方式的位置。
4. 官方事实：通过。已参考 OpenAI Help 的信用卡被拒、3DS/SCA、发卡行拦截、支持地区/发卡地、网页订阅与应用商店订阅分离等说明。
5. 避重：通过。和已发布 `chatgpt-plus-yinhangka-bei-ju` 的原因清单型结构拉开，本篇把主线改为“扣款状态与下一步动作”。
6. 内部字段隔离：通过。HTML 正文没有出现“搜索意图判断、用户当前状态、本篇解决动作、本文主线”等内部编辑字段。
7. 强承诺检查：通过。没有承诺一定成功、一定到账、官方渠道或保证退款。

## 已返修点

- 将标题从“先分清扣款、风控和下一步”收窄为“先看扣款状态再决定下一步”。
- 增加预授权、待处理、已扣款未生效三状态分流。
- 压缩卡信息/发卡行/3DS 原因解释，避免和旧文重复。
- 增加“网页订阅和应用商店订阅不是同一条账单路径”的事实边界。
- 更新 `data/search_structure_library.csv`，新增 3 条搜索素材留底。

## 审核结论

可以进入队列发布。建议保留 `data/publish_queue.csv` 的 2026-05-11 排期。
