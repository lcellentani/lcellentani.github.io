When I started my journey with AI tool, I felt lost and confuse. Too many new concepts, many different ways to engage with those new tools. All early experiements concluded with disappointed results. I found my self saying "Is that all?", "Am I use those tools in the wrong way?". I went back, worked to expand my knowledge, connected more dots, lined up parts of different workflows, and results improved. I understood my approach with AI needed to be tuned based on the type of work I was trying to accellerate through AI; brainstorming in a Chat window or directing tasks in a CLI environment could not be done with the same natural language tone or intention (I don't know how to express the idea of the intent or way to engage with AI agents to achieve some work).

The turning point was when I found the Anthropic’s AI Fluency course hosted in the Claude Academy website. The 14 lessons went down in a blast. Suddendly I realized that the AI revolution we are experiencing is not just another technological leap that requires to expand our engineers hard skill baggage, it is something deeper than that. It requires to integrate a new series of soft skills that usually engineers may need to learn if they decide to walk the leadership career path...like moving to be Tech Leads or Technical Director. The 4D Framework that explores the fout core competencies individual should be mindful when they engage with AI in a more mindful way helped me to assign names to the different struggles I was experiences in all my experiments with AI and Agentic Workflows.

The course inspired me to create what I named the Delegation Framework, it is not the most original name but naming things is probably the most difficult task.
In a nutshel the Delegation Framework is a metric to classify the collaboration between Humans and AI. It doesn't matter which type of work we are doing, the framework wants to explore questions like "who owns this line?", "who owns this pixel?", "who owns this result?"
The framework is built around four tiers of delegation: T1, the author wrote these lines independently. T2, the author wrote these lines with AI answering questions. T3, AI-drafted, and the author owns every line. T4, the author fully delegated to AI all lines.

After I framed the details of the framework, I built a small set of skills to explain Claude (or AI Agents in general), what the tiers are and how they should be used. Then I decided to run an experiment on myself. From April until today I decided to tag every single commit in any Github contribution with a tier that express how I produced a certain commit. I tried to be honest with myself and leveraging the skills system, I instructed Claude to be as strict as possible judging our collaboration. So it is not extremely scientific because there is some human factor in the way things have been done but it was enough significant for my day-to-day work routine.

The numbers I've been able to collect tell an interesting story. [here we should have a paragraph or two plus picture with diagrams that presents my numbers].

How all this changed my ability to feel effective and efficient when using AI? The framework didn't give me new techniques, or a magic ruleset to compose prompts, or a recipe to orhcestrate and distribute work across AI agents. It structured my engagement with AI from the very first moment when I start a CLI session through every time I write some line of code. I started to ask myself questions like "is it worth for me to write these lines? Do I learn anything from filling this boilerplate code block?" "Am I giving away important context if I don't pay attention to this particual architectural decisions?" "can I reconcile my knowledge gap later if I let Claude do this for me?"
I modelled my personal SPEC-Driven workflow around the Four Tiers; so at the end of each Implementation Plan I could look back and reflect and ask "did I still feel that I own and understand what has been done?"

There are areas of the Delegation Framework that I haven't been able to nail perfectly. The boundary between tiers such as for example T3 and T4 is fuzzy to define, or having a good separation of the work that covers a task may affect the projected picture when classifing Git commits. However as Claude and similar Agents starts to maintain memory of the collaboration with them, I observed that a more structured and intentional engagement helps achieving better (i want to find a more precise adjective) and meaningful results in terms of code produced, archictures designed, even casual conversations.

If you are curious of trying this approach on your projects, feel free to poke inside and get inspired by my delegation-tier skill (link here). Run the experiment on yourself for a few months then analyze your commits.

Also, I strongly recommend to sign up and complete the Anthropic AI Fluency: Framework and foundations cours (link to the Anthropic page). In my opinion is a skill anyone interested to have a meaningful and effective engagement with AI should acquire.


What the repos show: 

The four tiers: T1, written independently. T2, written with AI answering questions. T3, AI-drafted, and the author owns every line. T4, fully delegated.
The rules you built around them: every plan task gets a tier tag with a one-line rationale. When the right tier is unclear, you default to the higher-ownership tier. Mixed tasks are split, so a real design decision never hides inside a mechanical T4 task.
The audit trail: every commit starts with [Tn].
A number nobody else has: in flatline’s history, the tags split roughly 39% T4, 36% T3, 24% T2, and just 1% T1 (one commit, out of 88). That’s a striking fact about how you actually work with AI, and it would make a good small chart.

On the framework. Anthropic’s AI Fluency Framework has four competencies: Delegation, Description, Discernment and Diligence. Delegation covers problem awareness, platform awareness, and dividing work between you and the AI. The source I checked doesn’t mention levels or tiers, and it places ownership under Diligence, not Delegation. So your claim holds as far as I can tell: the tiers are your extension. I only checked a secondary article, not Anthropic’s course materials, so check the official material before the post says “the framework doesn’t define tiers”. The safe wording is “as far as I can tell”, and describing the tiers as something you built with Claude.

Suggested outline (about 550 words):

Hook: delegation isn’t yes or no. The useful question is “who owns this line?”
The four tiers, with one concrete example each.
Three rules: tag every task with a reason, default to more ownership when unsure, and split mixed tasks.
The data: your tier distribution, plus what surprised you.
What doesn’t work yet: the boundary between T3 and T4 is fuzzy, and review effort doesn’t scale evenly.
Closing: how to try it on your own project, and a credit to the AI Fluency framework