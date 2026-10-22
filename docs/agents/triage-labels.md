# Triage Labels

技能以五个标准分诊角色来表述。本文件将这些角色映射到本仓库 issue tracker 中实际使用的标签字符串。

| 本技能集内的标签   | 本 tracker 中的标签  | 含义                            |
| ----------------- | -------------------- | ------------------------------- |
| `needs-triage`    | `needs-triage`       | 维护者需要评估此 issue          |
| `needs-info`      | `needs-info`         | 等待报告者补充更多信息          |
| `ready-for-agent` | `ready-for-agent`    | 任务要求完整，AFK agent 可直接开始  |
| `ready-for-human` | `ready-for-human`    | 需要人工实现                    |
| `wontfix`         | `wontfix`            | 不予处理                        |

当技能提到某个角色时（如“打上 AFK 就绪的分诊标签”），使用本表中对应的标签字符串。

编辑右列以匹配你实际使用的术语。

## 仓库状态

映射表右列的五个标签尚未在 `zhanghongfeix/dsh-wb-credits` 创建。该仓库目前只有 GitHub 默认标签，其中 `wontfix` 与上表同名同义，其余四个需要单独创建。创建需要对上游仓库有写权限：

```bash
gh label create needs-triage --repo zhanghongfeix/dsh-wb-credits --description "维护者需要评估此 issue"
gh label create needs-info --repo zhanghongfeix/dsh-wb-credits --description "等待报告者补充更多信息"
gh label create ready-for-agent --repo zhanghongfeix/dsh-wb-credits --description "任务要求完整，AFK agent 可直接开始"
gh label create ready-for-human --repo zhanghongfeix/dsh-wb-credits --description "需要人工实现"
```

在 fork `ouyangjiahong26/dsh-wb-credits` 上创建只对该 fork 生效，对上游 issue 分诊无用。
