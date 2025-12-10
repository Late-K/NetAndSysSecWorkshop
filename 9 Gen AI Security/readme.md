# LAB 9

Networks and Systems Security
Week 09
Gen AI Security

## Aims of the Seminar

This laboratory exercise introduces you to fundamental security
considerations in generative artificial intelligence. Students will deploy a
local large language model using Ollama and investigate key
vulnerabilities, threat categories, and defensive strategies highlighted in
the lecture material. The aim is to develop awareness of risks inherent in
generative systems and to practise core security evaluation procedures
in a controlled environment.

Learning Objectives:

- Demonstrate the ability to run a local LLM instance and evaluate
  its behaviour under controlled security-testing scenarios.
- Identify major generative AI threat vectors, including prompt
  injection, data poisoning, inversion, model theft, and adversarial
  manipulation.
- Apply basic red-teaming principles to assess the robustness and
  safety of a deployed model.
- Recommend high-level mitigation strategies based on security
  best practices for model deployment, governance, and incident
  response.

## Resources

Ollama Library
https://github.com/ollama/ollama

Ollama is an open-source platform for running large language models (LLMs) locally
on your own computer (Windows, macOS, or Linux). It provides a simple command-line
interface (CLI) and an API for downloading, running, and managing various open-source
models, ensuring privacy and security by keeping data on your local machine.

## Final Conclusion and Reflection

By deploying local models through Ollama, systematically testing them against a range of scenarios and techniqies, I gained a clearer understanding of both the strengths and limitations of lightweight LLMs. I enjoyed testing the two models to see these strengths and weakneses for myself, where i found that despite both being highly capable of answering basic questions, they consistently showed vulnerabilities, mainly with prompt injection, hallucination, and inconsistent behaviour. This showed me how easily generative models can be manipulated or coerced without strong policies in place.

Clearly small open source models lack the proper built in safety mechanisms necessary to keep themselves secure, leading to sometimes quite hilarious hallucinations and personas adopted by the models to try and follow impossible instructions. At the same time, the differences between the two models highlighted how capability correlates with both reliability and ease of cloning behaviour.
