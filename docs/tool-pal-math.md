### ⛓️LangFlow example:

![Description](img/tool-pal-math.png#only-dark)
![Description](img/tool-pal-math.png#only-light)

[Get JSON file](data/Tool_pal_math.json){: .md-button download="Tool_pal_math"} 

## Nodes

`ZeroShotPrompt` is a tool that allows you to create a prompt template for Zero-Shot Agent. You can set the *Prefix* and *Suffix*. The *Prefix* is the text that will be added before the input text. The *Suffix* is the text that will be added after the input text. In the example, we used the *default* that is automatically set.

We used `OpenAI` as the LLM, but you can use any LLM that has an API. Make sure to get the API key from the LLM provider. For example, [OpenAI](https://platform.openai.com/){.internal-link target=_blank} requires you to create an account to get it yours.

Check the short tutorial of [OpenAI](llms.md){.internal-link target=_blank} options available.

The `LLMChain` is a simple chain that takes in a prompt template, formats it with the user input, and returns the response from an LLM.

`PAL-MATH`, is a language model that is good at solving complex math problems. The input should be a fully worded hard-word math problem.

`ZeroShotAgent` is an agent Agent for the MRKL chain. It uses a Zero Shot LLM to generate a response.