```markdown
```java
diff --git a/openai-code-review-sdk/src/main/java/plus/gaga/middleware/sdk/OpenAiCodeReview.java b/openai-code-review-sdk/src/main/java/plus/gaga/middleware/sdk/OpenAiCodeReview.java
index d89ed4f..b01e3a9 100644
--- a/openai-code-review-sdk/src/main/java/plus/gaga/middleware/sdk/OpenAiCodeReview.java
+++ b/openai-code-review-sdk/src/main/java/plus/gaga/middleware/sdk/OpenAiCodeReview.java
@@ -80,7 +80,7 @@

 public class OpenAiCodeReview {
     // ... (other code)

-    add(new ChatCompletionRequest.Prompt("user", "评审时要展示变更的代码情况，对代码的评审要有具体行号"));
+    add(new ChatCompletionRequest.Prompt("user", "评审时要展示变更的代码情况，对代码的评审要有具体行号，输出的markdown 代码块要有对应代码的高亮"));

     // ... (other code)
 }
```
```

### 代码评审：

在上述代码变更中，可以看到在`OpenAiCodeReview`类中，第80行发生了一个小的改动。原来的代码是：

```java
add(new ChatCompletionRequest.Prompt("user", "评审时要展示变更的代码情况，对代码的评审要有具体行号"));
```

这个代码行被更新为：

```java
add(new ChatCompletionRequest.Prompt("user", "评审时要展示变更的代码情况，对代码的评审要有具体行号，输出的markdown 代码块要有对应代码的高亮"));
```

这个变更增加了对输出Markdown代码块高亮显示的要求。这个改动可能意味着代码评审的输出格式有所增强，以便于用户更清晰地看到代码的变更和具体的行号。这样的改进对于提高代码评审的效率和可读性是有益的。