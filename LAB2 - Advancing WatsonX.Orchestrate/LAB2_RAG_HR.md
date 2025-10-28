# 🧑‍💼 AskHR Lab 2: Building a RAG Agent

> **Before you start:** Please refer to **Lab 2 Explanations** to understand the concept of Agentic RAG (Retrieval-Augmented Generation).

---

## 🎯 Objective

In this lab, we will enable our **HR agent** in *watsonx Orchestrate* to answer questions based on a **knowledge base (KB)**.  
This agent retrieves relevant information from documents to answer user queries.

We will make this agent more powerful with more tools and access to APIs, and enable it to collaborate with other agents in **Lab 3**.

---

## 🪜 Step-by-Step Instructions

### 1. Launch watsonx Orchestrate
When you launch **watsonx Orchestrate**, you’ll be directed to the main page.  
Click on the **hamburger menu (☰)** in the top left corner.

![Step1](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/step1.png)


---

### 2. Open Agent Builder
Click on the **down arrow** next to **Build**, then click on **Agent Builder**.

![step2](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/step2.png)

---

### 3. Create a New Agent
Click **Create agent +**

![step3](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/step3.png)


Select **Create from scratch**, then fill in the details as follows:

- **Agent name:** `[YourInitial]_HR Agent`
- **Description:**

```TEXT
You are an agent who handles employee HR queries.
You provide short and crisp responses, keeping the output to 200 words or less.
You can answer general questions about company benefits.
```


Click **Create**.

![step4](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/hr_step4.png)

---

## 🧠 Building the Knowledge Base

### 4. Add Knowledge
Scroll down to the **Knowledge** section and click **Choose knowledge**.

![step5](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/hr_step5.png)

---

### 5. Upload Documents
Select **Upload files** and click **Next**.

![step6](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/hr_step_6.png)

Drag and drop the file [Employee-Benefits.pdf](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/Employee-Benefits.pdf), then click **Next**.

![step7](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/hr_step7.png)

---

### 6. Add Knowledge Base Description
Copy and paste the following description:

```TEXT
This knowledge base addresses the company's employee benefits, including parental leaves, pet policy, flexible work arrangements, and student loan repayment.
```


Click **Save**.

![step8](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/hr_step8.png)

> ⏳ The knowledge base may take a few moments to finish creating. Once completed, you will be returned to the **Agent Builder UI**.

---

## ⚙️ Configure Behavior

### 7. Add Agent Instructions
Scroll down to the **Behavior** section.  
In the **Instructions** field, paste the following:

```TEXT
Use your knowledge base to answer general questions about employee benefits.
```

![step9](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/hr_step9.png)

---

## 🧪 Test the Agent

Test your agent in the **Preview Chat** (on the right-hand side) by asking the following questions:

- **What is the pet policy?**

![step10](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/hr_step10.png)

You can also try:

- *How many days of leave am I entitled to?*  
- *Can I work from home three times a week?*  
- *Does the company provide any assistance on loan repayments?*

> 💡 You’ll notice that the agent gives **generic answers** based on company policy for all employees.

---

## 🤝 Next Step

In the next lab, you will see how to **connect this HR Agent** to:
- The **Employee Address Agent**
- The **Leave Management Agent**

...to enable task execution and cross-agent collaboration.

---

## 🏁 Congratulations!

🎉 You’ve successfully built your **RAG Agent** — an intelligent HR assistant that retrieves answers from a knowledge base!

---


The knowledge base will take some time to create. After the knowledge base is done, you will be brought back to the Agent Builder UI.

![step11](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/hr_step11.png)

Scroll down to the Behavior section. Insert the instructions below into the Instructions field:

 Use your knowledge base to answer general questions about employee benefits. 

![step12](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/hr_step12.png)

Test your agent in the preview chat on the right side by asking the following questions and validating the responses. They should look similar to what is shown in the screenshot(s) below:

 What is the pet policy? 

![step13](https://github.com/Client-Engineering-Indonesia/Incubation-Agentic-AI-2025-batch-4-29Oct/blob/main/LAB2%20-%20Advancing%20WatsonX.Orchestrate/Images/hr_step13.png)

You can try the following sample questions as well:
```text
how many days of leave am i entitled to?
```

```text
can i work from home 3 times a week?
```

```text
does the company provide any assistance on loan repayments?
```

Notice that you get a generic answers based on policy for all employees. You will see in the next lab how you can connect it to Employee Address Agent and Leave Management Agent from Lab 1 to do tasks for you.

Congratulations! You’ve built your RAG Agent.
