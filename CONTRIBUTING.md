# Contribution Guidelines

[简体中文](#zh-cn) | [English](#en)

## zh-CN

欢迎为 CompPsyUnion 微信公众号贡献内容！你可以在 [Issue 页面](https://github.com/CompPsyUnion/2526-wechat-blogs/issues) 通过新建一个 issue 来提出你的公众号文章提议。

请仔细阅读下面的内容来了解我们的投稿流程。

### 一个投稿的标准流程

1. 提出文章标题和大纲
2. 文章标题和大纲审核通过
3. 完整稿件提交
4. 完整稿件审核
5. 文章发布（第二周 周三或周五）

### 详细说明

#### 1. 提出文章标题和大纲

> 当然，如果你足够自信，你也可以直接跳过这一步，写好完整的内容直接从 [第三步](#3-完整稿件提交) 开始。反之如果你不确定你的推文内容是否合适，建议还是走完这个流程。

你可以在 [Issue 页面](https://github.com/CompPsyUnion/2526-wechat-blogs/issues) 通过新建一个 issue 来提出你的公众号文章提议。

**Issue 标题格式：** 请在标题中简明扼要地写出你的文章标题。

**Issue 描述内容：** 在 issue 的 description 中添加你的文章内容大纲，不一定要写完。大纲应包括：

- 文章的主要小标题
- 每个小标题下的主要内容要点
- （可选）参考资料

**示例：**

```markdown
# 一个示例文章标题

大家好，今天我给大家带来的是一篇示例微信公众号文章

## 文章小标题 1

在提出这个提议的 issue 时，最好同时在 description 中添加一个文章内容的大纲，不一定要写完

## 文章小标题 2

提出的标题和这个大纲的内容，决定了我们是否会采纳你的提议。

## 结语
```

**Self-Assignment 说明：**

- 如果你只是想给文章提出一个建议，走到这一步就可以，我们可以在征得你的同意后将这个内容 assign 给我们 CPU 技术部的其他成员来完成。
- **如果你是想自己完成这个内容，请在这个 issue 创建后，把自己 assign 给自己（self-assign）**，这样我们就知道你会负责这个内容的后续工作。

**被动 Assignment：**

我们也可能通过主动创建一个 issue 然后 assign 给你来派发任务，这时你就需要新想出一个文章标题和大纲然后 Comment 到下方。收到 assignment 时你会收到通知。在你完成上面的操作后，我们会继续下面的审核流程。

#### 2. 文章标题和大纲审核

我们会在 3 个工作日内对你的文章标题和大纲进行审核。

**审核通过：**

- 我们会为这个 issue 添加上一个 `Task` 的标签（label）
- 我们会使用 milestone 给你排期
- 在 issue 下方留言告知你审核通过，例如："不错，请继续完成"
- 如果你被 assign 到了这个任务，你就可以继续进行下一步的操作了

**重要提醒：** 只有你的 issue 被标注为了 `Task` 标签，你才能放心开始写完整内容（否则如果你的推文提议被拒绝，你可能面临工作白干的风险）。

**需要修改：**

- 我们会在 issue 下方留言并说明需要修改的地方
- 请你根据反馈进行修改并在评论中回复

**审核不通过：**

- 我们会在 issue 下方留言并说明原因
- 并关闭（close）这个 issue

##### 大纲要点

- 文章标题要简洁明了，能够吸引读者的注意力
- 文章大纲要包含文章的主要内容和结构，至少要有 2 个子版块
- 文章内容要符合公众号的定位和读者的兴趣，避免敏感话题
- 提出的标题和这个大纲的内容，决定了我们是否会采纳你的提议

#### 3. 完整稿件提交

**注意时间节点：**

- 请在上方我们给你标注的 milestone 的 due date 之前完成你的推文
- 如果长时间没给你标注 milestone，你也可以直接开始编写完整的推文内容并发送到 issue
- 越是完善的内容，我们越可能给你更早排期到位
- 如果超期未完成，你将面临被扣积分的风险

**编写建议：**

- 你可以在本地使用编辑器写 Markdown
- **建议不要直接在 GitHub issue 评论框中写**，因为你的 Markdown 最终需要通过 VSCode Markdownlint 插件的语法规范检测

**提交步骤：**

1. **粘贴完整内容：** 首先在 Comment 输入框粘贴文件的所有内容，让其在 issue 中展示出来
2. **上传 Markdown 文件：** 将 Markdownlint 检查后没有报错的 markdown 文件拖拽进评论框上传
   - 文件名使用小写蛇形命名法（snake_case）描述你的标题
   - 禁止包含中文和特殊字符
   - 例如：`a_good_name_should_look_like_this.md`
   - GitHub 会自动上传并为你生成链接

**Markdown 文章内容要求：**

- 文章长度在 400 到 2000 字之间
- 由于微信对外部链接限制，外部链接请直接粘贴链接，**不要使用markdown语法插入链接**
- 避免在公式块中特殊规定颜色，*这个需求我们做不了*
- 如需**特殊署名**，请在自己文章下方标注作者。我们最终会以`Robert(Siyuan) He`的形式呈现。
- 文章内容要有逻辑性和连贯性，避免语法错误和拼写错误
- 文章内容要有一定的原创性，避免大篇幅抄袭和引用。我们会使用工具来检测文章的原创性
- **图片插入：** 使用 Markdown 语法 `![alt text](image_url)` 来插入图片
  - 确保图片的版权和来源合法
  - 提交前确保图片的链接可以访问（使用 preview 查看）
  - 图片清晰度足够、大小适中
    > 注意，如果图片原先是本地文件，请先上传到图床（如 GitHub Issues 自带的图床）然后再使用链接插入
- **代码块：** 如果包含代码，请使用 Markdown 代码块，并**标注语言**
  - 示例：` ```python` 而不是仅仅 ` ``` `
  - 确保代码的正确性和可读性
- **Markdown 语法规范：** 使用 VSCode 的 Markdownlint (DavidAnson.vscode-markdownlint) 插件检查语法
  - **不要插入 HTML 语句**，我们微信没那么 6
  - 如果我们发现你的 markdown 在我们这里会有报错，你会需要返工
  - 需要在本地格式化通过后再提交（如不会请自行上网搜索，或者看第一次周常回放）
- **参考资料：** 如果包含参考资料，请在文章末尾使用引用的方式列出，并确保版权和来源合法

#### 4. 完整稿件审核

我们会在 3 个工作日内对你的文章完整稿件进行审核。请关注这个 issue 的动态。

**审核通过：**

- 维护者会留言："好的，收到" 或类似内容
- 你的文案将移交宣传部
- 维护者会 close 这个 issue，你的任务就算彻底完成了

**需要修改：**

- 我们会在 issue 下方留言并提出修改意见
- 请按照意见修改，保存后再和之前一样完整发一次到 issue 评论
- 我们也可能顺手帮你格式化了，需要返工的情况大概率是自动格式化时会产生歧义，需要你来自己决定如何排版

### 积分制度

- **主动提出并完成：** 如果是你主动提出此 issue，self-assign 并最后完成，你会得到 **2 点积分**
- **提议被采纳：** 如果你只是提出了这个 issue 但是我们 assign 给别的成员完成，你也可以得到 **1 点积分**
- **被动完成任务：** 如果开始时是我们 assign 给你一个 issue（不管是否为空），且你在最后完成，你可以得到 **1 点积分**
- **逾期未完成：** 如果你长时间没有完成 milestone 的 due date，你将面临被扣积分的风险

### 在你开始前

在开始前，也请查阅 [Issue #1](https://github.com/CompPsyUnion/2526-wechat-blogs/issues/1)，我们在这里提供了一个完整的工作流程示例。请参考这个示例的方法提出 issue。你也可以查看其他的 issue 来了解大家是如何提出文章提议的。

祝工作愉快 ；）

---

## en

Welcome to contribute content to CompPsyUnion's WeChat Official Account! You can propose your WeChat article by creating a new issue on the [Issue Page](https://github.com/CompPsyUnion/2526-wechat-blogs/issues).

Please read the following carefully to understand our submission process.

### Standard Submission Process

1. Propose article title and outline
2. Title and outline review approval
3. Complete manuscript submission
4. Complete manuscript review
5. Article publication

### Detailed Instructions

#### 1. Propose Article Title and Outline

> Of course, if you are confident enough, you can skip this step and start from [Step 3](#3-complete-manuscript-submission) by writing the complete content directly. On the other hand, if you are unsure whether your article content is appropriate, it is recommended to follow this process.

You can propose your WeChat article by creating a new issue on the [Issue Page](https://github.com/CompPsyUnion/2526-wechat-blogs/issues).

**Issue Title Format:** Write your article title concisely and clearly in the issue title.

**Issue Description Content:** Add your article outline in the issue description. It doesn't need to be complete. The outline should include:

- Main subheadings of the article
- Key points under each subheading
- (Optional) References

**Example:**

```markdown
# An Example Article Title

Hello everyone, today I'm bringing you an example WeChat Official Account article

## Article Subheading 1

When proposing this issue, it's best to add an outline of the article content in the description. It doesn't have to be complete.

## Article Subheading 2

The title and outline you propose determine whether we will adopt your proposal.

## Conclusion
```

**Self-Assignment Instructions:**

- If you just want to suggest an article idea, you can stop here. With your consent, we can assign this to other members of CPU's technical department to complete.
- **If you want to complete this content yourself, please self-assign yourself to this issue after creating it**. This way we know you'll be responsible for the subsequent work.

**Passive Assignment:**

We may also create an issue and assign it to you to delegate tasks. In this case, you'll need to come up with an article title and outline and comment below. You'll receive a notification when you get an assignment. After you complete the above, we'll proceed with the review process.

#### 2. Title and Outline Review

We will review your article title and outline within 3 working days.

**Review Approved:**

- We will add a `Task` type label to this issue
- We will schedule you using a milestone
- We'll comment below the issue to inform you of approval, e.g., "Great, please continue to complete it"
- If you're assigned to this task, you can proceed to the next step

**Important Reminder:** Only when your issue is typed with the `Task` tag can you confidently start writing the complete content (otherwise, if your article proposal is rejected, you may risk wasting your work).

**Needs Revision:**

- We will comment below the issue explaining what needs to be revised
- Please revise according to the feedback and reply in the comments

**Review Rejected:**

- We will comment below the issue explaining the reason
- And close this issue

##### Outline Key Points

- Article title should be concise and clear, able to attract readers' attention
- Article outline should include the main content and structure of the article, with at least 2 subsections
- Article content should align with the Official Account's positioning and readers' interests, avoiding sensitive topics
- The proposed title and outline content determine whether we will adopt your proposal

#### 3. Complete Manuscript Submission

**Note on Timeline:**

- Please complete your article before the due date of the milestone we assigned to you
- If you haven't been assigned a milestone for a long time, you can still start writing the complete article and submit it to the issue
- The more complete your content, the more likely we'll schedule you earlier
- If you fail to complete on time, you risk having points deducted

**Writing Recommendations:**

- You can write Markdown locally using an editor
- **It's recommended NOT to write directly in the GitHub issue comment box**, as your Markdown ultimately needs to pass VSCode Markdownlint plugin's syntax validation

**Submission Steps:**

1. **Paste Complete Content:** First, paste all the file content in the comment input box to display it in the issue
2. **Upload Markdown File:** Drag and drop the markdown file (after Markdownlint check with no errors) into the comment box to upload
   - File name should use lowercase snake_case to describe your title
   - No Chinese characters or special characters allowed
   - Example: `a_good_name_should_look_like_this.md`
   - GitHub will automatically upload and generate a link for you
   > Note, if the image was originally a local file, please upload it to an image hosting service (like GitHub Issues' built-in image hosting) before using the link to insert it

**Markdown Article Content Requirements:**

- Article length between 400 and 2000 words
- Content should be logical and coherent, avoiding grammatical and spelling errors
- Content should have a certain level of originality, avoiding extensive plagiarism and quotation. We will use tools to detect originality
- **Image Insertion:** Use Markdown syntax `![alt text](image_url)` to insert images
  - Ensure image copyright and sources are legitimate
  - Before submission, ensure image links are accessible (check using preview)
  - Images should be clear and appropriately sized
- **Code Blocks:** If including code, use Markdown code blocks and **specify the language**
  - Example: ` ```python` instead of just ` ``` `
  - Ensure code correctness and readability
- **Markdown Syntax Standards:** Use VSCode's Markdownlint (DavidAnson.vscode-markdownlint) plugin to check syntax
  - **Do NOT insert HTML statements**, our WeChat isn't that sophisticated
  - If we find your markdown has errors on our end, you'll need to rework it
  - Rework is usually needed when auto-formatting creates ambiguity, requiring you to decide on formatting yourself
  - Format it locally and pass validation before resubmitting (if you don't know how, please search online or watch the first weekly meeting replay)
- **References:** If including references, list them at the end of the article using citation format, ensuring copyright and sources are legitimate

#### 4. Complete Manuscript Review

We will review your complete manuscript within 3 working days. Please follow the issue updates.

**Review Approved:**

- Maintainers will comment: "OK, approved" or similar
- Your content will be handed over to the publicity department
- Maintainers will close this issue, and your task is completely finished

**Needs Revision:**

- We will comment below the issue with revision suggestions
- Please revise according to the suggestions, save, and submit the complete content again to the issue comments as before
- We may also help you format it, but rework is usually needed when auto-formatting creates ambiguity, requiring you to make formatting decisions

### Points System

- **Proactive Proposal and Completion:** If you proactively propose this issue, self-assign, and complete it, you'll receive **2 points**
- **Proposal Adopted:** If you only proposed this issue but we assigned it to another member to complete, you can still receive **1 point**
- **Passive Task Completion:** If we initially assigned you an issue (whether empty or not) and you complete it, you can receive **1 point**
- **Overdue Incompletion:** If you fail to complete the milestone's due date for a long time, you risk having points deducted

### Before You Start

Before starting, please also check [Issue #1](https://github.com/CompPsyUnion/2526-wechat-blogs/issues/1), where we provide a complete workflow example. Please refer to this example's method to propose issues. You can also check other issues to understand how others propose article ideas.

Happy contributing ；）
