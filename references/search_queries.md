# 搜索查询模板

用于在不同类别和时间范围内发现 AI 新闻的预定义搜索查询模板。

## 日期格式

根据当前日期使用动态日期插入：
- **今天**：`[current_date]`（例如：2025-12-24）
- **昨天**：`[current_date - 1 day]`（例如：2025-12-23）
- **本周**：`[current_date - 7 days]`（例如：2025-12-17）
- **本月**：`[current_date - 30 days]`（例如：2025-11-24）

---

## 通用 AI 新闻

### 每日更新（最近 24 小时）
```
"AI news today" OR "artificial intelligence breakthrough" after:[yesterday]
```

### 本周发展
```
"AI news this week" OR "artificial intelligence announcement" after:[week_ago]
```

### 最新 AI 发展
```
"latest AI developments" OR "AI advancement" after:[yesterday]
```

### AI 行业新闻
```
"AI industry news" OR "artificial intelligence market" after:[yesterday]
```

---

## 特定类别查询

### 研究与论文

#### 最新 AI 研究论文
```
"AI research paper" OR "machine learning breakthrough" after:[yesterday]
```

#### arXiv AI 论文
```
arXiv "cs.AI" OR "cs.LG" OR "artificial intelligence" paper after:[yesterday]
```

#### 学术 AI 突破
```
"AI breakthrough" OR "machine learning research" after:[yesterday]
```

#### 会议论文
```
"NeurIPS 2025" OR "ICML 2025" OR "ACL 2025" AI paper
```

---

### 行业与商业

#### AI 融资与投资
```
"AI startup funding" OR "artificial intelligence investment" after:[week_ago]
```

#### AI 公司新闻
```
"AI company news" OR "OpenAI news" OR "Google AI" after:[yesterday]
```

#### AI 合作伙伴关系与收购
```
"AI acquisition" OR "AI partnership" OR "artificial intelligence deal" after:[week_ago]
```

#### AI 市场趋势
```
"AI market trends" OR "artificial intelligence industry analysis" after:[week_ago]
```

---

### 产品与工具

#### 新 AI 工具
```
"AI application launch" OR "new AI tool" after:[yesterday]
```

#### AI 产品发布
```
"AI product release" OR "artificial intelligence software launch" after:[yesterday]
```

#### 开源 AI
```
"open source AI" OR "AI model release" OR "LLM release" after:[yesterday]
```

#### AI 框架更新
```
"PyTorch update" OR "TensorFlow update" OR "AI framework" after:[week_ago]
```

---

### 特定公司查询

#### OpenAI
```
"OpenAI announcement" OR "GPT update" OR "ChatGPT news" after:[yesterday]
```

#### Google
```
"Google AI announcement" OR "Gemini update" OR "Bard news" after:[yesterday]
```

#### Anthropic
```
"Anthropic news" OR "Claude update" OR "constitutional AI" after:[yesterday]
```

#### Meta
```
"Meta AI announcement" OR "LLaMA update" OR "Facebook AI" after:[yesterday]
```

#### Microsoft
```
"Microsoft AI" OR "Copilot update" OR "Azure AI news" after:[yesterday]
```

#### DeepMind
```
"DeepMind research" OR "AlphaFold update" OR "Google DeepMind" after:[week_ago]
```

---

## 高级搜索技术

### 布尔运算符

#### AND（两个术语都必须存在）
```
"AI" AND "breakthrough" AND "2025"
```

#### OR（至少一个术语必须存在）
```
"artificial intelligence" OR "machine learning" OR "deep learning"
```

#### NOT（排除术语）
```
"AI" AND "news" NOT "cryptocurrency" NOT "blockchain"
```

#### 精确短语
```
"large language model" OR "LLM"
```

### 日期过滤器

#### 最近 24 小时
```
after:[yesterday's date]
```

#### 最近 3 天
```
after:[3 days ago]
```

#### 最近一周
```
after:[7 days ago]
```

#### 最近一个月
```
after:[30 days ago]
```

### 来源过滤器

#### 仅新闻网站
```
site:venturebeat.com AI OR site:techcrunch.com AI
```

#### 学术来源
```
site:arxiv.org "artificial intelligence"
```

#### 公司博客
```
site:openai.com/blog OR site:blog.google/technology/ai
```

### 主题组合

#### AI + 医疗保健
```
"AI" AND "healthcare" OR "medical AI" after:[week_ago]
```

#### AI + 金融
```
"AI" AND "finance" OR "fintech AI" after:[week_ago]
```

#### AI + 伦理
```
"AI ethics" OR "artificial intelligence safety" after:[week_ago]
```

#### AI + 监管
```
"AI regulation" OR "AI policy" after:[week_ago]
```

---

## 查询优化技巧

### 1. 从宽泛开始，然后细化
从通用查询开始，然后根据结果缩小范围：
1. `"AI news today"` → 广泛概览
2. `"AI product launch"` → 特定关注
3. `"OpenAI product launch"` → 非常具体

### 2. 始终使用日期过滤器
始终包含日期过滤器以确保新鲜内容：
- 每日简报：`after:[yesterday]`
- 每周摘要：`after:[week_ago]`

### 3. 组合类别以获得全面结果
混合不同类别的查询：
- 1-2 个通用查询
- 1-2 个研究查询
- 1-2 个行业查询
- 1-2 个产品查询

### 4. 避免冗余术语
不要组合相似术语：
- ❌ `"AI" AND "artificial intelligence"`（冗余）
- ✅ `"AI" OR "machine learning" OR "deep learning"`（互补）

### 5. 使用引号进行精确短语搜索
搜索特定短语时使用引号：
- ✅ `"large language model"`
- ❌ `large language model`（可能返回更广泛的结果）

### 6. 排除不相关主题
使用 NOT 过滤掉不相关内容：
```
"AI news" NOT "crypto" NOT "web3" NOT "blockchain"
```

---

## 示例查询组合

### 每日简报（全面）
```
Query 1: "AI news today" OR "artificial intelligence breakthrough" after:[yesterday]
Query 2: "AI research paper" OR "machine learning breakthrough" after:[yesterday]
Query 3: "AI startup funding" OR "AI company news" after:[week_ago]
Query 4: "AI product release" OR "new AI tool" after:[yesterday]
```

### 研究重点
```
Query 1: "AI research paper" OR "machine learning breakthrough" after:[yesterday]
Query 2: arXiv "cs.AI" OR "cs.LG" paper after:[yesterday]
Query 3: "AI breakthrough" OR "research advancement" after:[yesterday]
```

### 行业重点
```
Query 1: "AI startup funding" OR "artificial intelligence investment" after:[week_ago]
Query 2: "AI company news" OR "OpenAI news" OR "Google AI" after:[yesterday]
Query 3: "AI acquisition" OR "AI partnership" after:[week_ago]
```

### 产品重点
```
Query 1: "AI product release" OR "new AI tool" after:[yesterday]
Query 2: "open source AI" OR "AI model release" after:[yesterday]
Query 3: "GPT update" OR "Claude update" OR "Gemini update" after:[yesterday]
```

---

## 查询性能技巧

1. **限制结果**：大多数搜索工具默认返回 10-15 个结果，这通常就足够了
2. **优先考虑最新**：始终使用日期过滤器确保新鲜内容
3. **多样化来源**：使用能从不同类型来源（新闻网站、博客、学术）返回结果的查询
4. **调整范围**：如果结果太少，扩大日期范围或使用更广泛的术语
5. **优化相关性**：如果结果太多，添加更具体的术语或缩小日期范围
6. **验证结果**：始终检查发布日期以确保内容确实是最新的
