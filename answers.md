# MCP Assignment Answers

### 1. How many tools were available in Part 1 and Part 3? What changes were required in the client?

The MCP server initially provided 8 tools in Part 1. After implementing the new `predict_both` function, it provided 9 tools in Part 3. The client automatically detected the additional tool through `list_tools()`. I created a separate client program to discover and use the new tool.

### 2. For how many test patients did Logistic Regression and KNN produce different predictions? Which model was correct?

The two models gave different predictions for 8 of the 114 test patients.

- Patient 3 – Logistic Regression
- Patient 25 – Logistic Regression
- Patient 48 – Logistic Regression
- Patient 53 – KNN
- Patient 76 – Logistic Regression
- Patient 80 – Logistic Regression
- Patient 99 – Logistic Regression
- Patient 102 – Logistic Regression

These are the models that correctly predicted the actual diagnosis for each patient.

### 3. Which model performed better when the predictions were different?

Logistic Regression made the correct prediction in 7 cases, whereas KNN was correct in 1 case. Based on these disagreements, Logistic Regression performed better.

### 4. What is the importance of the triple-quoted tool description?

The tool description tells an AI application what the function is designed to do. It helps the application understand the tool's purpose and determine when it should be used.

### 5. Why should an MCP server maintain a log of tool calls?

Maintaining logs makes it easier to monitor tool usage, identify successful and failed requests, troubleshoot problems, and keep a record of activities. These records also help with auditing and accountability.