# Car Smart
An AI powered app helping you troubleshoot car issues

## Table of Contents

- [Overview](#overview)
- [Tech Stack](#tech-stack)
- [Features](#features)
- [Deployment](#deployment)
- [License](#license)


## Overview
Car Smart is an AI powered PWA application that helps users by answering car related questions. 
It allows getting advice based on user provided text and images. The interface includes a chat, dashboard page with recent and specific brand related questions.
All previous threads (own and from other users) are available at all times for reference, as other user threads are read-only.
Users can save their car brand preferences, which will personalize their dashboard with brand-relevant questions first. 

## Tech Stack

- Oracle APEX - application development framework
- Oracle Database
- Claude 3 (Haiku) API - AI chat completions 

## Features

The app allows users to take picture of a car dashboard alert, broken parts or simply a description of an issue. By using a car brand tailored System Prompts
and a chat feature, they can get help from the AI assistant. All chat threads are saved and can be reviewed by other app users. 

Beyond the chat feature, users can explore past issues and find similar ones with their resolution.

The application is a PWA, which means that it runs in the browser, but can also be installed on any device, just like native one.

The initial version uses Anthropic Claude 3 (Haiku) as a LLM, supporting multimodal inputs. For the demo purpose all costs are covered by me.
If you install it on your Oracle APEX instance, make sure to update the API Key (which is not included in the installation file).

## Deployment
Import the application `.sql` export file in APEX. 

Read the guide on how to [Import an Application in Oracle APEX](https://docs.oracle.com/en/database/oracle/apex/24.1/htmdb/importing-export-files.html)

During the installation, you will be prompted for installing `Supporting Object`. Agree and proceed with this part too.
After installation is complete, make sure to configure the Credentials for accessing Claude 3's API.

![image](https://github.com/user-attachments/assets/e6f35479-cf6e-47f9-9152-bb0bacfc208c)

## License

This is project is under [MIT LICENSE](LICENSE)
