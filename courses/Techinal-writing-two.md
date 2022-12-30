Technical Writing Two


* Adopt a style guide.
* Think like your audience.
* Read documents out loud (to yourself).
* Return to documents well after you've written the draft.
* Find a good peer editor.
* Outline a document. Alternatively, write free form and then organize.
* Introduce a document's scope and any prerequisites.
* Prefer task-based headings.
* Disclose information progressively (in some situations).
* Consider writing the caption before creating the illustration.
* Constrain the amount of information in a single drawing.
* Focus the reader's attention on the relevant part of a picture or diagram by describing the takeaway in the caption or by adding a visual cue to the picture.
* Create concise sample code that is easy to understand.
* Keep code comments short, but prefer clarity over brevity.
* Avoid writing comments about obvious code.
* Focus your commenting energy on anything non-intuitive in the code.
* Provide not only examples but also anti-examples.
* Provide code samples that demonstrate a range of complexity.
* Make a practice of continuous revision.


Self-editing


Adopt a style guide

Many of the documentation projects on the Google Developers site follow the Google Developer Documentation Style Guide. The guide offers detailed guidance on topics such as grammar, punctuation, and documenting computer interfaces. If you've never used a style guide before, Google's guide might seem a little intimidating.

Note: For smaller projects, such as team documentation or a small open source project, you might find the highlights are all you need.

* Use active voice to make clear who's performing the action.
* Format sequential steps as numbered lists.
* Format most other lists as bulleted lists.


* Write in the second person. Refer to your audience as "you" rather than "we".
* Place conditional clauses before an instruction, rather than after.
* Format code-related text as code font.


Think like your audience

Make sure the purpose of your document is clear, and provide definitions for any terms or concepts that might be unfamiliar to your readers.

You can then review your draft with your persona in mind. It can be especially useful to tell your audience about any assumptions you've made.

You can also provide links to resources where they can learn more if they need to brush up on a specific topic

Read it out loud

Depending on the context, the style of your writing can alienate, engage, or even bore your audience.

=> To check if your writing is conversational, read it out loud.
=> Listen for awkward phrasing, too-long sentences, or anything else that doesn't feel natural. 
=> Alternatively, consider using a screen reader to voice the content for you.

Come back to it later

After you write your first draft (or second or third), set it aside. Come back to it after an hour (or two or three) and try to read it with fresh eyes.

Change the context

A change of context when reviewing your own work can help you find things to improve. For a modern take on this classic tip, copy your draft into a different document and change the font, size, and color.


Find a peer editor

- Ask someone to review your document and give you specific, constructive comments.
- Your peer editor doesn't need to be a subject matter expert on the technical topic of your document. But they should be familiar with the style guide you follow.


Organizing large documents


When to write large documents

Some readers respond more positively than others to longer documents.

Consider the following perspectives from two hypothetical readers you're writing documentation for:
* Hong finds reading long documents difficult and disorientating. He prefers to use site search to find answers to his questions.
* Rose is comfortable navigating large documents. She often uses the built-in page search feature in her web browser to find useful information on the current page.

Consider the following guidelines:
* How-to guides, introductory overviews, and conceptual guides often work better as shorter documents when aimed at readers who are new to the subject matter. For example, a reader who is completely new to your subject matter might struggle to remember lots of new terms, concepts, and facts. Remember that your audience might be reading your documentation to gain a quick and general overview of the topic.
* In-depth tutorials, best practice guides, and command-line reference pages can work well as lengthier documents, especially when aimed at readers who already have some experience with the tools and subject matter.
* A great tutorial can rely on a narrative to lead the reader through a series of related tasks in a longer document. However, even large tutorials can sometimes benefit from being broken up into smaller parts.
* Many longer documents aren't designed to be read in one sitting. For example, users typically scan through a reference page to search for an explanation of a command or flag.


Organize a document

	Outline a document

* Before you ask your reader to perform a task, explain to them why they are doing it. For example, the following bullet points illustrate a section of an outline from a tutorial about auditing and improving the accessibility of web pages:
    * Introduce a browser plugin that audits the accessibility of web pages; explain that the reader will use the results of the audit report to fix several bugs.
    * List the steps to run the plugin and audit the accessibility of a web page.
* Limit each step of your outline to describing a concept or completing a specific task.
* Structure your outline so that your document introduces information when it's most relevant to your reader. For example, your reader probably doesn't need to know about the history of the project in the introductory sections of your document when they're just getting started with the basics. Document includes a link to this type of information at the end of the document.
* Consider explaining a concept and then demonstrating how the reader can apply it either in a sample project or in their own work. Documents that alternate between conceptual information and practical steps can be a particularly engaging way to learn.
* Before you start drafting, share the outline with your contributors. Outlines are especially useful if you're working with a team of contributors who are going to review and test your document.


	Outline exercise


* Rearrange the existing topics.
* Add any missing topics you feel should be in an introduction.
* Remove any topics you feel are irrelevant for an introduction.


![Screenshot 2022-12-27 at 19 53 22](https://user-images.githubusercontent.com/25881847/210047930-d8e49d27-70c4-4cea-945e-073319a0d3f6.png)

=> a possible solution

![Screenshot 2022-12-27 at 19 53 30](https://user-images.githubusercontent.com/25881847/210047942-039cfdb1-7ef7-4964-b27d-db99ab696b09.png)

Introduce a document

To set the ground rules for your users, we recommend providing an introduction that includes the following information:
* What the document covers.
* What prior knowledge you expect readers to have.
* What the document doesn't cover.

Note: Remember that you want to keep your documentation easy to maintain, so don't try to cover everything in the introduction.

Introduction exercise

Remove any information you feel is irrelevant in this context and add any information you feel is missing.
![Screenshot 2022-12-27 at 19 56 01](https://user-images.githubusercontent.com/25881847/210047954-10075356-afed-40c6-9b1d-2de4501cd285.png)

=> a possible solution

![Screenshot 2022-12-27 at 19 56 04](https://user-images.githubusercontent.com/25881847/210047966-2cd37c82-009b-4e7a-a052-1864994af90b.png)


Add navigation

Clear navigation includes:
* introduction and summary sections
* a clear, logical development of the subject
* headings and subheadings that help users understand the subject
* a table of contents menu that shows users where they are in the document
* links to related resources or more in-depth information
* links to what to learn next


Prefer task-based headings

Choose a heading that describes the task your reader is working on.

![Screenshot 2022-12-27 at 19 57 36](https://user-images.githubusercontent.com/25881847/210047982-cefbdc70-c58d-46de-965e-bdbd26c8d13f.png)


Provide text under each heading
Most readers appreciate at least a brief introduction under each heading to provide some context. Avoid placing a level three heading immediately after a level two heading

![Screenshot 2022-12-27 at 20 01 54](https://user-images.githubusercontent.com/25881847/210047993-c3952558-51a7-4d57-8829-1952904995f3.png)

A brief introduction can help orient the reader:

![Screenshot 2022-12-27 at 20 02 03](https://user-images.githubusercontent.com/25881847/210048007-0d069073-44a1-4521-852f-6231f39bbe9e.png)



Disclose information progressively

The following techniques can help you incorporate progressive disclosure in your documents:
* Where possible, try introducing new terminology and concepts near to the instructions that rely on them.
* Break up large walls of text. To avoid multiple large paragraphs on a single page, aim to introduce tables, diagrams, lists, and headings where appropriate.
* Break up large series of steps. If you have a particularly long list of complicated steps, try to re-arrange them into shorter lists that explain how to complete sub-tasks.
* Start with simple examples and instructions, and add progressively more interesting and complicated techniques. For example, in a tutorial for creating forms, start by explaining how to handle text responses, and then introduce other techniques to handle multiple choice, images, and other response types.


Illustrating

In fact, when it comes to reading technical material, the vast majority of adults are still little kids—still yearning for pictures rather than text.

![book_readers](https://user-images.githubusercontent.com/25881847/210048015-1a286391-74e4-4616-b70f-c932364608e2.jpg)


Write the caption first

Good captions have the following characteristics:
* They are brief. Typically, a caption is just a few words.
* They explain the takeaway. After viewing this graphic, what should the reader remember?
* They focus the reader's attention. Focus is particularly important when a photograph or diagram contains a lot of detail.


Constrain the amount of information in a single drawing

Just as you avoid overly-long sentences, strive to avoid visual run-ons. As a rule of thumb, don't put more than one paragraph's worth of information in a single diagram.

Focus the reader's attention

![Screenshot 2022-12-27 at 20 15 03](https://user-images.githubusercontent.com/25881847/210048037-3147b570-79ee-4605-94a9-fdc2c2fac616.png)

Readers don't know what to focus on.

![Screenshot 2022-12-27 at 20 15 06](https://user-images.githubusercontent.com/25881847/210048045-8a140fc4-4010-4c76-be7a-76d936b89413.png)

Readers focus on a shape that breaks the pattern

Illustrating is re-illustrating

As with writing, the first draft of an illustration is seldom good enough. Revise your illustrations to clarify the content. As you revise, ask yourself the following questions:
* How can I simplify the illustration?
* Should I split this illustration into two or more simpler illustrations?
* Is the text in the illustration easy to read? Does the text contrast sufficiently with its background?
* What's the takeaway?

Illustration tools
There are many options available for creating diagrams. Three options that are free or have free options include:
* Google Drawings
* diagrams.net
* LucidChart
When exporting diagrams from these tools to use in documentation, it is usually best to export the files as Scalable Vector Graphics (SVG). The SVG format easily scales diagrams based on space constraints so that no matter the size, you end up with a high quality image.




Create sample code


Good samples are correct and concise code that your readers can quickly understand and easily reuse with minimal side effects.


Correct

Sample code should meet the following criteria:
* Build without errors.
* Perform the task it claims to perform.
* Be as production-ready as possible. For example, the code shouldn't contain any security vulnerabilities.
* Follow language-specific conventions.


Running sample code

Good documents explain how to run sample code.

Users don't always perform the preceding activities properly. 

In some situations, users prefer to run or (experiment with) sample code directly in the documentation. ("Click here to run this code.")


Understandable

Follow these recommendations to create clear sample code:
* Pick descriptive class, method, and variable names.
* Avoid confusing your readers with hard-to-decipher programming tricks.
* Avoid deeply nested code.
* Optional: Use bold or colored font to draw the reader's attention to a specific section of your sample code. However, use highlighting judiciously—too much highlighting means the reader won't focus on anything in particular.

![Screenshot 2022-12-27 at 20 38 01](https://user-images.githubusercontent.com/25881847/210048056-63fbe6de-b600-47fc-97b8-0979a1671c48.png)

Answer 3 is the best choice here. Although it is tempting to keep sample code as short as possible, omitting parameter names makes it harder for novices to learn.

Commented

Consider the following recommendations about comments in sample code:
* Keep comments short, but always prefer clarity over brevity.
* Avoid writing comments about obvious code, but remember that what is obvious to you (the expert) might not be obvious to newcomers.
* Focus your commenting energy on anything non-intuitive in the code.
* When your readers are very experienced with a technology, don't explain what the code is doing, explain why the code is doing it.

Reusable

For your reader to easily reuse your sample code, provide the following:
* All information necessary to run the sample code, including any dependencies and setup.
* Code that can be extended or customized in useful ways.

The example and the anti-example

good

![Screenshot 2022-12-27 at 20 38 43](https://user-images.githubusercontent.com/25881847/210048074-cdae988f-3634-4d8f-9d71-f23368adf8b2.png)

bad

![Screenshot 2022-12-27 at 20 38 46](https://user-images.githubusercontent.com/25881847/210048086-0071d57c-be2e-4ee0-b37a-1f26a641ed05.png)

Sequenced

A good sample code set demonstrates a range of complexity.

![Screenshot 2022-12-27 at 20 49 05](https://user-images.githubusercontent.com/25881847/210048096-58db72fc-d9ea-42f9-88f8-852d29c262e3.png)

good
