# AzureDevopsWebHookBot

The aim of this was to have notification in google chat room on specific actions in azure (http service hooks).

# Currently supported features
   - send message to google chat room on pull request creation
   - send message to google chat room on specific comments (like "PTAL" - will tell reviewers that author asks reviewers "Please Take Another Look")
   - send message to google chat room when pipeline fails (will mention person with @annotation, which pipeline failed(with link) and detailed message)

# Requirements
  - Azure account
  - Configured azure functions 
  
# How to install
 - https://docs.microsoft.com/en-us/azure/python/tutorial-vs-code-serverless-python-01 
   The information in the link above will teach you how to create/debug/deploy python based function apps
 - update bot_url in script. This is the link that you obtain when you add "Incoming webhook" in google chat room.
 - when you deploy app to azure - go to your favorite project and in setting configure service hook (Post via HTTP)
