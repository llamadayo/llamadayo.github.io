---
title: spec-kit
published: 2025-11-11
description: ''
image: ''
tags: []
category: ''
draft: true 
lang: ''
---

```powershell title="(Windows) Install specify-cli"
# https://github.com/github/copilot-cli 
npm install -g @github/copilot

# https://github.com/github/spec-kit
uv tool install specify-cli --from git+https://github.com/github/spec-kit.git
```


```powershell title="(Windows) specify-cli"
specify init copilot_specify_test
specify check

cd .\copilot_specify_test\
copilot
```

```powershell title="(Windows) copilot"



> We're going to be using slash commands from ./github/prompts
> Create custom slash commands by adding prompt files to .github/prompts/

> /constitution static web app with minimal dependencies
> /specify a respnosive cross-platform business card web app, the business card should be dark and font color can be golden or any suitable color, and can be easily
   sharing to another people
> /speckit.clarify
> /speckit.plan (how to implement, tech, misc.)
> /speckit.tasks 
> /implement

```


建立一個web app ，主要是用來嵌在line 聊天室中的 liff 應用，因此需要響應式設計，預計搭配firebase，功能主要有幾項:
1. 即時顯示會員卡使用狀態(使用中/未使用)，包括使用者資訊及使用時間
2. 預約使用會員卡的時段，並顯示可預約的時段
3. 取消已預約的會員卡使用時段
4. 立即使用會員卡/結束使用會員卡的功能，即時更新使用狀態並傳送訊息到line 聊天室