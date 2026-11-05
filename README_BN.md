# AI Builder Studio — বাংলা গাইড

Build reliable AI applications with provider-aware architecture, safe data handling, evaluation, user-centered UX, and explicit separation between model capabilities and configured external services.

## ব্যবহারের নিয়ম

এই Repository-তে একটি মাত্র Selectable Master Skill আছে: `ai-builder-studio`। বাকি 13টি Specialist Module তার `references/` ফোল্ডারে Internal Playbook হিসেবে থাকবে। প্রতিবার আলাদা আলাদা Skill নির্বাচন করতে হবে না।

## ব্যবহার

Claude Code:
```text
/ai-builder-studio
```

OpenCode:
```text
@ai-builder-studio
```

প্রথমে Project-এর বর্তমান ফাইল, নির্দেশনা, Dependencies ও Tools পরীক্ষা করতে হবে। প্রয়োজনীয় Reference Module নিজে নির্বাচন করে Master Skill সম্পূর্ণ Workflow চালাবে।

## গুরুত্বপূর্ণ

এই Repository AI Model বা API দেয় না। বাইরের Provider, API Key, Tool, Permission, Dependency ও Hardware প্রয়োজন হলে সেগুলো আলাদাভাবে Configure করতে হবে। কাজ সত্যিই Build/Test/Generate না হলে Agent সেটি সম্পন্ন হয়েছে বলে দাবি করতে পারবে না।

বিস্তারিত ইংরেজি নির্দেশনা: [README.md](README.md)।
