## Types of AI

```
let's add a section for deep learning as well
would be good to discuss an example under each of these

Also, what do you think is the more appropriate title for this section? Should it be types of AI or various approaches to AI?
```

AI is a broad term that has evolved overtime. The purpose here is to understand the necessary types of artifacts, constructs, and models that AI provides to make software applications intelligent. Although, this list is long, let's confine te discussion to two broad categories, namely rule-based AI and machine learning.

### Rule-based AI
Rule-based AI is considered a simple technique that tries to represent the domain knowledge and inference rules to draw conclusions. For example, consider the situation where we need to represent the rule "all men are mortal" in a way that it can be used to draw new inferences. It can be represented using the following predicate logic:

- ∀ X man(X) → mortal(X) (read as "for all X, if X is a man, then X is mortal". Here X is a variable)

This rule can be used in combination with domain knoelwedge to draw inferences. For example:

- man(socrates) (read as "socates is a man")

This predicate can be used with the above rule to draw the inference that "socrates is mortal".

The major limitation of this rule-based AI is that it can be used to build deterministic systems only where the data is small and rules are clear. Such systems cannot learn new things themselves.

### Machine learning
Machine learning on the other hand has the capability to define it's own rules based on data. The system can learn and adapt as new data emerges. This capacity to learn and adapt has made machine learning the most popular choice while integrating intelligence is software systems.
As an example, let's consider the question [this example is taken from Sebastian Thun's Intro to ML course on Udacity]

- "is horse an acerous?"

What is an acerous? Well, instead of answering this question directly, let's have a few examples that can help us learn this.

- An elephant is acerous
- A ram is non-acerous
- A triceratops is non-acerous
- A lemur is acerous
- A dog is acerous
- A giraffe is non-acerous
- A goat is non-acerous
- A cat is acerous
- A parrot is acerous
- A deer is non-acerous

Before answering this question, let's discuss the approach. We need to look at different features to decide. These features could be color, number of legs, and horns, etc. And it happens that a horse is an **acerous**. Why? Because a horse does not have either horns or antlers. Whereas, all the animals in non-acerous group have. This demonstrates the process and capability of machine learning to learn something new by itself as new data emerges.
