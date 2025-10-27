## 🧑‍💼 AskHR Lab 2: Building a RAG agent
Please refer to Lab 2 Explanations before starting.

In this lab, we will enable our HR agent in watsonx Orchestrate to answer questions based on a knowledge base. This agent retrieves relevant information from documents to answer user queries.

We will make this agent more powerful with more tools and access to APIs, and enable it to collaborate with other agents in lab3.

Step by step instructions to build the HR Agent:
When you launch watsonx Orchestrate, you’ll be directed to this page. Click on the hamburger menu in the top left corner:

![image]()

Click on the down arrow next to Build. Then click on Agent Builder:

![image]()

Click on Create agent +:

![image]()

Select “Create from scratch”, give your agent a unique name (make sure to identify yourself by your initials or name, since this is a shared instance), e.g. “[Your Initial]_HR Agent”, and fill in the description as shown below:

 You are an agent who handles employee HR queries.  You provide short and crisp responses, keeping the output to 200 words or less. You can answer general questions about company benefits.

Click on Create:

![image]()

We are going to build a knowledge base for the agent. Scroll down the screen to the Knowledge section and click on “Choose knowledge”.

![image]()

Choose “Upload files” and click “Next”.

![image]()

Drag and drop the Employee Benefits.pdf and click on Next:

![image]()

Copy the following description into the Description section and click Save:

 This knowledge base addresses the company's employee benefits, including parental leaves, pet policy, flexible work arrangements, and student loan repayment.

![image]()# 🧑‍💼 AskHR Lab 2: Building a RAG Agent

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

![image]()

---

### 2. Open Agent Builder
Click on the **down arrow** next to **Build**, then click on **Agent Builder**.

![image]()

---

### 3. Create a New Agent
Click **Create agent +**

![image]()

Select **Create from scratch**, then fill in the details as follows:

- **Agent name:** `[YourInitial]_HR Agent`
- **Description:**

```TEXT
You are an agent who handles employee HR queries.
You provide short and crisp responses, keeping the output to 200 words or less.
You can answer general questions about company benefits.
```


Click **Create**.

![image]()

---

## 🧠 Building the Knowledge Base

### 4. Add Knowledge
Scroll down to the **Knowledge** section and click **Choose knowledge**.

![image]()

---

### 5. Upload Documents
Select **Upload files** and click **Next**.

![image]()

Drag and drop the file **Employee Benefits.pdf**, then click **Next**.

![image]()

---

### 6. Add Knowledge Base Description
Copy and paste the following description:

```TEXT
This knowledge base addresses the company's employee benefits, including parental leaves, pet policy, flexible work arrangements, and student loan repayment.
```


Click **Save**.

![image]()

> ⏳ The knowledge base may take a few moments to finish creating. Once completed, you will be returned to the **Agent Builder UI**.

---

## ⚙️ Configure Behavior

### 7. Add Agent Instructions
Scroll down to the **Behavior** section.  
In the **Instructions** field, paste the following:

```TEXT
Use your knowledge base to answer general questions about employee benefits.
```

![image]()

---

## 🧪 Test the Agent

Test your agent in the **Preview Chat** (on the right-hand side) by asking the following questions:

- **What is the pet policy?**

![image]()

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

![image]()

Scroll down to the Behavior section. Insert the instructions below into the Instructions field:

 Use your knowledge base to answer general questions about employee benefits. 

![image]()

Test your agent in the preview chat on the right side by asking the following questions and validating the responses. They should look similar to what is shown in the screenshot(s) below:

 What is the pet policy? 

![image]()

You can try the following sample questions as well:

 how many days of leave am i entitled to?

 can i work from home 3 times a week?

 does the company provide any assistance on loan repayments?

Notice that you get a generic answers based on policy for all employees. You will see in the next lab how you can connect it to Employee Address Agent and Leave Management Agent from Lab 1 to do tasks for you.

Congratulations! You’ve built your RAG Agent.
