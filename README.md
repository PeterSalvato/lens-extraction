# Lens Extraction
### Decomposed Evaluation Through Practitioner-Derived Criteria

"Is this good?" I asked an AI that question in 2023. A compound prompt: evaluate a portfolio site across voice quality, structural integrity, narrative coherence, and brand alignment. The model processed the first criterion with full attention. Each subsequent criterion got less. The output blurred all four into a blended average that was none of them.

I recognized it immediately. A compound instruction given to a system that cannot process it whole. I had seen this every day in the classroom. In the critique room at SVA, five people evaluated the same piece and disagreed. That was the point. This paper documents how I extract a real practitioner's evaluative framework, codify it as testable criteria, and run multiple lenses independently against the same work. Where they disagree is where the real decisions live.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.18986295.svg)](https://doi.org/10.5281/zenodo.18986295)

**Source:** [github.com/PeterSalvato/lens-extraction](https://github.com/PeterSalvato/lens-extraction)

**Peter Salvato**
Design Engineer | [petersalvato.com](https://petersalvato.com/)
March 2026

---

## Abstract

Lens extraction begins as a compositional act, not an evaluative one. Once the practitioner's raw thinking is out — unfiltered, uncompressed, unstructured — the first decision is the lens array: a closed set of evaluative frameworks extracted from real practitioners whose judgment they have chosen to honor. The unstructured source material reveals the shape of what is actually there. The array is the first act of authorship on that material. It declares what the work is committed to being before any generative work proceeds. Evaluation, when it comes, is the mechanism for staying true to that declaration.

This paper proposes lens extraction as a protocol for studying a practitioner's body of work, identifying the evaluative framework underneath their visible decisions, and codifying it as testable criteria that an AI can execute independently. Multiple extracted lenses run in parallel across independent evaluation dimensions. Where they agree is signal. Where they disagree is a decision point for the maker, and where persistent disagreement appears across multiple passes, a potential values conflict in the declaration itself.

The paper distinguishes compositional lens arrays from conventional persona work. Traditional personas ask whether different user types can access a product. Compositional lens arrays declare what the work must embody. The lens is not a user to be served. It is a commitment to be honored.

The protocol is demonstrated through three years of applied practice using lenses extracted from real practitioners (Vignelli, Bierut, Millman, Victore, Rams, Shaw, Muller-Brockmann, Draplin) deployed on a production site, and through the development of a practitioner-specific methodology curriculum where the persona stack specified what the curriculum had to be before any content was written. The paper situates lens extraction within the accommodation design framework (Salvato, 2026): compound evaluation degrades in AI systems the same way compound instructions degrade in special education classrooms. Decompose the evaluative function. Staff each dimension independently. Let the maker resolve the conflicts.

---

## 1. Twelve Questions Disguised as One

Criteria contaminated each other. Contradictions showed up within a single evaluation pass. The solution was obvious once I saw it that way. Break the compound prompt apart. One dimension per pass. One objective, one output. Run each evaluation on its own.

That solves the compound-evaluation problem. It does not solve the criteria problem: who decides what "good" means for each dimension?


## 2. The Criteria Problem

Generic evaluation criteria produce generic evaluation. "Is the typography clean?" is answerable but uninformative. "Does the type system demonstrate the economy of means and systematic limitation that Vignelli consistently demanded across forty years of practice?" produces a different evaluation entirely.

The difference goes beyond precision. It is a difference in perspective. A generic criterion evaluates against a statistical average of what "good" means. An extracted criterion evaluates against a specific practitioner's consistent, documented standards. The first tells you whether the work is competent. The second tells you whether the work would satisfy someone whose judgment you trust.

The model for this existed before AI. The critique room at the School of Visual Arts. Multiple faculty evaluating the same work independently, from different perspectives, in good faith, at the same time. Where they agreed, strong signal. Where they disagreed, a decision for the maker. The evaluative function was decomposed across independent perspectives, and the disagreements were the most valuable output.

The question is how to reconstruct that evaluative function in AI-mediated work.


## 3. What the Field Is Doing

### 3.1 LLM-as-Judge

The dominant approach to AI evaluation is LLM-as-judge: a single model scores output against a rubric. The rubric may be generic ("rate creativity, coherence, and relevance on a scale of 1-5") or domain-specific. The model applies all criteria in a single pass.

The architecture has the same flaw as my initial compound prompt. The model blends criteria. A piece of work that is structurally excellent but narratively weak receives a middling score that obscures both the strength and the weakness. The evaluative function is flattened.

Recent work on multi-model debate (multiple models arguing about quality) addresses the perspective problem by introducing disagreement. But the models are not staffed with specific evaluative frameworks. They are generic models generating generic arguments. The disagreement is artificial.

### 3.2 Style Transfer and Aesthetic Scoring

Machine learning approaches to aesthetic evaluation train models on datasets of human preference judgments. The model learns to predict what humans rate highly. The output is a score or a ranking.

These systems capture statistical preferences. They do not capture evaluative logic. Knowing that a design will score 7.2/10 on a preference model tells you nothing about whether the typography serves the content, whether the grid is honest, or whether the identity is present. The score compresses every evaluative dimension into a single number.

### 3.3 Design Linting and Automated Review

Rule-based systems check mechanical properties: spacing consistency, color contrast, accessibility compliance. These are valuable and necessary. They are not evaluation. Passing every accessibility check does not mean the design communicates. Correct grid spacing does not mean the hierarchy works.

### 3.4 Rubric-Based AI Assessment

Predefined rubrics applied by AI models. The rubrics are generic by necessity, designed to apply across many projects. "Does the design have a clear visual hierarchy?" "Is the color palette consistent?" The criteria are testable but shallow. They evaluate the surface without evaluating the thinking.


## 4. The Gap

Nobody is extracting a named practitioner's evaluative framework from their body of work, codifying it as testable criteria, and running multiple extracted lenses independently against the same work to read convergence and divergence.

The evaluative function in the current literature is either:
- **Single-perspective** (one model, one rubric, blended output)
- **Generic-perspective** (multiple models, no specific evaluative frameworks)
- **Mechanical** (rule-based, surface properties only)
- **Statistical** (preference prediction, compressed to a single score)

Missing: multi-perspective evaluation using criteria extracted from the documented practice of specific, named practitioners, run independently, with convergence and divergence both treated as signal.


## 5. Lens Extraction

### 5.1 The Protocol

A lens is a codified evaluative framework extracted from a real practitioner's body of work. The extraction protocol:

1. **Study the practitioner's output.** Read their books, examine their work, listen to their talks. Massimo Vignelli has forty years of documented practice and published design philosophy. Debbie Millman has twenty years of interviews where her evaluative questions are explicit.

2. **Extract the framework.** What does this practitioner consistently ask? What do they never tolerate? Vignelli consistently demands economy of means: systematic limitation, type discipline, nothing that does not earn its place. Victore consistently demands personality: is the maker fiercely present? Does the work have the courage of its own identity?

3. **Codify as testable criteria.** Turn the extracted questions into specific, evaluable checks. "Does each typeface earn its presence, or could one be removed?" (Vignelli). "Would a stranger know who made this just by being in the room?" (Shaw). "Is there a real person in this text, or could it be anyone's?" (Millman).

4. **Validate against their known work.** The lens should confirm what the practitioner would confirm. Run a Vignelli lens against Vignelli's own work. If it scores poorly, the extraction is wrong.

This is what a good creative director does when building a team: systematize how strong practitioners think so the thinking scales beyond one person's presence. Lens extraction formalizes the process.


### 5.2 Multiple Lenses, Independent Dimensions

Each layer of concern gets its own lenses. On the production site (petersalvato.com), the layers are:

**Structural lenses** evaluate whether the design is well-built:
- Vignelli: restraint, economy, systematic limitation
- Rams: as little design as possible, everything earning its place
- Muller-Brockmann: the grid as order, structure creating clarity from complexity

**Narrative lenses** evaluate whether the site communicates identity:
- Victore: is the maker fiercely present? Does the work have personality?
- Millman: is there a real person here? Is the stake specific enough to be believed?
- Shaw: does this feel like a world? Would a stranger know who this person is?
- Draplin: is there a human with opinions here? Does the brand feel like the person?

Each lens runs independently. Each produces its own verdict. The coordinator collects the verdicts and maps convergence.


### 5.3 Why Tension Is the Point

A single lens produces imitation. If you extract Vignelli and apply only Vignelli, you get work that looks like Vignelli's. Multiple lenses produce tension. Vignelli demands restraint. Victore demands personality. Vignelli says remove everything unnecessary. Victore says put yourself into everything. Those two instructions, applied to the same page, force a decision you would not have reached working from either influence alone.

That tension is where the real decisions happen. Over time, the way you resolve those conflicts page after page is what makes the work yours. The system identifies where the disagreements are. The maker resolves them. That's the accommodation: the system does the parallel evaluation the maker can't hold simultaneously, and the maker provides the judgment the system can't perform.

The IEP parallel is direct. Individualized criteria, independent assessment, the practitioner resolving conflicts between goals that measure different things. A student's IEP has multiple goals that sometimes conflict (build independence vs. provide support). The teacher navigates the tension. The framework holds both goals without pretending they are the same dimension.


### 5.4 The Lens Array as Values Declaration

The paper to this point has described lens extraction as an evaluative tool. That framing is accurate but incomplete. It describes the mechanism without describing the more fundamental use.

When I build a lens array for a project, I build it immediately after the unstructured source material is out. I can see the shape of what I'm actually working with. The lens array is the first decision I make in response to that shape: which voices do I want in the room, which values will govern every decision I make, which practitioners' judgment I have chosen to honor. The array is not derived from evaluation needs. It is the first act of authorship on the raw material that input inversion produced.

The evaluation use, when it comes, is the mechanism for staying true to that declaration. Running the array against work-in-progress tests whether the work is holding to the values I committed to at the outset. The sequence matters: declaration first, evaluation in service of the declaration.

This distinction resolves something the field has not clearly articulated.

**Designed for vs. designed to be**

Traditional persona work operates in an evaluative register. You build personas representing different user types, then ask whether each persona can access the product. The question is pass/fail: does this reach the user I defined? The persona is an instrument for measuring reach.

The lens array works differently. The lenses I select do not represent an audience I am trying to reach. They represent the values the work is designed to embody. When I include a Victore lens, I am not asking whether fiercely-opinionated practitioners will be served. I am declaring that fierce presence is a value the work must hold. The Victore lens is not a user. It is a commitment.

The difference in practice: a product designed for a persona can succeed if that persona can use it. A product designed to embody a set of values succeeds only if the values are actually present in the work. The first is about access. The second is about integrity.

I have not found this distinction made explicitly in the UX or product literature. The persona framework was built for the evaluative register. The compositional use, building an array as a declaration of what the work must be before a user ever encounters it, is something practitioners do without a name for it.

**The array as a closed peer set**

The lens array is a closed peer set. Every lens I include carries equal weight. There is no primary persona, no secondary persona, no hierarchy of importance. The Victore lens does not outrank the Vignelli lens. The Millman lens does not defer to the Rams lens.

This has a specific consequence. The intersection of what satisfies all lenses simultaneously defines the work. A decision that satisfies Vignelli but violates Victore is not an acceptable decision. The work must find the resolution that holds both. If no resolution exists, the array itself needs examination. Either a lens was chosen carelessly, or the project has an unresolved values conflict that needs to surface before the work proceeds.

Adding or removing a lens is not a minor adjustment. It changes what the work is required to be. Including a Draplin lens commits the work to having a human with strong opinions visibly present. Removing it releases that commitment. The closed peer set is not casual. It is the specification.

**The persona stack version**

The same logic applies to persona stacks. I built the first persona stack for Joinery, the methodology school, using four practitioner types: a brand designer, a novelist, a copywriter, and a creative director. The question I asked was not "can each of these people access the curriculum?" It was "what must the curriculum be if it is to hold all four of these people simultaneously?"

The personas were not derived from user research. They were composed before the curriculum existed. I was declaring the stack of minds the work would be designed to satisfy: not as users to be served, but as peers whose presence in the room would shape every decision about what the work should be.

The distinction from conventional persona work is structural. In conventional use, personas are evaluative instruments. You derive them from data, you use them to test reach, you update them as the audience shifts. In compositional use, personas are a values declaration. You build them as an act of authorship, you use them to specify what the work must be, and you hold them stable precisely because they represent a commitment, not a hypothesis.

The intersection of what satisfies all four personas simultaneously was not obvious. It required finding the framing, the methodology, and the specific language that a novelist, a brand designer, a copywriter, and a creative director could each recognize as directly relevant to their practice. That specification work, finding the thing that holds all four, is what produced the positioning. The persona stack was not a research artifact. It was a compositional constraint that generated the work.

**Implications for the evaluation function**

This reframes what lens-based evaluation is doing.

When I run the lens array against work-in-progress, I am checking whether the work is honoring a commitment I made at the start of the project. The evaluation is not asking "is this good?" in the abstract. It is asking "is this still holding to what I said it would be?"

The divergence case is different in this frame. When two lenses disagree, the question is not just "where does my judgment matter?" It is "is this values conflict resolvable within the project as I've defined it, or does the array need examination?" A persistent divergence between two lenses on every pass is a signal that the values they represent may be incompatible within the current project definition. That is different from a single divergence on a single pass, which is just a decision point.

The maker's job in this frame is not only to resolve individual disagreements between lenses. It is to maintain fidelity to the values declared at the outset, and to recognize when a pattern of divergence indicates a problem with the declaration itself.


## 6. Applied Evidence

### 6.1 The Steward Paradox

During one evaluation pass on petersalvato.com, the structural lenses scored seven out of nine criteria at the top tier. The grid was sound. The typography was clean. The spacing held.

The narrative lens that asks "does this feel like a world? would a stranger know who this person is just by being in the room?" scored WEAK.

Same site. Two layers. Opposite readings.

That looked like a contradiction until I recognized what the two layers were actually measuring. The structural layer was evaluating craft: is the thing well-built? The narrative layer was evaluating identity: does the thing feel like a specific person's space?

Both layers were right. The craft was sound and the identity was buried. I kept the structural foundation and rewrote the copy to bring the identity forward. That was a convergence decision: two layers, opposite readings, one choice that honored both.

A single-score evaluation would have returned something middling. "The site is adequate." The decomposed evaluation told me exactly what was strong, exactly what was weak, and exactly where my judgment was needed. I would not have found that split without running the layers independently.


### 6.2 Generation Constraints

The same lenses that evaluate can constrain generation. When the evaluation identifies that the voice is too generic, the voice lens criteria become generation inputs. The model writes under specific constraints: "lead with a real situation, not a concept" (Millman), "show the work, do not describe the methodology" (craftsman register), "no sentence exists to impress rather than demonstrate" (Victore).

Every generative output stops before writing to disk. The maker sees what was produced, decides, approves. The system handles analysis and generation. The maker handles creative direction. The lenses ensure that the generation is evaluated against specific, extracted standards, not against a generic sense of "good enough."


### 6.3 Scale

The production system currently runs twenty-two single-purpose diagnostic skills and five coordinators. Each diagnostic has one objective, one clear output. The coordinators dispatch them in parallel where they are independent and sequentially where one depends on another. The model never receives twelve evaluation goals at once.

This is task decomposition as accommodation. The model's processing limitation (compound evaluation degrades) is accommodated by the architecture (single-objective skills, coordinator orchestration). The individual assessments stay focused. The coordinator handles synthesis. The practitioner resolves disagreements.


## 7. Connection to Accommodation Design

Lens extraction applies the accommodation design framework (Salvato, 2026) to the evaluation function:

**The disability.** The model cannot evaluate across multiple dimensions simultaneously without blending them. Compound evaluation degrades the same way compound instruction degrades in the classroom. Criteria contaminate each other. The output is a blended average.

**The accommodation.** Decompose the evaluative function. Staff each dimension with criteria extracted from a practitioner whose judgment you trust. Run them independently. Give the model one evaluation task per lens. Collect results and map convergence.

**The human's role.** The maker resolves disagreements between lenses. The system identifies where judgment is needed. The human provides the judgment. The model never decides whether structural integrity outweighs narrative presence. That is a creative decision. The model does not make creative decisions.

The accommodation is bilateral. The AI cannot evaluate across all dimensions simultaneously (so we decompose). The human cannot hold nine independent perspectives simultaneously (so the AI runs them in parallel). Each system compensates for the other's processing limitation.


## 8. Implications

**Evaluation is decomposable.** "Is this good?" is twelve questions. Each question needs its own criteria, its own lens, its own definition of success. Systems that compress evaluation into a single score or a single rubric will always flatten the evaluative function.

**Practitioner extraction scales critique.** A junior designer working alone has access to their own judgment. With lens extraction, they have access to a codified approximation of Vignelli's judgment, Millman's judgment, Victore's judgment, all running in parallel. The critique room scales beyond the physical room.

**Disagreement between lenses points to where the maker's judgment is needed.** Multi-perspective systems should expect and value that disagreement. A system that eliminates it by averaging has thrown away the most useful information in the evaluation.

**The maker stays in the loop.** Lens extraction doesn't replace the maker's judgment. It identifies where the maker's judgment is required and provides the specific criteria each perspective would bring to the decision. The final choice is always the maker's.

**The protocol is replicable.** Any practitioner with a documented body of work can be extracted into a lens. Any domain with multiple evaluative perspectives can benefit from decomposed, lens-based evaluation. The protocol is not limited to visual design. Any field where "is this good?" is multiple questions disguised as one is a candidate.


## 9. Conclusion

The AI evaluation field is organized around single-perspective scoring. One model, one rubric, one score. The evaluative function is flattened into a number that obscures what is strong, what is weak, and where the maker's judgment is needed.

Lens extraction reconstructs the multi-perspective evaluation that working practitioners have always relied on. Multiple perspectives, extracted from real practice, running independently, with convergence and divergence both treated as signal. The tensions between lenses force decisions that no single perspective would produce. Those decisions, accumulated across every page, are what give the work a specific identity instead of a blended average.

The protocol is derived from the accommodation design framework: decompose the compound task, individualize the criteria, let the practitioner resolve the conflicts. The same move that works in a self-contained classroom works in AI-mediated evaluation. The processing limitation is the same.

---

## References

Salvato, P. (2026). AI Governance as Accommodation Design: A Pedagogical Framework for Human-AI System Architecture. petersalvato.com.

Salvato, P. (2026). Input Inversion: Why Unstructured Human Thinking Produces Better AI Output. petersalvato.com.

Salvato, P. (2026). A Different Kind of Harness: AI as Cognitive Prosthetic Through Mutual Accommodation. petersalvato.com.

Salvato, P. (2026). Semantic Flattening and the Case for Human-Marked Importance in AI Memory. petersalvato.com.

---

## License

This work is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

You are free to share and adapt this material for any purpose, including commercially, with attribution.

---

*Peter Salvato is a design engineer based in Fort Lauderdale, FL. He studied Visual Communication at the School of Visual Arts, taught special education in Brooklyn, NY, and spent thirteen years building the front end of an enterprise recruiting platform. His AI governance work applies twenty-five years of practice across construction, print production, pedagogy, enterprise software, and brand systems to the question of what AI systems actually need to produce quality output. His work is published at [petersalvato.com](https://petersalvato.com/).*
