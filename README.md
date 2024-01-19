# Exploring Azure OpenAI rate limiting
Azure OpenAI standard SKU has rate limits to control the amount of load on OpenAI.

The rate limiting model depends on:
1. The size of the requests sent to Azure OpenAI
2. The rate at which these requests are sent

Alongside the rate limits, there is also a charging model based also on the request size and request rate and it is easy to assume that these two are fully aligned.

Where things get more complicated is when using the completions extensions - where Azure Search is used in combination with Azure OpenAI
