# Technical Writing One

Table of content

1. [Just enough grammar](#just-enough-grammar)
2. [Words](#words)
3. [Active voice vs Passive voice](#active-voice-vs-passive-voice)
4. [Clear sentences](#clear-sentences)
5. [Short sentences](#short-sentences)
6. [Lists and tables](#lists-and-tables)
7. [Paragraphs](#paragraphs)
8. [Audience](#audience)
9. [Documents](#documents)
10. [Punctuation](#punctuation)

## Just enough grammar

Part of Speech
- Noun -> a person, place, concept, or thing
- Pronoun -> a noun that replaces another noun
- Adjective -> a word or phrase that modifies a noun
- Verb -> an action word or phrase
- Adverb -> a word or phrase that modifies a verb, an adjective, or another adverb
- Preposition -> a word or phrase specifying the positional relationship of two nouns
- Conjunction -> a word that connects two nouns or phrases
- Transition -> a word or phrase that connects two sentences

## Words

We researched documentation extensively, and it turns out that the best sentences in the world consist primarily of words.

### Define new or unfamiliar terms

* If the term already exists, link to a good existing explanation. (Don't reinvent the wheel.)
* If your document is introducing the term, define the term. If your document is introducing many terms, collect the definitions into a glossary.

### Use terms consistently

When I encounter two words that seem to be synonyms, I wonder if the author is trying to signal a subtle distinction that I need to track down and understand.

_For example_, the following paragraph mistakenly renames Protocol Buffers to protobufs:

Protocol Buffers provide their own definition language. Blah, blah, blah. And that's why protobufs have won so many county fairs.

For correct example: Protocol Buffers (or protobufs for short) provide their own definition language. Blah, blah, blah. And that's why protobufs have won so many county fairs.

### Use acronyms properly


On the initial use of an unfamiliar acronym within a document or a section, spell out the full term, and then put the acronym in parentheses

For example:

- If no cache entry exists, the Mixer calls the OttoGroup Server (OGS) to fetch Ottos for the request. The OGS is a repository that holds all servable Ottos. The OGS is organized in a logical tree structure, with a root node and two levels of leaf nodes. The OGS root forwards the request to the leaves and collects the responses.

_Note_: Do not cycle back-and-forth between the acronym and the expanded version in the same document.

### Use the acronym or the full term?

* Don't define acronyms that would only be used a few times.
* Do define acronyms that meet both of the following criteria:
    * The acronym is significantly shorter than the full term.
    * The acronym appears many times in the document.

### Recognize ambiguous pronouns

* Only use a pronoun after you've introduced the noun; never use the pronoun before you've introduced the noun.
* Place the pronoun as close as possible to the referring noun. In general, if more than five words separate your noun from your pronoun, consider repeating the noun instead of using the pronoun.
* If you introduce a second noun between your noun and your pronoun, reuse your noun instead of using a pronoun.

Avoid using this or that in ways where it's not clear what they refer to.

## Active voice vs Passive voice

Distinguish active voice from passive voice in simple sentences
```
Active Voice Sentence = actor + verb + target
```
```
Passive Voice Sentence = target + verb + actor
```
Passive, Passive

![Screenshot 2022-12-25 at 10 05 19](https://user-images.githubusercontent.com/25881847/209455789-ea9a0c50-64b7-483d-869d-d750fc5880a2.png)

=> Partly converted to Active, Passive voice

![Screenshot 2022-12-25 at 10 05 35](https://user-images.githubusercontent.com/25881847/209455791-e3ded6f2-6ebe-489c-9545-fcb0c14183c6.png)

=> Fully converted to Active, Active voice

![Screenshot 2022-12-25 at 10 06 01](https://user-images.githubusercontent.com/25881847/209455792-ed2011f0-7ce3-4e98-8bbf-cb4f1f539ef3.png)

_Prefer active voice to passive voice_

Use the active voice most of the time. Use the passive voice sparingly. Active voice provides the following advantages:
* Most readers mentally convert passive voice to active voice. By sticking to active voice, you enable readers to skip the preprocessor stage and go straight to compilation.
* Passive voice obfuscates your ideas, turning sentences on their head. Passive voice reports action indirectly.
* Some passive voice sentences omit an actor altogether, which forces the reader to guess the actor's identity.
* Active voice is generally shorter than passive voice.
Be bold—be active.

## Clear sentences

Nice quote :D

“Comedy writers seek the funniest results, horror writers strive for the scariest, and technical writers aim for the clearest”

Choose strong verbs

Reduce imprecise, weak, or generic verbs, such as the following:
* forms of be: is, are, am, was, were, etc.
* occur
* happen

![Screenshot 2022-12-21 at 14 15 50](https://user-images.githubusercontent.com/25881847/209455801-df5d3344-3189-4245-a5ce-40bc3c4e9a5f.png)


Good examples

![Screenshot 2022-12-21 at 14 25 00](https://user-images.githubusercontent.com/25881847/209455803-9ff45cfa-42ae-40a9-9acf-5d4710f613ac.png)


They are Clarified to 

![Screenshot 2022-12-21 at 14 25 06](https://user-images.githubusercontent.com/25881847/209455804-0c040aa2-5de5-4e0b-9da6-a71f4838accc.png)


Reduce there is / there are

Sentences that start with There is or There are marry a generic noun to a generic verb.

In the best-case scenario, you may simply delete There is or There are:

![Screenshot 2022-12-21 at 14 34 13](https://user-images.githubusercontent.com/25881847/209455808-fa4136e6-bb3c-4364-bfad-fd802e2585fc.png)


After being removed:

![Screenshot 2022-12-21 at 14 34 16](https://user-images.githubusercontent.com/25881847/209455811-0a9f12a7-e01d-41e7-aa61-388df45c29b8.png)


Repair a There is or There are sentence by moving the true subject and true verb from the end of the sentence to the beginning

![Screenshot 2022-12-21 at 14 35 35](https://user-images.githubusercontent.com/25881847/209455814-1b571197-c460-48a9-bb65-d7b268574d08.png)


Writers start sentences with There is or There are to avoid the hassle of creating true subjects or verbs. If no subject exists, consider creating one

![Screenshot 2022-12-21 at 14 36 21](https://user-images.githubusercontent.com/25881847/209455816-f3d60340-ddbe-48f7-aac1-6e3a689a6dff.png)


**Some good examples**

From

![Screenshot 2022-12-21 at 14 38 21](https://user-images.githubusercontent.com/25881847/209455819-0da70186-6907-4f4c-88f4-5f168cdd431b.png)

To

![Screenshot 2022-12-21 at 14 38 25](https://user-images.githubusercontent.com/25881847/209455823-e6396424-1ee0-4d8f-b191-1578e79478a5.png)


### Minimize certain adjectives and adverbs

Adjectives and adverbs can make technical documentation sound dangerously

![Screenshot 2022-12-21 at 14 54 57](https://user-images.githubusercontent.com/25881847/209455939-c32a442b-9091-4f59-8fe9-42f1e0e65cc0.png)

## Short sentences

* Shorter documentation reads faster than longer documentation.
* Shorter documentation is typically easier to maintain than longer documentation.
* Extra lines of documentation introduce additional points of failure.

### Focus each sentence on a single idea

Focus each sentence on a single idea, thought, or concept. Just as statements in a program execute a single task, sentences should execute a single idea.

![Screenshot 2022-12-21 at 15 14 34](https://user-images.githubusercontent.com/25881847/209455944-4ea1b134-e22f-4c20-8c7d-faaa83771f64.png)

### Convert some long sentences to lists

Inside many long technical sentences is a list yearning to break free.

Example

![Screenshot 2022-12-21 at 15 22 31](https://user-images.githubusercontent.com/25881847/209456362-dbc5a8a9-67b8-4ad0-8456-b2a23a422cc2.png)


into this

![Screenshot 2022-12-21 at 15 22 54](https://user-images.githubusercontent.com/25881847/209456363-0ad9b22a-debb-478f-a3d0-6efe4212a4c9.png)

_Note:_ when we encounter OR in a long sentence, consider refactoring that sentence into a bulleted list.

### Eliminate or reduce extraneous words

Many sentences contain filler—textual junk food that consumes space without nourishing the reader.

_For example:_
An input value greater than 100 causes the triggering of logging.

We can replace causes the triggering of with the much shorter verb triggers

=> An input value greater than 100 triggers logging.

The following table suggests replacements for a few common bloated phrases:

![Screenshot 2022-12-21 at 15 34 03](https://user-images.githubusercontent.com/25881847/209456364-d17915f5-c592-435c-b55a-95c3ff61b280.png)

### Reduce subordinate clauses (optional)

A clause is an independent logical fragment of a sentence

Every sentence contains the following:
* a main clause
* zero or more subordinate clauses
Subordinate clauses modify the idea in the main clause. As the name implies, subordinate clauses are less important than the main clause.

_For example:_

![Screenshot 2022-12-21 at 16 41 15](https://user-images.githubusercontent.com/25881847/209456366-bb1e22b4-6250-4f6c-853b-11582a60cdfa.png)

Common words that introduce subordinate clauses

* which
* that
* because
* whose
* until
* unless
* since

one sentence = one idea

### Distinguish that from which

That and which both introduce subordinate clauses. And here is some diference

In US, reserve which for nonessential subordinate clauses, and use that for an essential subordinate clause that the sentence can't live without.

Python is an interpreted language, which Guido van Rossum invented.

_For example_
The key message in the following sentence is that Python is an interpreted language; the sentence can survive without Guido van Rossum invented:

> Python is an interpreted language, which Guido van Rossum invented.

By contrast, the following sentence requires don't involve linear algebra:

>Fortran is perfect for mathematical calculations that don't involve linear algebra.

=> Note: If you read a sentence aloud and hear a pause just before the subordinate clause, then use which. If you don't hear a pause, use that.


## Lists and tables

“Good lists can transform technical chaos into something orderly”

Choose the correct type of list

The following types of lists dominate technical writing:
* bulleted lists
* numbered lists
* embedded lists

Note:
* If you rearrange the items in a bulleted list, the list's meaning does not change.
* If you rearrange the items in a numbered list, the list's meaning changes.

For example, we've made the following a bulleted list because rearranging its items does not change the list's meaning:
Bash provides the following string manipulation mechanisms:
* deleting a substring from the start of a string
* reading an entire file into one string variable


The following list, by contrast, must be a numbered list because rearranging its items would change the list's meaning:
Take the following steps to reconfigure the server:
1. Stop the server.
2. Edit the configuration file.
3. Restart the server.

Generally speaking, embedded lists are a poor way to present technical information. Try to transform embedded lists into either bulleted lists or numbered lists

Good example:

![Screenshot 2022-12-24 at 14 41 50](https://user-images.githubusercontent.com/25881847/209456370-8dd07dbb-2fbe-44ed-b908-ae60f2e3ce5c.png)

converted to

Here's one possible answer:

![Screenshot 2022-12-24 at 14 41 45](https://user-images.githubusercontent.com/25881847/209456371-4c7009d9-a546-480f-9cdd-2d882da89c3a.png)


The following is an alternative answer:

![Screenshot 2022-12-24 at 14 41 56](https://user-images.githubusercontent.com/25881847/209456373-9365ac79-b96d-43d9-a884-ca3dfae47736.png)

### Keep list items parallel

Effective lists are parallel; defective lists tend to be nonparallel. All items in a parallel list look like they "belong" together

That is, all items in a parallel list match along the following parameters:
* grammar
* logical category
* capitalization
* punctuation

Conversely, at least one item in a nonparallel list fails at least one of the preceding consistency checks.

good example for checking whether the following list parallel or nonparallel?

* The red dots represent sick trees.
* Immature trees are represented by the blue dots.
* The green dots represent healthy trees.

=> This is a nonparallel list. The first and third items are in active voice, but the second item is in passive voice.

### Start numbered list items with imperative verbs

An imperative verb is a command, such as open or start
For example
1. Download the Frambus app from Google Play or iTunes.
2. Configure the Frambus app's settings.
3. Start the Frambus app.

### Punctuate items appropriately

If the list item is a sentence, use sentence capitalization and punctuation. Otherwise, do not use sentence capitalization and punctuation.

## Paragraphs

an inspirational message to start a great chapter :D.

![Screenshot 2022-12-24 at 17 52 34](https://user-images.githubusercontent.com/25881847/209456375-6fa44d87-02c6-4b1b-bd0a-ced3a00b7ced.png)

### Write a great opening sentence

The opening sentence is the most important sentence of any paragraph. Busy readers focus on opening sentences and sometimes skip over subsequent sentences. Therefore, focus your writing energy on opening sentences.

Good opening sentences establish the paragraph's central point. _For example_, the following paragraph features an effective opening sentence:

![Screenshot 2022-12-24 at 18 55 48](https://user-images.githubusercontent.com/25881847/209456377-d313d73e-fd47-484d-a845-6bb5afe2f5c1.png)

By contrast, the following opening sentence sends readers in the wrong direction

![Screenshot 2022-12-24 at 18 56 16](https://user-images.githubusercontent.com/25881847/209456379-1d64d31b-2044-4dc8-ae46-4fb9f332cbbe.png)

One example on what effective paragraph is

not this one

![Screenshot 2022-12-24 at 18 57 48](https://user-images.githubusercontent.com/25881847/209456382-d9e35bfa-8ed9-47ba-9b54-ed40da33e0c7.png)

This paragraph is defective because it implies that the paragraph will focus on the Pythagorean Theorem. In fact, its focus is actually clustering algorithms


this one is actually an effective alternative.

![Screenshot 2022-12-24 at 18 57 39](https://user-images.githubusercontent.com/25881847/209456384-b16f6a66-6cc2-446f-afab-9e7c3fc6b677.png)


Note: Effective opening sentences can take many forms. That is, not all great paragraphs start with a sentence that states the theme. Starting a paragraph with a rhetorical question, for example, can engage readers.


### Focus each paragraph on a single topic

A paragraph should represent an independent unit of logic. Don't describe what will happen in a future topic or what happened in a past topic.

![Screenshot 2022-12-24 at 23 13 52](https://user-images.githubusercontent.com/25881847/209456388-65d7e905-29aa-41da-8bda-fcac136e2149.png)

![Screenshot 2022-12-24 at 23 16 34](https://user-images.githubusercontent.com/25881847/209456390-c124f5fe-3322-4fcd-bf50-fed1ef7e463a.png)

```
Don't make paragraphs too long or too short
```
### Answer what, why, and how

Good paragraphs answer the following three questions:
1. What are you trying to tell your reader?
2. Why is it important for the reader to know this?
3. How should the reader use this knowledge? Alternatively, how should the reader know your point to be true?
For example, the following paragraph answers what, why, and how:

![Screenshot 2022-12-24 at 23 27 59](https://user-images.githubusercontent.com/25881847/209456391-97f6b267-18a5-4418-bf07-49e4e2e7fc8c.png)

## Audience

![Screenshot 2022-12-24 at 23 29 58](https://user-images.githubusercontent.com/25881847/209456395-a4ab1c17-fd7f-4ff5-be50-0ac48f4289aa.png)

In other words, make sure your document provides the information that your audience needs but doesn't already have. Therefore, this unit explains how to do the following:
* Define your audience.
* Determine what your audience needs to learn.
* Fit documentation to your audience.

### Define your audience

Begin by identifying your audience's role(s). Sample roles include:
* software engineers
* technical, non-engineer roles (such as technical program managers)
* scientists
* professionals in scientific fields (for example, physicians)
* undergraduate engineering students
* graduate engineering students
* non-technical positions


People within the same role generally share certain base skills and knowledge

### Determine what your audience needs to learn

In some cases, the list should hold tasks that the target audience needs to perform.

After reading the documentation, the audience will know how to do the following tasks:
* Use the Zylmon API to list hotels by price.
* Use the Zylmon API to list hotels by location.
* Use the Zylmon API to list hotels by user ratings.


If you are writing a design spec, then your list should focus on information your target audience should learn rather than on mastering specific tasks: For example:
After reading the design spec, the audience will learn the following:
* Three reasons why Zylmon outperforms Zyljeune.
* Five reasons why Zylmon consumed 5.25 engineering years to develop.


### Fit documentation to your audience

#### Vocabulary and concepts

Experienced people on your software team probably understand the implementation details and data structures of your team's project, but nearly everyone else (including new members of your team) does not. Unless you are writing specifically for other experienced members of your team, you typically must explain more than you expect.

#### Curse of knowledge

Experts often suffer from the curse of knowledge, which means that their expert understanding of a topic ruins their explanations to newcomers. As experts, it is easy to forget that novices don’t know what you already know.

#### Simple words

A significant percentage of technical readers are more comfortable in languages other than English. Therefore, prefer simple words over complex words

#### Cultural neutrality and idioms

Keep your writing culturally neutral. Do not require readers to understand the intricacies of NASCAR, cricket, or sumo in order to understand how a piece of software works.


## Documents

### State your document's scope

A good document begins by defining its scope. For example:

![Screenshot 2022-12-25 at 00 43 18](https://user-images.githubusercontent.com/25881847/209456399-61ff62db-e1d2-4bd3-8b47-abfc7a8a6c71.png)


A better document additionally defines its non-scope—the topics not covered that the target audience might reasonably expect your document to cover. For example:

![Screenshot 2022-12-25 at 00 47 08](https://user-images.githubusercontent.com/25881847/209456400-5be29b8b-dea0-4107-a92f-4b48d5a89dae.png)


Scope and non-scope statements benefit not only the reader but also the writer (you). While writing, if the contents of your document veer away from the scope statement (or venture into the non-scope statement), then you must either refocus your document or modify your scope statement. When reviewing your first draft, delete any sections that don't help satisfy the scope statement.


### State your audience

A good document explicitly specifies its audience.

![Screenshot 2022-12-25 at 00 51 25](https://user-images.githubusercontent.com/25881847/209456402-69defd18-86ba-4c26-90b8-9ddb94bf1647.png)


a good audience declaration might also specify any prerequisite knowledge or experience.

![Screenshot 2022-12-25 at 00 51 38](https://user-images.githubusercontent.com/25881847/209456405-e7b51335-33e1-41e9-964b-46dfa6288439.png)

In some cases, the audience declaration should also specify prerequisite reading or coursework

![Screenshot 2022-12-25 at 00 52 27](https://user-images.githubusercontent.com/25881847/209456408-0f11644d-3475-4094-9a53-73d9fb3114e8.png)

### Summarize key points at the start

Engineers and scientists are busy people who won't necessarily read all 76 pages of your design document. Imagine that your peers might only read the first paragraph of your document. Therefore, ensure that the start of your document answers your readers' essential questions.

Professional writers focus considerable energy on page one to increase the odds of readers making it to page two. However, the start of any long document is the hardest page to write. Be prepared to revise page one many times.

### Compare and contrast

Most of your work will be evolutionary, building on existing technologies and concepts. Therefore, compare and contrast your ideas with concepts that your audience already understands.

![Screenshot 2022-12-25 at 01 03 59](https://user-images.githubusercontent.com/25881847/209456414-d3456a58-daf9-4bde-bcaf-e20ce1aac84f.png)

Or

![Screenshot 2022-12-25 at 01 04 26](https://user-images.githubusercontent.com/25881847/209456416-dacaf6ae-db12-4ea8-8c25-8c523044383d.png)


“Frambus Weather app v2 introduces ten features not available in Frambus Weather app v1. Most importantly, v2 offers two-week forecasts, v1 offered only one-week forecasts. Tidal information won't change.”
=> The final sentence (about tides) isn't important enough to appear in the opening paragraph. The first sentence mentioned ten new features, so readers would likely expect to hear more about those new features. Instead, the final sentence refers to something other than a new feature.

### Write for your audience

This chapter’s worth any words.

#### Define your audience's needs

Answering the following questions helps you determine what your document should contain:

![Screenshot 2022-12-25 at 07 39 06](https://user-images.githubusercontent.com/25881847/209456417-3058b4d4-fa98-4dec-ba7f-7b9873c52c00.png)

For example, suppose you have invented a new sorting algorithm, which is similar to quicksort. The following list contains some potential answers to the preceding questions:

![Screenshot 2022-12-25 at 07 39 14](https://user-images.githubusercontent.com/25881847/209456420-b359061d-2b6f-4f87-98ea-55e9590282be.png)


#### Organize the document to meet your audience's needs

![Screenshot 2022-12-25 at 07 41 01](https://user-images.githubusercontent.com/25881847/209456423-e05d8416-ad86-4bc6-aee1-1a65695bfa01.png)


## Punctuation

Grammarly cares all :D but there are a few good best practices here.

**Commas**

![Screenshot 2022-12-25 at 07 42 00](https://user-images.githubusercontent.com/25881847/209456427-aea89d8b-ccdd-4998-9856-7f6359b7ea1f.png)

![Screenshot 2022-12-25 at 07 42 04](https://user-images.githubusercontent.com/25881847/209456429-7b82f397-f972-4b15-9a02-0cc620b5f8af.png)


**Semicolons**

![Screenshot 2022-12-25 at 07 42 35](https://user-images.githubusercontent.com/25881847/209456433-b8b1d5dd-803b-485f-b301-735fb6470b61.png)


Before using a semicolon, ask yourself whether the sentence would still make sense if you flipped the thoughts to opposite sides of the semicolon.


The thoughts preceding and following the semicolon must each be grammatically complete sentences.

For example, the following semicolon is incorrect because the passage following the semicolon is a clause, not a complete sentence:

![Screenshot 2022-12-25 at 07 42 48](https://user-images.githubusercontent.com/25881847/209456437-0254d8e4-6a8e-46e9-9b5f-6ae72a31349d.png)

You should almost always use commas, not semicolons, to separate items in an embedded list

![Screenshot 2022-12-25 at 07 42 54](https://user-images.githubusercontent.com/25881847/209456441-f23c70db-0548-4c01-9607-373ed4998eda.png)

![Screenshot 2022-12-25 at 07 42 57](https://user-images.githubusercontent.com/25881847/209456446-7f0fc811-5515-418a-998e-96b8f128f7ce.png)

![Screenshot 2022-12-25 at 07 43 02](https://user-images.githubusercontent.com/25881847/209456448-f6187daa-b35b-42cb-94de-b67a3969b754.png)

**Em dashes**

Em dashes are compelling punctuation marks, rich with punctuation possibilities

![Screenshot 2022-12-25 at 07 44 52](https://user-images.githubusercontent.com/25881847/209456458-7ced226d-1096-410e-960e-432b5036c9d3.png)

**Parentheses**

The rules regarding periods and parentheses aren't always clear. Here are the standard rules:
* If a pair of parentheses holds an entire sentence, the period goes inside the closing parenthesis.
* If a pair of parentheses ends a sentence but does not hold the entire sentence, the period goes just outside the closing parenthesis.

