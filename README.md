i# Generative AI & AI _newsletter_15.04


## 🚀  AI News 

### Hugging Face got hacked 
Wiz researchers discovered architecture risks that may compromise AI-as-a-Service providers and put customer data at risk. 
Wiz and Hugging Face worked together to mitigate the issue.
- https://www.wiz.io/blog/wiz-and-hugging-face-address-risks-to-ai-infrastructure
- https://youtu.be/ZcoOW8nqVP8?feature=shared

### HuggingChat 

https://apps.apple.com/fr/app/huggingchat/id6476778843


### AI developments this week :

- Meta’s Llama 3, the next iteration of the open-access Llama family, is now released and available at Hugging Face. 
https://huggingface.co/blog/llama3
https://www.databricks.com/blog/building-enterprise-genai-apps-meta-llama-3-databricks
https://x.com/karpathy/status/1781028605709234613?s=46

- Moirai: A Time Series Foundation Model for Universal Forecasting, 
a groundbreaking TS foundation model by Salesforce. MOIRAI is awesome in terms of performance — but more importantly, the authors have pledged to open-source the model and its training dataset! https://blog.salesforceairesearch.com/moirai/

- Mixtral 8x22B open model. https://mistral.ai/fr/news/mixtral-8x22b/
It sets a new standard for performance and efficiency within the AI community. It is a sparse Mixture-of-Experts (SMoE) model that uses only 39B active parameters out of 141B, offering unparalleled cost efficiency for its size.
Mixtral 8x22B comes with the following strengths:
  * It is fluent in English, French, Italian, German, and Spanish
  * It has strong mathematics and coding capabilities
  * It is natively capable of function calling; along with the constrained output mode implemented on la Plateforme, this enables application development and tech stack modernisation at scale
  * Its 64K tokens context window allows precise information recall from large documents

  
## 🎯 A Little guide to building Large Language Models in 2024 
This is a post-recording of a 75 min lecture on how to train a LLM from scratch in 2024 made by Thom Wolf - Hugging Face 
 - https://huggingface.co/posts/thomwolf/706415412818350
 - https://youtu.be/2-SPH9hIKT8?feature=shared

Concepts/tools/techniques for training good performance LLM explained by Thom Wolf 
* Step 1 : Finding, preparing and evaluating web scale data
  * Datasets examples : Cosmopedia v1.0  https://github.com/huggingface/cosmopedia , Starcoder2  https://github.com/bigcode-project/starcoder2/
  * Filter Data tools by Meta : https://fasttext.cc/
  * Process and deduplicate text data at a very large scale: https://github.com/huggingface/datatrove
  * Evaluating the data with Face LightEval is a lightweight LLM evaluation : https://github.com/huggingface/lighteval

* Step 2 : Understanding model parallelism and efficient training
  * 4D Parallelims : Data Parallelism, Tensor Parallelism, Pipeline Parallelism, Sequence Parallelism  : https://docs.aws.amazon.com/sagemaker/latest/dg/model-parallel-intro.html#model-parallel-intro-sdp
  * Capacity and architecture : MOE (Mixed of experts), Mamba : https://youtu.be/mwO6v4BlgZQ?feature=shared , https://youtu.be/9dSkvxS2EB0?feature=shared
  * Nanotron The objective of this library is to provide tools to implement efficient training : https://github.com/huggingface/nanotron
  
* Step 3 : Fine-tuning/aligning models
  * RLFH - Reinforcement learning from human feedback old fashion : https://www.youtube.com/live/2MBJOuVq380?feature=shared
  * DPO - Direct Preference Optimization new way to align model : https://youtu.be/XZLc09hkMwA?feature=shared

* Step 4 : Fast inference / deploy the model
  * Quantization - https://huggingface.co/blog/4bit-transformers-bitsandbytes
  * Speculative Decoding - Medusa : https://youtu.be/hMs8VNRy5Ys?feature=shared

*  Step 5 : Share the model with the world 
   *  https://chat.lmsys.org/?leaderboard
 

## 🎯 Focus on Generative Arts 

### Video Poet 
To showcase VideoPoet's capabilities, we have produced a short movie composed of many short clips generated by the model. For the script, we asked Bard to write a series of prompts to detail a short story about a traveling raccoon. We then generated video clips for each prompt, and stitched together all resulting clips to produce the final YouTube Short below
- https://www.youtube.com/shorts/70wZKfx6Ylk
-https://sites.research.google/videopoet/

### LATTE3D 
The LATTE3D model rapidly transforms text prompts into high-quality 3D shapes that could help populate virtual worlds.
- https://blogs.nvidia.com/blog/latte-3d-generative-ai-research/


## 📖 AI Learning / Courses 

### Blog - Agentic Design Patterns 
- https://www.deeplearning.ai/the-batch/how-agents-can-improve-llm-performance

###  Preprocessing Unstructured Data for LLM Applications
Learn to extract and normalize content from a wide variety of document types, such as PDFs, PowerPoints, Word, and HTML files, tables, and images to expand the information accessible to your LLM.
- https://www.deeplearning.ai/short-courses/preprocessing-unstructured-data-for-llm-applications/

### Quantization Fundamentals with Hugging Face
Generative AI models, like large language models, often exceed the capabilities of consumer-grade hardware and are expensive to run. Compressing models through methods such as quantization makes them more efficient, faster, and accessible. This allows them to run on a wide variety of devices, including smartphones, personal computers, and edge devices, and minimizes performance degradation.
- https://www.deeplearning.ai/short-courses/quantization-fundamentals-with-hugging-face/

