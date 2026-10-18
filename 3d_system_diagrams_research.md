# Three-Dimensional Mental Models and System Diagrams: A Case for Spatial Externalisation in Software Engineering

## Abstract

This paper examines the cognitive basis for three-dimensional (3D) mental representations of complex systems, with particular reference to software engineering and systems thinking. Drawing on research in spatial cognition, mental imagery, diagrammatic reasoning, and individual differences in cognitive style, I argue that a significant population of systems thinkers, particularly software engineers, naturally represent abstract relational structures as 3D spatial networks of connected nodes. I further argue that no adequate tool exists to externalise these representations, despite the need being identified as early as 1982 by computing pioneer Rear Admiral Grace Hopper. I assess the barriers to adoption of 3D diagram tools and argue that the primary obstacles are historical and cultural rather than fundamental cognitive ones, and that generational shifts in 3D navigation fluency may make such tools viable now in a way they were not previously.

---

## 1. Introduction

When people think about complex systems, whether software architectures, organisational structures, or causal networks, what form do those thoughts take? The question is less settled than it might appear. A substantial body of research in cognitive science suggests that the mind does not simply process abstract relational information linguistically or propositionally, but often represents it in a spatial format: an internal structure of entities and connections that can be navigated, rotated, and manipulated in mental space.

This paper explores a specific and underexamined variant of this phenomenon: people who report experiencing these mental representations as three-dimensional networks of connected shapes, essentially node-link diagrams occupying imagined 3D space. I argue that this experience is:

1. Cognitively well-grounded and supported by neuroscience
2. Particularly common among software engineers and systems thinkers
3. Underserved by existing diagramming tools, which are almost universally constrained to two dimensions
4. Something that Grace Hopper identified and attempted to address in 1982, with a physical prototype using chemistry molecule sets

The paper synthesises research across cognitive psychology, spatial cognition, diagrammatic reasoning, and HCI, and concludes with an argument for why the conditions may now be ripe for a genuine 3D diagram tool to emerge.

---

## 2. Mental Models and Relational Structure

The foundational framework for understanding how people represent systems internally is Philip Johnson-Laird's theory of mental models, developed in his 1983 book *Mental Models: Towards a Cognitive Science of Language, Inference, and Consciousness*. Johnson-Laird argued that humans apprehend the world by constructing internal replicas of the relationships among objects and events, the mind as a model-building device. Crucially, these models contain objects and relations, not the linguistic structures through which we learn about them. They are structural and relational at their core.

Jay Wright Forrester captured the same intuition more plainly:

> "The image of the world around us, which we carry in our head, is just a model. Nobody in his head imagines all the world, government or country. He has only selected concepts, and relationships between them, and uses those to represent the real system." (Forrester, 1971)

Johnson-Laird further established that mental models are *iconic* insofar as possible: their parts and relations correspond to those of the situations they represent. They are not pictures, but they are structural analogues. This distinction matters: a mental model of a software system need not look like a photograph of servers and cables; it may instead be an abstract spatial structure in which entities occupy positions and connections indicate relationships.

Importantly, mental models are distinct from mental imagery. As Johnson-Laird noted, it is not necessary to *visualise* something vividly to hold a mental model of it. Models are abstract structural representations, not sensory images. This creates space for a cognitive phenomenon that is neither purely verbal nor purely pictorial: spatial-relational thinking that operates through structural topology rather than visual surface.

---

## 3. Visual vs. Spatial Imagery: A Critical Distinction

A persistent confusion in the literature on mental imagery conflates two distinct capacities that have been experimentally dissociated: *object imagery* (vivid, pictorial, detail-rich) and *spatial imagery* (structural, relational, dynamic). The distinction was formalised by Kozhevnikov and colleagues in a landmark 2005 paper.

Their research identified that the category "visualiser" conceals two fundamentally different cognitive styles:

- **Object visualisers** generate vivid, photographic mental images. They encode images holistically as single perceptual units. They tend to be artists and designers.
- **Spatial visualisers** manipulate abstract structural representations. They process images analytically, part by part, attending to spatial relations rather than surface detail. They tend to be scientists and engineers.

The two types perform differently on abstract graph problems: object visualisers consider only the global shape of a graph and struggle to restructure it analytically, while spatial visualisers naturally attend to the relational structure, the topology, and can mentally reorganise it.

This finding is directly relevant to systems thinking. Someone who reports "seeing" a software architecture as a 3D structure of connected nodes is almost certainly a spatial visualiser in Kozhevnikov's sense. They are not experiencing photographic imagery of hardware; they are experiencing a spatial representation of *connectivity and relationship*, which is precisely what a system diagram encodes.

Later research established that spatial imagery and visual imagery are neurologically distinct, engaging different brain systems. Visual imagery involves perceptual detail and object properties; spatial imagery involves location, topology, and relational structure. The latter is more dynamic and more directly relevant to reasoning about systems.

---

## 4. The Neural Basis: Spatial Cognition Serving Abstract Thought

A convergent finding from neuroscience strengthens the picture. Research on mental models has shown that reasoning about abstract relational structures recruits the same neural systems used for spatial navigation, particularly the hippocampal-entorhinal complex and parietal cortex.

One study found that transitive reasoning using mental models relies on neural mechanisms associated with spatial cognition, independent of whether the content is actually spatial (Goodwin & Johnson-Laird, 2005; van der Henst, 2002). A broader theoretical framework proposes that neurons coding for positions in physical space are *recycled* to represent locations in abstract conceptual spaces, meaning the brain's spatial machinery is repurposed for abstract relational thought.

This has a striking implication: people who report navigating abstract systems as though moving through a 3D space may be doing something neurologically literal. The hippocampal place cells and grid cells that encode physical location may genuinely be encoding positions in a relational structure, nodes in a graph, using the same computational machinery.

This framework also explains why spatial visualisers excel at systems reasoning. Their well-developed spatial navigation machinery provides a powerful substrate for holding and manipulating abstract relational structures. The 3D node-link model is not a metaphor for how they think; it may be a direct description of the neural representation.

---

## 5. Diagrammatic Reasoning and the Externalisation Imperative

The philosopher and logician Charles Sanders Peirce argued that all necessary reasoning is diagrammatic: that thinking proceeds by constructing and manipulating structured representations, internal or external. His existential graphs formalised this idea: areas representing concepts, lines representing relations, operations of insertion and deletion representing inference.

Modern research on diagrammatic reasoning has extended this insight. The primary function of diagrams, on this account, is not communication but *cognitive externalisation*: offloading relational structure from working memory into a physical or digital medium where it can be inspected, manipulated, and extended beyond the limits of internal representation.

This externalisation function is distinct from the communication function. A diagram used to communicate a system architecture to a colleague serves a different purpose from a diagram used to extend one's own mental model of that architecture. Existing diagramming tools, such as Lucidchart, draw.io, Visio, Mermaid, and their kin, are designed primarily for communication: producing artefacts to share. They are poorly suited to the exploratory, generative use case in which a spatial thinker is trying to externalise and extend a mental model that already has structure and dimensionality.

Barbara Tversky's research on the spatial nature of thought connects these threads. She argues that at the abstract level of systems design, what matters are components and their interconnectivity, and for that, nodes and links are the natural representation. The spatial externalisation of thought into diagrams is not arbitrary convention but reflects the underlying structure of the mental model.

---

## 6. Grace Hopper's 3D Prototype: A Historical Precedent

In a 1982 lecture to NSA personnel entitled "Future Possibilities: Data, Hardware, Software, and People," Rear Admiral Grace Hopper described in concrete terms her need for three-dimensional system diagrams and her attempts to build them:

> "I decided that if I was going to have systems of computers, I'd need three dimensional flow charts. So I got some plastic plates and I could draw charts on each one, pile them up, looked like three dimensional chess. When I connected between the plates, I used little pieces of string and Scotch tape, but they fell off. Finally I remember tinker toy and got a nice tinker toy set and it had to square things and round things and sticks to put them together and I started building three-dimensional flow charts."

Hopper went further, proposing a colour-coded node system using chemistry molecule sets:

> "Get some of those sets the chemist used to show you molecules. Red balls can be computers, blue balls can be databases, yellow balls database managers, green balls switches. And you can build a model of a system of computers and how they communicate and which ones are connected to which others. And you're going to have to get out of the plain of the paper. You can't write, draw em on flat paper anymore. They've got to be in three dimensions."

This is a remarkable passage. Hopper was not speaking metaphorically or speculatively. She had physically built 3D node-link models of computer systems, encountered their limitations (pieces fell off; she ran out of nodes), and was proposing a better physical medium. She identified the colour-coded node-type convention, a standard feature of modern UML and architecture diagrams, and explicitly located the problem: flat paper is no longer adequate for representing systems of the complexity she was working with.

Hopper was, by any assessment, a high spatial visualiser. Her pattern of thinking, insisting on physical, tangible representations of abstract structures, reaching for 3D when 2D failed, reasoning by analogy through physical models, is characteristic of the spatial cognitive style Kozhevnikov's research would later characterise. Her 1982 observation predates the formal cognitive science by two decades, but is entirely consistent with it.

---

## 7. Why 3D Diagram Tools Have Not Succeeded

Given Hopper's identification of the need in 1982, the cognitive science supporting it, and the obvious commercial opportunity, why has no successful 3D system diagram tool emerged?

Several barriers have historically combined to prevent uptake.

### 7.1 The Display-Input Mismatch

The fundamental difficulty of 3D visualisation on 2D screens is not cognitive but ergonomic. Hopper's physical Tinker Toy model could be walked around, rotated by hand, and inspected from any angle with zero cognitive overhead. A 3D graph on a flat monitor requires constant camera management, rotating the viewpoint, zooming, managing occlusion, which competes directly with the cognitive work of thinking about the system. Early research on 3D graph drawing found that for most tasks and most users, 2D layouts outperformed 3D ones on standard screens, precisely because of these interaction costs.

This is a hardware problem, not a fundamental cognitive one. The conclusion that "3D diagrams don't work" conflates "3D diagrams don't work on 2D screens with mouse input" with a more general claim that is not supported.

### 7.2 Research Population Bias

The experimental literature on 3D graph visualisation largely tested adults who learned computing in a 2D-native environment and had decades of established 2D spatial habits. These participants found 3D navigation cognitively expensive because it was unfamiliar. This finding has been overgeneralised as a universal cognitive constraint.

Younger users who have grown up navigating 3D environments in games such as Minecraft and Roblox have deeply internalised 3D spatial navigation on flat screens. For this population, the overhead that made 3D graphs unworkable in 1990s studies may simply not exist. The generational shift in baseline 3D navigation fluency has not been adequately reflected in the HCI literature on diagram tools.

### 7.3 Tool Design by Non-Spatial Visualisers

Diagramming tools are overwhelmingly designed by and for people who think in 2D hierarchies and flowcharts, a design population that skews toward verbal thinkers and object visualisers. Spatial visualisers who naturally think in 3D relational structures are underrepresented in product design roles, in part because their cognitive style is less well suited to the verbal communication demands of design processes, and in part because they have historically worked around the limitation by maintaining their models mentally.

The result is a self-reinforcing gap: those who most need 3D externalisation tools have the least influence over what gets built, and those who build tools do not experience the need.

### 7.4 The Externalisation Use Case is Invisible

Existing diagramming tools are designed for communication, producing artefacts that can be shared and read by others. The externalisation use case, a spatial visualiser recording and extending their own mental model, is different in character and has different requirements. It prioritises rapid capture, spatial freedom, and the ability to navigate and extend a structure, rather than the production of a clean, readable diagram for an audience.

This use case is largely invisible in user research because it happens internally. A spatial visualiser who builds a mental model of a system and then draws a flat diagram for their team has already done the cognitive work privately. The tool never sees the 3D model; only the 2D projection is recorded. The gap between what was thought and what was drawn is never measured.

### 7.5 The Bootstrapping Problem

Spatial visualisers who would benefit from 3D externalisation tools are often highly capable reasoners who have developed extensive compensatory strategies, such as breaking large mental models into sub-models, using sketches as memory aids, and maintaining spatial structures in working memory through repetition. They experience their limitation less acutely than they would if they had no coping mechanisms, making the pain less visible to product developers and investors.

---

## 8. The Case for a 3D Diagram Tool Now

The confluence of several developments suggests that conditions are now more favourable for a 3D system diagram tool than at any previous point.

**Improved hardware.** VR headsets with hand tracking offer the closest digital equivalent to Hopper's Tinker Toy model: a 3D space that can be physically navigated and manipulated. Several research prototypes have demonstrated 3D network visualisation in VR with promising results. Even without VR, large touchscreens and multi-touch interfaces offer interaction patterns closer to physical manipulation than the mouse-based interfaces of earlier 3D graph research.

**Generational 3D fluency.** The population entering software engineering careers has grown up with 3D navigation as a baseline skill. The HCI research that found 3D graphs harder to use than 2D graphs was measuring a generation for whom 3D navigation was novel. That finding should not be assumed to generalise forward.

**The size and complexity of modern systems.** Software architectures, cloud infrastructure, microservice meshes, and distributed systems have grown in complexity to a point where 2D diagrams routinely fail, becoming illegible hairballs that convey topology without communicating it. The problem Hopper identified in 1982, when she was connecting early networked computers, is now endemic. The pressure for a better solution is greater than it has ever been.

**Cognitive science validation.** The research base supporting spatial visualisation as a genuine and common cognitive style, particularly among engineers, has grown substantially since Hopper's lecture. A tool designed explicitly for spatial visualisers can now be grounded in a robust literature, making the user population easier to identify, study, and design for.

**The externalisation framing.** Reframing the tool's purpose from "communicating a system diagram" to "externalising and extending a spatial mental model" opens a different and underserved design space. Such a tool would prioritise rapid spatial capture, navigability, and the ability to grow a structure incrementally, rather than the production of a clean, shareable artefact. These are tractable design challenges.

---

## 9. Conclusion

The experience of representing complex systems as three-dimensional networks of connected nodes is cognitively real, neurologically grounded, and common among the population of software engineers and systems thinkers. It was described with practical concreteness by Grace Hopper in 1982, who built physical prototypes to address the need. It is supported by Kozhevnikov's research on spatial visualisers, Johnson-Laird's mental model theory, and neuroscientific findings on the spatial basis of abstract reasoning.

No adequate digital tool for externalising these representations currently exists. The barriers that have historically prevented such a tool from succeeding, including screen-based interaction costs, non-3D-fluent research populations, and the invisibility of the externalisation use case, are eroding. The population of spatially-fluent users is growing, the complexity of systems demanding representation is increasing, and the hardware for genuine 3D interaction is available.

Hopper's challenge, "you're going to have to get out of the plain of the paper," remains unmet forty-three years later. The cognitive science says the need is real. The engineering says the tools are available. What remains is the will to build for the minority who think in three dimensions, recognising that this minority includes a disproportionate share of the people who design and reason about the systems on which modern life depends.

---

## References

- Forrester, J.W. (1971). *World Dynamics*. Wright-Allen Press.
- Hopper, G. (1982). *Future Possibilities: Data, Hardware, Software, and People*. Lecture delivered to NSA workforce, August 19, 1982. Released by NSA, August 2024.
- Johnson-Laird, P.N. (1983). *Mental Models: Towards a Cognitive Science of Language, Inference, and Consciousness*. Harvard University Press.
- Kozhevnikov, M., Hegarty, M., & Mayer, R.E. (2002). Revising the visualizer/verbalizer dimension: Evidence for two types of visualizers. *Cognition & Instruction, 20*, 47–77.
- Kozhevnikov, M., Kosslyn, S., & Shephard, J. (2005). Spatial versus object visualizers: A new characterization of visual cognitive style. *Memory & Cognition, 33*(4), 710–726.
- Peirce, C.S. (1931–1958). *Collected Papers*. Harvard University Press.
- Tversky, B. (2008). Cognitive tools shape thought: Diagrams in design. *Cognitive Semiotics*.
- Zeman, A., Dewar, M., & Della Sala, S. (2015). Lives without imagery: congenital aphantasia. *Cortex, 73*, 378–380.
- Blazhenkova, O., & Kozhevnikov, M. (2009). The new object-spatial-verbal cognitive style model: Theory and measurement. *Applied Cognitive Psychology, 23*(5), 638–663.
