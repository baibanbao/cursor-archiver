---
tags:
  - sora
---
# Jim Fan



I see some vocal objections: "Sora is not learning physics, it's just manipulating pixels in 2D".

I respectfully disagree with this reductionist view. It's similar to saying "GPT-4 doesn't learn coding, it's just sampling strings". Well, what transformers do is just manipulating a sequence of integers (token IDs). What neural networks do is just manipulating floating numbers. That's not the right argument.

Sora's soft physics simulation is an *emergent property* as you scale up text2video training massively.

- GPT-4 must learn some form of syntax, semantics, and data structures internally in order to generate executable Python code. GPT-4 does not store Python syntax trees explicitly.

- Very similarly, Sora must learn some *implicit* forms of text-to-3D, 3D transformations, ray-traced rendering, and physical rules in order to model the video pixels as accurately as possible. It has to learn concepts of a game engine to satisfy the objective.

- If we don't consider interactions, UE5 is a (very sophisticated) process that generates video pixels. Sora is also a process that generates video pixels, but based on end-to-end transformers. They are on the same level of abstraction.

- The difference is that UE5 is hand-crafted and precise, but Sora is purely learned through data and "intuitive".

Will Sora replace game engine devs? Absolutely not. Its emergent physics understanding is fragile and far from perfect. It still heavily hallucinates things that are incompatible with our physical common sense. It does not yet have a good grasp of object interactions - see the uncanny mistake in the video below.

Sora is the GPT-3 moment. Back in 2020, GPT-3 was a pretty bad model that required heavy prompt engineering and babysitting. But it was the first compelling demonstration of in-context learning as an emergent property.

Don't fixate on the imperfections of GPT-3. Think about extrapolations to GPT-4 in the near future.