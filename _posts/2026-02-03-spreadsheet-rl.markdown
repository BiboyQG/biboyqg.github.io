---
layout: post
title: "Spreadsheet-RL: Advancing Large Language Model Agents on Realistic Spreadsheet Tasks via Reinforcement Learning"
date: 2026-05-21 22:21:59 +00:00
image: /images/spreadsheet-rl.png
categories: publications
author: "Banghao Chi"
authors: "<strong>Banghao Chi*</strong>, Yining Xie*, Mingyuan Wu*<sup>&dagger;</sup>, Jingcheng Yang, Jize Jiang, Zhaoheng Li, Shengyi Qian, Minjia Zhang, Klara Nahrstedt, Rui Hou, Xiangjun Fan, Hanchao Yu"
venue: "arXiv preprint"
paper: https://arxiv.org/abs/2605.22642
code: https://github.com/Spreadsheet-RL/Spreadsheet-RL
website: https://spreadsheet-rl.github.io/
dataset: https://huggingface.co/datasets/Spreadsheet-RL/Spreadsheet-RL
---

We present Spreadsheet-RL, an end-to-end reinforcement learning post-training framework for spreadsheet agents in a realistic Microsoft Excel environment. Spreadsheet-RL combines automated construction of paired start-goal spreadsheet tasks, Spreadsheet Gym for multi-turn tool-based interaction, and GRPO training with outcome-based rewards. On SpreadsheetBench, it improves Qwen3-4B-Thinking-2507 Pass@1 from 12.0% to 23.4%; on Domain-Spreadsheet, it raises Pass@1 from 8.4% to 17.2%.

\* Equal contribution. <sup>&dagger;</sup> Project lead.
