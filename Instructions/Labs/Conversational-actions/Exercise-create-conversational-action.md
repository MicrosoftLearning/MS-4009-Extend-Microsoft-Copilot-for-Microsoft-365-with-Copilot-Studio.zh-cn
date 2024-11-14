# 练习：创建对话操作

在本练习中，你将创建一个对话操作，提供关于一个名为“Project ABC”的虚构组织项目的信息。

练习任务：

- 在 Copilot Studio 中创建对话操作
- 将对话操作发布到 Microsoft Copilot
- 在 Microsoft Copilot 中测试你的对话操作

## 任务 1：（可选）测试默认体验

首先，在 Microsoft 365 Copilot 中问一个有关 Project ABC 的问题。

1. 打开 **Microsoft Teams**，使用你的工作或学校帐户登录。

1. 在边栏中选择“**聊天**”。

1. 在聊天菜单中选择“**Copilot**”。

1. 在消息撰写框中输入 `Who should I contact for questions about Project ABC?`

1. 请注意，Microsoft 365 Copilot 目前没有任何有关 Project ABC 的信息。

## 任务 2：创建新的对话操作

首先，在 Microsoft Copilot 中为新的对话操作配置名称、解决方案和架构。

1. 在 Web 浏览器中，导航到 [Copilot Studio](https://copilotstudio.microsoft.com) 并使用你的工作或学校帐户登录（如果出现提示）。  选择“**跳过**”，以跳过任何欢迎消息。

    **注意：** 首次打开 Copilot Studio 时，它可能会显示聊天界面来创建第一个 copilot。 如果发生这种情况，请选择**** 右上角的“...”菜单（“**Create**”按钮旁），然后选择“**Cancel copilot creation**”，选择“**leave**”以离开聊天界面并查看 Copilot Studio 主页。
1. 在左侧导航中，选择“**库**”。 你可以在此处查看现有操作和连接器的列表并创建新的列表。
1. 选择顶部的“**添加项**”。  菜单列出了用于为 Microsoft 365 扩展 Copilot 的 2 个选项。
:::image type="content" source="../Media/extend copilot options.png" alt-text="窗口列出了用于扩展 Copilot 的 2 个选项：创建 copilot 或创建操作。":::
1. 选择**新建操作**。

1. 选择“**对话**”以创建对话操作。

1. 在“**名称**”字段中，输入 `Project ABC` 并接受默认解决方案和架构。

1. 选择“创建”以继续****。 将创建新的对话操作。 这需要几秒钟。 完成后，你将进入创作画布以继续配置操作。

## 任务 3：配置主题

接下来，配置主题的名称和触发器。

1. 在对话操作创作窗格中，导航到“**主题**”选项卡。

1. 选择窗格顶部的“**主题名称**”文本框，该文本框默认名称为 `"Untitled"`，并输入 `Project ABC info` 以为主题命名。

1. 在主题中的“**触发器**”节点中，选择“描述主题的作用”文本下的文本框，然后输入 `Answers questions and provides information about Project ABC, including questions about objectives, points of contact, and rollout timeline.`。

## 任务 4：发送消息

接下来，向主题添加一个节点，以发送有关 Project ABC 的消息。

1. 在“触发器”节点下，选择要添加新节点的“**+**”图标。

1. 在显示的菜单中，选择“**发送消息**”。  已创建新的消息节点。

1. 在“消息”节点中，选择文本框并输入 `Project ABC is an initiative aimed at improving the culture and engagement within the company.  Objectives of the project include improved morale, increased employee survey results, and improved culture ratings.  For more information about Project ABC, contact Devon Torres.`。

1. 选择创作画布上方的“**保存**”以保存更改。

## 任务 5：发布操作

接下来，发布操作以在 Microsoft 365 Copilot 中使用。

1. 选择页面顶部的“**发布**”。

1. 在“**发布插件**”页上选择“**发布**”。

1. 在“**发布最新内容**”页上，确认已启用 Project ABC 信息插件并选择“**发布**”。  发布可能需要几分钟时间。  发布完成后，窗口顶部会显示一条通知。

## 任务 6：启用和测试操作

最后，在 Microsoft 365 Copilot 中测试操作。

1. 打开 **Microsoft Teams**。

1. 在边栏中选择“**聊天**”。

1. 在聊天菜单中选择“**Copilot**”。

1. 在消息撰写区域，选择“**管理 Copilot 响应**”按钮。

1. 在浮出控件中，搜索 **Copilot Studio**，然后选择“**添加**”以添加 Copilot Studio。
 
2. “**Project ABC 信息**”操作现在应列在浮出控件中。  确认“**Project ABC 信息**”已启用，然后关闭浮出控件。

:::image type="content" source="../Media/projectABCInfo-action-enabled.png" alt-text="Project ABC 信息操作在浮出控件中列出的屏幕截图"Manage Copilot response" flyout in Teams.":::

3. 在消息撰写框中输入 `Who should I contact for questions about Project ABC?`

4. 请注意，Microsoft 365 Copilot 通过调用对话操作返回有关 Project ABC 的信息。

可以使用其他节点自定义或展开此对话操作。  例如，可以创建新的“**生成式答案**”节点并上传一个文件，从而扩展可用于操作的知识。

**注意：** 在 Copilot 中测试操作时，请记住以下几点：
- Copilot 将始终用自己的语言改写你的答案。 在此预览版中，不可能将内容原封不动地传递给最终用户。
- 对话操作的说明对于调用它的可靠性至关重要。 此说明会告诉业务流程协调程序你的操作擅长什么以及它能提供什么答案。 在写描述时，一定要使用清晰的文字，并考虑尝试改变以获得最好的结果。
- 正确执行这些步骤不能保证 Copilot 每次都会返回预期结果。  Copilot 将确定何时调用插件以及如何返回结果。

## （可选）挑战：创建自己的对话操作！

应用你学到的知识为所选应用场景创建、发布和测试新的对话操作。  根据需要回顾本练习中的步骤。