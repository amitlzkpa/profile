# Type Safety: Safety wheels or crutches that keep you from leaning into a turn?

Hey there, fellow tech enthusiasts! Today, I've got something on my mind that I can't help but ponder – the ever-controversial topic of type safety. So, grab your virtual thinking caps, and let's open up for some "technical yellow-journalism".

## Types and Data: A Delicate Dance

Let's clarify what we mean by "type safety". It's the practice of ensuring that data in your code is used in ways that are consistent with types defined in the project.

To set the stage, let's break down a unit of computation into two parts: the logic and the data. For now, let's focus on the data part. Data can enter, be processed, and exit a computation unit in various ways – think of it like a function with multiple arguments, internal variables, and multiple return values.

Now, here's the crux of my pondering: Does associating types (especially non-nullable ones) with data provide airtight assurance, or is more like hoping the weatherman can predict the future? Sure, types are incredibly helpful when you're reading code, but can we be absolutely certain that data marked with a type is always used correctly?

## Comfort, Constraints and Alternatives for Type Safety

To position it in a more concrete example - imagine a function with well-defined types for inputs, outputs, and internal variables. You could establish pre and post conditions to ensure these variables always stay in line, somewhat akin to the assurance provided by type safety. However, custom-tailoring these checks within the context of the function might make it easier to grasp when reading the code. It's a matter of perception – a local rulebook versus a global library of types used throughout a project.

But here's where it gets tricky. What happens when a type that has served a codebase well suddenly needs to accommodate a new feature? Picture a scenario where you're tasked with upgrading a method named `convertToLocalCurrency` to return not only the converted amount but also the name of the currency. It's a desperate requirement for a new market which has multiple local currencies, but your codebase was initially designed for a market which has had a single currency for centuries.

Some might argue that this predicament stems from a poorly designed codebase in the first place. Yet, I'm not entirely convinced. Shouldn't our tools adapt to our needs rather than the other way around?

## Technical Debt: My debt, your debt, whose debt is it anyway?

So, the new developer on the team takes on the challenge and updates the method's return type to include the currency name. And lo and behold, errors start popping up all over the system. Suddenly, changing the type definition seems like an Everest-sized task. I won't delve into other potential solutions here; they might not be visible to this new developer just yet.

Fast forward a few weeks, and you're in a team meeting. Senior personnel are asking about that seemingly small change for the local currency name. The client's inquiring, the sales team is counting on it, and it's starting to feel like a ticking time bomb for the developer's job security. Meanwhile, the codebase's type correctness enthusiasts are engrossed in their own priorities.

Now, I'll admit this example is a bit far-fetched, but it's in an effort to raise a question – would it have been easier to implement local, in-context type checks for the function instead of imposing a system-wide type library? After all, regardless of the approach, test cases and system-wide changes will need updates. And let's face it, how many of us really start by inspecting every type in a codebase when we dive into a new project?

## Conclusion: Resistant to Change?

Well, there you have it – my tech ponderings of the day. We know about the trusty training wheels, but have you ever thought of [balance bikes](https://en.wikipedia.org/wiki/Balance_bike)? That's my rant for the day and hope it was spicy enough for you to retort ;)
