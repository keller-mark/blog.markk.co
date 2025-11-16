# How I am thinking about AI

🚧 work in progress; some sections more complete than others

_I like to think about this blog post as externalizing my thoughts on AI to free up space in my brain to think about other topics._


_I am sure these thoughts will evolve over time (and I may update this post over time)._


_Caveat: I have a CS background, but do not claim to be an AI expert._




## What does it mean to be "fluent in AI"?

I recently attended a career fair panel in which four high-up executives in big pharma companies discussed hiring for R&D positions.
The audience consisted of mostly PhD students and postdocs in bio/medicine broadly.
The topic of AI came up several times, and the panelists' response was basically "all applicants need to be fluent in AI".


But for students (and anyone else on the job market), what does "AI fluency" actually mean?
The panelists never addressed this, nor did they seem like they would be the right people to ask anyway, given that their high-up positions (and non-computational backgrounds) made them seem quite distant/disconnected from us in the audience.

<details>
  <summary>Aside: If you ask an academic, they will tell you that AI fluency means being able to respond "I can" to the following statements (<a href="https://doi.org/10.1016/j.caeai.2023.100126">Laupichler et al. 2023</a>):</summary>
    <ul>
      <li>tell if the technologies I use are supported by artificial intelligence.</li>
      <li>name examples of technical applications that are supported by artificial intelligence.</li>
    <li>explain the differences between human and artificial intelligence.</li>
    <li>explain the difference between general (or strong) and narrow (or weak) artificial intelligence.</li>
    <li>evaluate whether media representations of AI (e.g., in movies or video games) go beyond the current capabilities of AI technologies.</li>
    <li>name weaknesses of artificial intelligence.</li>
    <li>name strengths of artificial intelligence.</li>
    <li>describe risks that may arise when using artificial intelligence systems.</li>
    <li>describe advantages that can come from using artificial intelligence systems.</li>
    <li>describe the potential impact of artificial intelligence on the future.</li>
    <li>distinguish AI applications that already exist from AI applications that are still in the future.</li>
    <li>explain how AI applications make decisions.</li>
    <li>explain how machine learning works at a general level.</li>
    <li>describe how machine learning models are trained, validated, and tested.</li>
    <li>explain the difference between ’supervised learning’ and ’unsupervised learning’ (in the context of machine learning).</li>
    <li>explain how ’reinforcement learning’ works on a basic level (in the context of machine learning).</li>
    <li>explain how deep learning relates to machine learning.</li>
    <li>explain what the term ’artificial neural network’ means.</li>
    <li>critically evaluate the implications of artificial intelligence applications in at least one subject area.</li>
    <li>explain why data plays an important role in the development and application of artificial intelligence.</li>
    <li>describe why humans play an important role in the development of artificial intelligence systems.</li>
    <li>describe how some artificial intelligence systems can act in their environment and react to their environment.</li>
    <li>explain how sensors are used by computers to collect data that can be used for AI purposes.</li>
    <li>name applications in which AI-assisted natural language processing/ understanding is used.</li>
    <li>identify ethical issues surrounding artificial intelligence.</li>
    <li>explain what the term ’black box’ means in relation to artificial intelligence systems.</li>
    <li>describe how biases arise in AI systems.</li>
    <li>critically reflect on the potential impact of artificial intelligence on individuals and society.</li>
    <li>explain why AI has recently become increasingly important.</li>
    <li>explain how rule-based systems differ from machine learning systems.</li>
    <li>assess if a problem in my field can and should be solved with artificial intelligence methods.</li>
    <li>describe what artificial intelligence is.</li>
    <li>describe the concept of explainable AI.</li>
    <li>explain why data security must be considered when developing and using artificial intelligence applications.</li>
    <li>explain why data privacy must be considered when developing and using artificial intelligence applications.</li>
    <li>describe the concept of big data.</li>
    <li>give examples from my daily life (personal or professional) where I might be in contact with artificial intelligence.</li>
    <li>explain what an algorithm is.</li>
    <li>describe potential legal problems that may arise when using artificial intelligence.</li>
    </ul>
</details>


## What would I want a family member to know about AI?

In my personal life, I have also been thinking about this topic after a recent discussion with my parents about usage of AI in their (non-computational) workplaces.
It got me thinking, what do I want my family members to know about AI?
Similarly, if I had never studied computer science, what would I want a hypothetical non-CS version of myself to know about AI?


### Artificial Intelligence (AI) is an umbrella term for multiple things, but due to marketing is now synonymous with Large Language Model (LLM)


An LLM is technically a special case of deep learning, which is a special case of machine learning.
Historically, AI was a very broad term that encompassed not only machine learning but also topics in fields like neuroscience.


### LLMs perform next-token prediction

The "goal" of an LLM is to predict the next "token" (think word or phrase) in a sentence.
Some researchers have (controversially) referred to LLMs as ["Stochastic Parrots"](https://en.wikipedia.org/wiki/Stochastic_parrot) to try to highlight their limitations.

### Before asking an LLM, ask yourself: Does this question makes sense as a "language problem"?

<!-- Is your task language-based? Do previous tokens predict future tokens? -->


Before asking an LLM, I ask myself: **Does this task make sense as a language prediction or translation problem?** Is it plausible that the information I need was in the training dataset (assuming the training data consists of all text on the internet approximately one year ago)? Am I alright with the randomness inherent to LLM responses?

- English -> Code, yes it makes sense.
- Prediction of the weather? No, it does not make sense as a language prediction problem. The weather forecast today does not depend on the words in my prompt.
  - Caveat: LLM providers can integrate Web Search tools, but the model needs to recognize this and perform a web search before returning an answer.


### AI in education and the LLM-as-a-tool analogy: Would you allow a child to use a calculator to learn their times tables?

Many argue that we should think of LLMs as "just another tool" (or as ["normal technology"](https://knightcolumbia.org/content/ai-as-normal-technology)).
I think it can be useful to consider the calculator-for-math analogy when we think about using AI in education.


Think back to when you were a student learning multiplication. Were you allowed to use a calculator when learning your times tables?


Think back to when you have taken standardized tests.
At least when I took the SAT, we were not allowed to use computers, and there were strict limits on what types of calculators could be used.
When I took the GRE, it was on a computer at a testing center, without access to the internet or any applications beyond the testing software.
Even if we view the AI as just another tool, it would be very appropriate to tightly restrict its usage in educational settings, especially in K-12 education.


Sure, eventually students are introduced to the TI-83, but this is not until the advanced math classes are reached.
If we extend this thinking to AI/LLMs, we should not be introducing them prior to being confident that students can read, write, and do critical thinking on their own.


Even as a computer science major in college, I had many CS/programming/algorithms classes in which exams were entirely on paper, no computers or phones in sight (albeit I graduated in 2019, squeaking out pre-COVID).
In addition to exam restrictions, I took several CS classes that had no-laptop policies: laptops were not allowed in class, even on non-exam days.
(If needed for health/accessibility reasons, disability accomodations could always still be made through a disability office on a case-by-case basis, just as they always have been.)
Post-pandemic, these policies may be more challenging to implement, but with AI such policies seem more necessary than ever.


### Randomness is inherent to LLMs

Are you alright with randomness in the response? Think of "hallucination" as a feature of LLMs, not a bug. It is just that sometimes, the hallucinations are useful.

This is why, for instance, they are good at generating text, but bad at generating URLs and DOIs (or other identifiers).
If I start typing `http://cnn.com/`, there are certain words (e.g., 'congress', 'conflict'), that are much more likely than others (e.g., 'lightbulb') to come next. So the LLM may have learned that certain places/positions in a URL or DOI always contains digits, for instance, but the inherent randomness will mean that the generated URL or DOI or other identifier is not actually valid.


(For the computational reader: sure, you can change the "temperature" of an LLM to reduce its randomness, but the average chat user has no clue about this.)


#### Code must be the intermediary if the problem requires determinism

_Note: this may be beyond the scope of AI fluency, especially for those without programming expertise._

While randomness is inherent to LLMs, the solution to this problem is to use an LLM to translate from human language (e.g., English) to an intermediate deterministic (e.g., code) representation.
Rather than asking an LLM to solve the problem end-to-end, stopping at producing code ensures that (1) the logic can be verified by a human, and (2) avoids the randomness problem (since re-running deterministic code ensures that, given the input, the same output will be produced).

Once in code form, not only are things deterministic, but all existing software development tools such as testing and version control can be used.

This point is tightly coupled to the fact that AI-for-coding (e.g., GitHub Copilot, Cursor) is has been of the most useful applications for LLMs: because English-to-Code translation "makes sense" as a language problem.

### LLMs use multiple levels of "context"

When using an LLM, it is important to understand the concept of "context".
Thinking back to how LLMs are just doing next-token prediction, the "context" refers to all of the previous tokens (i.e., words).

It is important to note that in any chatbot-type scenario, there are also words preceding your own, referred to as a ["system prompt"](https://github.com/x1xhlol/system-prompts-and-models-of-ai-tools).
You can think of the system prompt as hidden text that the LLM developer will inject before yours, in order to condition the next tokens in a certain way.
For instance, the system prompt may include suggestions for how the LLM should format its responses.


If you are using an LLM via an intermediary, such as a customer service chat on an e-commerce website, there may be multiple levels of system prompts injected before any end-user prompt: one from the LLM provider, then another from the e-commerce web developer.

#### Limits of context windows

It is also important to remember that there are limits to LLM context (in terms of the number of tokens), referred to as the "context window".
For current [open models](https://ollama.com/search), context window limits are generally ~2K-128K tokens (and typically increasing over time as new models are released).
For this reason, LLMs perform best on well-scoped small tasks, without a bunch of unrelated text cluttering the context window (the buzzword for this is ["context engineering"](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents)).


### LLMs are not good at creativity; they are optimized to produce the "average" prediction

It is inherent to an LLM that the training data is compressed in some way.
Current LLMs train on essentially the entire set of available text on the internet, yet their weights can typically be stored in tens to hundreds of gigabytes.
This has implications for anyone who hopes to use LLMs for creativity or brainstorming tasks.


#### Implications for AI detectors

Researchers have shown that the compressed nature of LLMs means that there are subtle patterns that can be exploited for detection.
However, as models become more advanced, these subtle patterns will become increasingly difficult to detect.
In these cases, techniques such as [watermarking](https://proceedings.mlr.press/v202/kirchenbauer23a/kirchenbauer23a.pdf) can be used to modify any LLM output in order to make its machine-generated nature detectable.
To learn more, see this [recent study](https://doi.org/10.48550/arXiv.2510.18774) that uses AI detection to reveal widespread undisclosed usage in journalism.
When sharing LLM-generated text without disclosing LLM usage, it is important to keep in mind that both detectors and watermarking techniques exist (and any closed-source LLM may be applying a watermark without your knowledge).


### Training data is old

Basically, assume the training data was collected approximately one year ago.

(This point is complicated by the fact that there are now MCP "tools", e.g., for web search.)


This makes LLMs bad for those tasks that require up-to-date information.
As an example, when using LLMs for code autocompletion in software development, the LLM will naively suggest versions of dependencies that are often already outdated.
As such, it is important to always check the current latest version (e.g., by using the package repository such as NPM or PyPI as the source of truth).


#### Implications for "greenfield" software development

_Note: this section goes beyond the scope of AI fluency for those without programming expertise._

Software developers like to say that LLMs are more useful for fresh projects, compared to large legacy codebases.
While this is true, there is an important caveat: LLMs are bad for the initial setup ("scaffolding") of a codebase, due to both their outdated training data and their tendency towards the "average" output.
The scaffolding produced by LLMs will therefore stray from current best practices and dependency versions.



Therefore, when starting a new software repository, even if intending to use an LLM, it is best to manually start the repo/configuration yourself, typically using a scaffolding CLI tool.
For example, for a Vite (web development) project, it is best to use the `create vite@latest` [CLI](https://vite.dev/guide/#scaffolding-your-first-vite-project).


### All training data is biased, the question is towards/against what (and to what extent)



### Be wary of prompt injection

The "lethal trifecta": https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/


### Things written before 2022 (/release of ChatGPT) is much more certain to be human-generated. Beyond 2022, keep a healthy level of skepticism.

2022 will forever be the year that writing/reading changed.
I am already considering limiting the books that I read to pre-2022 moving forward.
I would prefer to focus on the substance of text, and to not also constantly be asking myself: has this text been written by a human, AI, or some mixture of both?

### There are environmental costs to training and using LLMs


While small individually, the costs are clearly large in aggregate as we observe the boom in data center construction around the country/world.
See Google's [environmental impact analysis](https://arxiv.org/abs/2508.15734).


### Closed vs. Open-weight vs. Open-source LLMs

<!-- Could also mention local vs. hosted. --> 

See https://opensource.org/ai/open-weights

### Model weights can be manipulated

While to some extent LLM models are black boxes, there are ever-increasing efforts to probe models and develop methods for [interpretability](https://transformer-circuits.pub/2024/scaling-monosemanticity/).
It is important to remember that there is nothing stopping LLM developers or providers from manipulating model weights to prefer certain outputs over others.
In the best case, providers may do so to ensure AI safety, but in the worst case, bad actors may manipulate model weights to further their own [interests](https://www.bbc.com/news/articles/c4g8r34nxeno).


### What is an agent?

See https://simonwillison.net/2025/Sep/18/agents/

### Sycophancy is a problem for LLMs

It is in the best interest of LLM providers that their products appeal to human users.
In doing so, [sycophancy](https://www.nature.com/articles/d41586-025-03390-0) has become a problem.
(This is related to the contents of system prompts as well as how the model is rewarded during training.)


### PDFs are hard for machines to read

Do not assume PDF contents can be extracted completely/correctly.
See below section about Language models for science.

### What is data poisoning?

See https://www.cs.umd.edu/~tomg/projects/invisible/





### Neural networks are universal function approximators

NN as universal function approximation. Start with Y = mx+b defines a line. NN does this, but for an arbitrary function / decision boundary.


### How does a vision language model work?

Language models perform "next-token" prediction.
For standard text-based models, tokens can be thought of as words.
For vision (i.e., image-generation) models, each token can be thought of as a "tile" of pixels.
Just like how a text-based model predicts subsequent words to build up a sentence, vision models predict subsequent tiles of pixels to build up a larger image.


### What is model collapse?

See https://www.nature.com/articles/s41586-024-07566-y


## Other AI thoughts

The following sections are less related to general AI fluency and instead are more likely to be geared for a computational audience, but since they are related to AI, why not share them here anyway.

### Writing as thinking

> Writing, to me, is simply thinking through my fingers.
>
> -- Isaac Asimov

### Language models for science

There is currently a ton of hype around the idea that language models can replace scientists.
Yet there is plenty of reason to be skeptical.

#### The literature lacks many negative results

The current incentives for authors of scientific publications remain overwhelmingly biased toward publishing only positive results.
This means that for machine learning and AI, there is a major class imbalance problem between the positive and the negative.
The problem is even more acute in certain fields, such as chemistry, in which understanding which reactions do not work can be equally as important as understanding which do work.

#### Reasoning about figures and diagrams

Many key results and data points within papers are only found within figures.
Currently, many approaches only extract paper text and consider this to be "the paper" in the context of the language model.

#### The PDF problem

The majority of the world's scientific knowledge is locked up within PDF files.
This is due to current publishing incentives in which authors aim to publish in journals and conferences to advance their careers, each which has its own formatting requirements, and most of which still publish papers in PDF form.
It is also due to the nature of the PDF format, which lacks semantics.
The world still lacks tools to extract high-quality text from PDFs.


If you have ever tried to extract text from a PDF using the most commonly recommended tools of PyMuPDF, pypdf, or even [science-parse](https://github.com/allenai/science-parse), then you know how challenging it can be.
[OlmOCR](https://olmocr.allenai.org/) is currently one of the top open-source methods, but still suffers from problems.
Current approaches extract text from each page individually, which means that elements such as headers, footers, and figure captions clutter the results, often appearing abruptly within sentences that span page breaks.

#### Opportunities

The PDF problems are probably the lowest hanging fruit.
The problems with headers, footers, and interleaved figures can likely be addressed by additional language model passes.
After all, if they are this easy to spot for a human, they probably stick to predictable patterns.


Perhaps the figure/diagram reasoning problem can be addressed through methods such as vision transformers.
Otherwise, the visualization research community is currently racing to understand how language models reason about plots, so this too may not be too far off.


The lack of negative results (as well as the presence of false positive results) is probably the most challenging of these problems to solve.
Perhaps it will take lab-in-the-loop approaches and advancements in lab automation.


In the meantime, I am not going to spend too much time getting excited or worried about AI scientists until the quality of text and figures that can be extracted from PDFs of scientific articles improves significantly.

### MCP is an admission that LLMs can't do everything

MCP is an admission by AI companies/big-tech that LLMs are not the "everything machines" that they are constantly marketed as. They sometimes need adaptors. That is ok, but it is also something to think about.




### LLMs lower the cost of code that previously required a library; LLMs increase developer confidence (too much?)

As it has now become very low cost to generate code using LLMs, it lowers the barrier to asking the LLM to generate utility (or other low-level) functions that a developer would have historically reached for a library to achieve.


This has advantages and disadvantages.
For instance, from a security perspective (on my mind given recent NPM package incidents), a widely-used and well-established library may be more likely to have already resolved glaring security issues.
But at the same time, if every app has its own, slightly different implementation of some function(ality), say `foo`, then a malicious actor cannot target everyone's app via the strategy of targeting some widely-used utility library that has a near-monopoly on `foo`. 


It will increase the amount of spaghetti/bad code, as developers become overconfident and ask for code that is too far outside of their level of expertise.


#### How does this all affect open-source software licensing?

If a fellow developer does not like the terms of an open-source license that applies to some code repository, what stops them from simply asking an LLM to vary the variable names and other code patterns to generate code that retains the same functionality but is now syntactically different enough in the eyes of the legal system to pass as an entirely separate codebase that now lacks any direct ties to the original repository.
This feels similar to other intellectual property concerns that have been raised by newspapers, book authors, and artists.
In the open-source realm specifically it could have implications for collaboration and sustainability of open-source projects which were [already facing a crisis](https://openpath.quest/2024/the-open-source-sustainability-crisis/).


#### LLMs are bad at abstraction

However it is interesting to consider that LLMs are (at least currently) bad at creating abstractions that reflect the bigger picture.

- It is still on the developer to recognize the value of an abstraction, such as when to go to the extra effort to create a reusable package for some code, and how to structure the end-user APIs.
In a way, this makes sense though, as the LLM is only doing what we ask, and we are generally asking for features that solve a specific problem in a specific codebase (we are not asking to solve a problem in-general, across many code-bases).


#### LLMs are bad at performance optimization

- LLMs are good at producing language that follows patterns, such as code. It really knows very little about the context of the code to be able to optimize it, such as which variables may store very large arrays, or which functions will take a long time to compute. Their training is optimized to produce the next tokens that are probable; there is nothing in the training process that would optimize for next-tokens that have good performance (besides maybe basic patterns or lack thereof in the training data, such as lack of many nested for loops).
- The LLM may be able to help optimize or analyze the big-O notation of a block of code, but only if you asked it to do so. It probably will not recognize "hot" code paths on its own without more context/prompting. There is some [evidence](https://doi.org/10.48550/arXiv.2511.04427) for this.


## Do you like seeing AI in your vision of the future?

I was recently asked, "How do you think your job will be changed by AI?" and subsequently, "Do you like that vision of the future?".

These were my responses to the latter question:

- I am worried about the societal implications of AI, such as deepfake images/videos/calls, cybersecurity, job losses, and education impacts. https://bsky.app/profile/masonfromtwitter.bsky.social/post/3lu3m36wlak2u
  - Two things can be true: AI can simultaneously be useful for certain tasks (e.g., language translation, writing code) while at the same time being harmful to society. The main questions are: do the benefits outweigh the risks? and what will it take for goverments to implement sufficient guardrails (if they ever get past the AGI-race mentality)?
- I don't like that dedication of so much interest/human-energy to LLMs/chatbots comes at the cost of not pursuing other interesting projects (e.g., non-LLM-based CS/machine learning/bioinformatics).
  - It is unnerving that in academia, funding agencies (and their study sections which are supposed to be panels of experts on specific topics that guide grant funding and decide how tax dollars are spent) seem to have bought into hype around AI just as much as everyone else. (There are of course exceptions, and there are plenty of people doing great research on AI. For instance, I particularly like the [Ai2 Paper Finder](https://allenai.org/blog/paper-finder) tool).
- I am worried about the loss of critical thinking skills, on both collective and individual levels. 
- I don't like the environmental costs (energy and water).
  - May be miniscule per-prompt, but as a whole it is having a major impact, especially with companies racing to integrate AI into everything without first considering whether it is useful.
  - I have switched to using Gemini (Flash/Pro) via Copilot or the Harvard AI Sandbox, since they published their [environmental impact paper](https://arxiv.org/pdf/2508.15734). I like the transparency and I suspect that Google has much more experience at scaling infrastructure efficiently, compared to the newer startups such as OpenAI/Anthropic/etc which are also reported to be chaotic workplaces. (There are also many disadvantages to going with the Google/big-tech option. For instance, I do not want them to own yet more aspects of my data when they already have search history, email, photos, docs, slides, etc. and given their ad-driven business model.)
- I don't like the intellectual property aspects (lack of proper credit, hallucination of references, risks to open-source ecosystem).
- I don't like to constantly be questioning whether text or code that I am reading was AI-generated (on top of trying to understand the content). (Keep in mind that articles _about_ AI that argue _in favor_ of AI are especially likely to be at least partially AI-generated.)





## Other AI-related readings

But wait! 
When reading about AI, it is especially important to ask oneself: Who is writing/publishing this?
Do they have an obvious conflict of interest (e.g., is it someone from an AI company telling me that AI will revolutionize education or some other field)?
If so, take it with a grain of salt.

- https://www.youtube.com/watch?v=e70RT6c01M8
- https://www.nplusonemag.com/issue-51/the-intellectual-situation/large-language-muddle/
- https://www.newyorker.com/culture/open-questions/what-if-ai-doesnt-get-much-better-than-this
- https://cdh.princeton.edu/blog/2025/08/12/ted-chiang/
- https://www.normaltech.ai/p/could-ai-slow-science
- https://www.foundationwebdev.com/2025/07/opinion-is-the-use-of-ai-worth-it/
- https://apnews.com/article/electricity-prices-data-centers-artificial-intelligence-fbf213a915fb574a4f3e5baaa7041c3a
- https://openai.com/index/why-language-models-hallucinate/
- https://www.shloked.com/writing/claude-memory
- https://www.youtube.com/watch?v=Vz0oQ0v0W10
- https://www.technologyreview.com/2025/10/30/1127057/agi-conspiracy-theory-artifcial-general-intelligence/
<!-- - https://arxiv.org/abs/2508.15734 -->
<!-- - https://doi.org/10.1145/3442188.3445922 -->

On AI in education:
- https://www.economist.com/podcasts/2025/09/20/we-dont-need-no-ai-education
- https://statmodeling.stat.columbia.edu/2025/07/18/i-am-no-longer-chairing-defenses-or-joining-committees-where-students-use-generative-ai-for-their-writing/
- https://www.ted.com/talks/advait_sarkar_how_to_stop_ai_from_killing_your_critical_thinking

On AI in software development:
- https://www.phillipcarter.dev/posts/coding-with-llms
- https://blog.genesmindsmachines.com/p/llms-excel-at-programminghow-can


