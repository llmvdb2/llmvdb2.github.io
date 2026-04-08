**Title:**
<br/> Semantic Query Processing over Relations


**Abstract:**
<br/> Language models are making it possible to ask richer questions over relational data, but doing so efficiently remains difficult. Join-heavy queries, often over networked data, can produce large intermediate results that must be serialized into prompts and then fed into language models. This talk presents FFX (Fast Factorized eXecution), a query engine that combines factorized and vectorized execution to address this bottleneck.

The talk focuses on how FFX changes semantic query processing by keeping join intermediates compact, enabling semantic operators to serialize factorized intermediates and predict over their implied Cartesian products. Operators then produce predictions as flat output tuples and bypass having to first flatten the input relation. Empirically, and somewhat surprisingly, our evaluation shows that even non-reasoning models can often perform this Cartesian expansion accurately while still carrying out the semantic task. In our evaluation, FFX achieves an order-of-magnitude reduction in input tokens while maintaining the same accuracy and degrades more gracefully as context size increases.


**Bio:**
<br/> Amine Mhedhbi is an assistant professor at École Polytechnique de Montréal. His interests are in building and analyzing analytical and AI-driven data system architectures. His work includes tackling performance considerations, debuggability, interface design, and data applications. Amine received his Ph.D. in 2023 from the University of Waterloo. His research has been awarded a VLDB best paper award, a Microsoft Ph.D. fellowship award, and the University of Waterloo's Computer Science distinguished dissertation award.
