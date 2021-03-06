Approximate computing is the idea that we are hindering computer systems' efficiency by demanding too much accuracy from them. While precision is crucial for some tasks, many modern applications are fundamentally approximate. Perfect answers are unnecessary or even impossible in domains such as computer vision, machine learning, speech recognition, search, graphics, and physical simulation. Today's systems waste time, energy, and complexity to provide uniformly pristine operation for applications that do not require it.

Resilient applications are not, however, a license for computers to abandon predictability in favor of arbitrary errors. We need abstractions that incorporate approximate operation in a disciplined way. Application programmers should be able to exploit these richer abstractions to treat accuracy as a resource and trade it off for more traditional resources such as time, space, or energy.

This dissertation explores new abstractions for approximate computing across hardware and software. It develops these abstractions from two perspectives: from the point of view of programmers, where the challenge is constraining imprecision to make it acceptable, and from a system perspective, where the goal is to exploit programs' constraints to improve efficiency. For approximate programming, this dissertation proposes:

- a type system that uses information flow to separate an application's error-resilient components from its critical control structures;
- an extended type system that restricts the probability that a value is incorrect, along with type inference and optional dynamic tracking for these probabilities; and
- a construct for expressing probabilistic constraints on programs along with a technique for verifying them efficiently using symbolic execution and statistical properties.

For approximate execution, it describes:

- two mechanisms for trading off accuracy for density, performance, energy, and lifetime in solid-state memory technologies; and
- an end-to-end compiler framework for exploiting approximation on commodity hardware, which also serves as research infrastructure for experimenting with new approximation ideas.
