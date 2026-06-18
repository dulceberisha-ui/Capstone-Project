# Capstone-Project
Restaurant Complaint Escalation Agent
The Tool
For this capstone project, I used Relevance AI, an agent-building platform that allows users to create autonomous agents capable of analyzing information, making decisions, and generating business outputs. Relevance AI was not used or demonstrated during this course, which makes it an eligible platform for the capstone requirement. I used the free-tier version of the platform.
I selected Relevance AI because it provides a simple way to build agentic workflows without requiring coding knowledge while still allowing an agent to perform multiple decision-making steps. Rather than functioning as a simple chatbot, the platform enables agents to analyze information, classify problems, determine escalation paths, and generate actionable outputs.
The Build
I built a Restaurant Complaint Escalation Agent designed for restaurant managers and operations teams. The purpose of the agent is to analyze customer complaints and reviews, determine the seriousness of the issue, decide whether management intervention is required, and generate both customer-facing and internal business responses.
The workflow begins when a customer complaint is submitted. The agent analyzes the complaint and identifies sentiment, category, severity level, and whether escalation is required. It then creates a professional customer response, an internal manager memo, and a recommended action plan.
This workflow mirrors a real process commonly performed by restaurant managers and customer service staff. By automating the initial review process, the agent helps managers prioritize serious complaints while maintaining consistent communication with customers.
Pic 1
https://app.relevanceai.com/agents/d7b62b/894effb2-c397-4d5f-8a29-3abf3d5fe972/9c9a85c1-e253-49de-96d7-ecc2d173c24e/embed-chat?hide_tool_steps=false&hide_file_uploads=false&hide_conversation_list=false&bubble_style=agent&primary_color=%23685FFF&bubble_icon=pd%2Fchat&input_placeholder_text=Type+your+message...&hide_logo=false&hide_description=false
Agent Card
Purpose
Analyze restaurant customer complaints and reviews to identify operational issues, determine escalation requirements, and generate actionable responses.
Role
Restaurant Complaint Escalation Agent
Inputs
The agent has access to:
Customer complaints
Customer reviews
Restaurant feedback text
Reservation-related complaints
Service-related complaints
The agent does not have access to:
Customer payment information
Employee personnel records
Internal financial data
Confidential business documents
Private customer account information
Task Steps
Receive customer complaint.
Analyze complaint sentiment.
Identify primary complaint category.
Determine severity level.
Decide whether escalation is required.
Generate a customer response.
Generate an internal manager memo.
Recommend corrective actions.
Constraints
Must not fabricate customer information.
Must maintain professional language.
Must not make legal promises.
Must not disclose confidential information.
Must classify complaints consistently.
Output Format
Sentiment
Category
Severity
Escalation Required
Customer Response
Manager Memo
Recommended Action
Escalation Trigger
Escalation is required when complaints involve:
Repeated negative experiences
Management misconduct
Food safety concerns
Harassment or discrimination claims
Severe customer service failures
Potential legal issues
Success Metric
The agent successfully classifies complaints, identifies escalation needs, and produces accurate customer-facing and internal management outputs.
Evaluation
The agent was evaluated using the four dimensions discussed in Module 3.
Correctness
Score: 9/10
The agent consistently identified sentiment and severity levels that matched the content of each complaint. It successfully distinguished between positive, mixed, and negative customer experiences.
Completeness
Score: 9/10
The agent provided all required outputs including sentiment analysis, categorization, escalation decisions, customer responses, manager memos, and recommended actions.
Safety
Score: 8/10
The agent did not expose confidential information and maintained professional language. However, like most LLM-based systems, it could still potentially misclassify unusual complaints without additional human review.
Fit
Score: 10/10
The agent directly addresses a real operational problem faced by restaurants. The outputs generated are immediately useful for managers and customer service teams.
Test Run 1 – Positive Customer Experience
Input:
"The food was amazing, our server was friendly, and everything arrived quickly. We will definitely be coming back."
Results:
Sentiment: Positive
Severity: Low
Escalation Required: No
The agent correctly recognized a positive experience and determined that no escalation was necessary.
Insert Screenshot 2
Test Run 2 – Reservation Delay
Input:
"The food tasted great but we waited 45 minutes for our table even though we had a reservation."
Results:
Sentiment: Mixed
Severity: Medium
Escalation Required: Yes
The agent correctly identified both positive and negative aspects of the experience and recommended management review.
Insert Screenshot 3
Test Run 3 – Serious Customer Complaint
Input:
"We waited over an hour for our food. It arrived cold, and when we asked for help the manager refused to speak with us. This is the second time this has happened."
Results:
Sentiment: Negative
Severity: High
Escalation Required: Yes
The agent correctly recognized multiple service failures and recommended escalation.
Insert Screenshot 4
Risk and Governance
Prompt Injection
Risk
A user could intentionally include instructions inside a complaint attempting to manipulate the agent's behavior.
Mitigation
The agent is restricted to complaint analysis tasks and follows a structured output format that limits opportunities for prompt manipulation.
Tool Abuse
Risk
An agent connected to external systems could perform unintended actions.
Mitigation
This agent has no external business system access and only performs text analysis and response generation.
Over-Permissioning
Risk
An agent could have access to data beyond what is necessary for its role.
Mitigation
The agent only receives customer complaint text and does not access payment systems, employee records, or confidential company information.
Data Leakage
Risk
Sensitive customer or employee information could appear in outputs.
Mitigation
The workflow uses sample data and excludes confidential information. Outputs are limited to complaint analysis and management recommendations.
Business Case
Restaurants receive customer feedback from many channels including review websites, surveys, email, and social media. Managers often spend significant time reviewing complaints and determining which issues require attention.
This agent reduces the time required to evaluate complaints by automatically classifying issues and recommending actions.
ROI Estimate
Time Saved
Manual review of a complaint may take approximately 10 minutes.
Agent review takes less than one minute.
For 100 complaints per month:
10 minutes × 100 complaints = 1,000 minutes
1,000 minutes = approximately 16.7 hours saved monthly.
Error Reduction
The agent provides a consistent classification process and reduces variation between different managers reviewing complaints.
Deflection
The agent generates customer responses automatically, reducing the amount of writing required from managers and customer service staff.
Overall, the system can improve operational efficiency while ensuring that serious complaints receive attention more quickly.
Honest Limits and Next Steps
Although the agent performed well during testing, several limitations remain.
First, the agent depends entirely on the information provided by the customer. If the complaint is vague or misleading, the classification may be inaccurate.
Second, the agent cannot independently verify events that occurred in the restaurant. Human review is still necessary before taking significant action.
Third, the agent may occasionally misclassify unusual situations that were not represented during testing.
Overall, this project demonstrated how agentic AI can support restaurant operations by automating complaint analysis, improving consistency, and helping management respond more effectively to customer concerns.
