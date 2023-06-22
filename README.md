## llmlite

**Vision — beyond go-openai**

[go-openai](https://github.com/sashabaranov/go-openai) is a popular OpenAI ChatGPT client for the Go programming language. 
One might start playing with it by simply submitting prompts to ChatGPT API. But to utilize LLMs for production-grade projects, a lot of additional features might be needed:

- 🔭 **Observability** — keep track of prompt performance and latencies by recording LLM execution logs (with potential anonymization)
- ⚙️ **Better de-coupling** — hardcoding prompts and execution parameters is not a good practice. De-coupling them from your code would enable a number of features:
  - No vendor lock-in
  - A|B testing for prompts/parameters/execution engines
  - Interactions with prompt engineering tools
- 🚀 **Efficient execution** — to run LLMs faster and cheaper
  - Caching
  - Rate-limiting
  - Retries
- ⛩️ Prompt scripting with injection security

The list of features might go further to [langchain](https://github.com/hwchase17/langchain)-like orchestration territory or some other parts of the LLM stack outlined in the recent a16z [review](https://a16z.com/2023/06/20/emerging-architectures-for-llm-applications/).

The idea is to provide those features in a library that would bring all these features that would work well together. The current name `llmlite` is inspired by `sqlite`, which provides powerful database features as a library.



