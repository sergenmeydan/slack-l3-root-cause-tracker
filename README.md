# 🤖 Slack L3 Error & Root Cause Tracker

This project is an **n8n workflow** that automatically analyzes error messages shared by operations teams via Slack. It transforms complex logs into meaningful reports in seconds.

## 🔥 Key Features
* **Smart Filtering:** Only activates for messages containing critical keywords (error, problem, fault).
* **Python Logic Engine:** Scans incoming text to determine whether the error is database-related, network-related, or permission-related.
* **Action Recommendation:** Based on the analysis, it provides the team with direct solutions such as “Restart the service” or “Check the DB Pool.”
* **Loop Lock:** Includes a special `bot_id` and header check that prevents the bot from analyzing its own messages.

## 🛠️ How to Set It Up?
1. Download the `.json` file from the repo.
2. Import it from the n8n interface by selecting **Import from File**.
3. Set up your own **Credentials** in the Slack Trigger node.
4. Activate the flow by **Publishing** it.

⚠️ Note: For security reasons, Slack API keys and Channel IDs have been removed from this JSON file. After importing the flow, you must set up your own Slack connections and reselect your Channel ID in the Slack Trigger and Send a message nodes.

## 📸 Screen Shots
<img width="871" height="322" alt="image" src="https://github.com/user-attachments/assets/26971bc9-7750-4be4-a46b-3fc4c821f60a" />
<img width="538" height="406" alt="image" src="https://github.com/user-attachments/assets/17e55251-8bd7-49cc-8e74-7e86c5722a09" />

