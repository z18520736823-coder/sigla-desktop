# Review AI Work with Confidence

## English

Sigla turns long AI-generated Markdown into clear conclusions, source-linked insights, and actionable feedback. Review every claim in context while your original document remains safely read-only.

## 中文

Sigla 将冗长的 AI 生成 Markdown 提炼为清晰结论、原文证据与可执行反馈。每条观点都能精准返回对应位置，整个审阅过程始终保持源文件只读。

## Code

```typescript
const review = await sigla.analyze(document, {
  provider: "OpenAI | DeepSeek",
  sourceAnchors: true,
  readOnly: true,
});
```

## Review Summary

| Signal | Result | Status |
| --- | --- | :---: |
| Central conclusion | Evidence linked | ✓ |
| Source annotations | Precisely anchored | ✓ |
| Agent feedback | Ready to hand off | ✓ |
