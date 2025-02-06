## Humanities Research with Generative AI ##

### 1. About this Tutorial ###
This tutorial will walk you through two exercises using generative AI for humanities research.
Please keep in mind there are ethical issues with using generative AI:
- the models and apps generate profit for their companies while the training data includes art, writing, code without compensating the original creators
- there is a debate about energy and water usage (here is a [January 2025 MIT article](https://news.mit.edu/2025/explained-generative-ai-environmental-impact-0117) on the issue
- low wage workers classify, tag, annotate, or moderate the data
- creating chatbots that talk like another person or group of people can be considered offensive (for example, accusations of digital blackface)

This tutorial lives online (with live links) at https://github.com/ctschroeder/tutorials/blob/master/generativeAI.md

Last edited for Dr. Schroeder's Spring 2025 Intro DH course.

Note: This technology is changing very fast.

This work is licensed by Caroline T. Schroeder under a [Creative Commons Attribution-NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/)

#### Do you want to level up? ####
Because this course includes students of all levels of experience with generative AI models and apps, this tutorial will not be training or customizing our own apps (although that is quite possible to do).
If you have experience programming or training models already, you may choose to train an app for a Humanities research purpose. However, I cannot give you coaching on this. You're on your own. Common trainable apps are:
- Llama
- [Chatdoc](https://chatdoc.com/)
- a ton more

If you choose this option:
1. Be sure you are training your app for a _humanities_ objective
2. Your lab report should
   - explain your humanities objective, what model you trained, what additional documents/sources you used for the training
   - link to/cite all of the above
   - link to the app you created if it's online
   - provide a transcript of some humanities task you asked it to do
   - evaluate the results (accuracy? helpfulness? ethical issues)

### 2. Text Analysis with Generative AI ###

#### A note about corpora ####
Keep in mind that the _free_ versions of these apps limit the number of documents you can upload and the size of documents. 
- If you already have a subscription to a paid version of ChatGPT, Gemini, Copilot, Claude, etc., please use that.
- If you are using a free version, be certain you are uploading the document(s) you want.

Here is a [plain text file of Frankenstein](https://github.com/ctschroeder/tutorials/blob/master/Frankenstein-half-projectgutenberg.txt) you can download. (Click on the icon with the down arrow above the text on the right.)
Here is a [plain text file of the first half of Frankenstein](https://github.com/ctschroeder/tutorials/blob/master/Frankenstein-half-projectgutenberg.txt) you can download and use with DeepSeek. (Click on the icon with the down arrow above the text on the right.) (When I uploaded full book to DeepSeek, it told me it could only process the first 56%.)
I got the text from [Project Gutenberg](https://www.gutenberg.org/files/84/84-h/84-h.htm). Please link to the version you use and cite Project Gutenberg as the source.

#### Take notes ####
As you are going through this process, be sure to take notes in your Notebook about what app you are using, what files you are uploading, what prompts you are giving the app. 

You may want to take regular screenshots.

I will ask you at the end to use your cursor to select the whole chat + responses and copy it to another document to turn in. 

#### Text analysis on DeepSeek ####
We are going to try this on DeepSeek since that textfile works with DeepSeek's limits. If you have a paid subscription to another app or just want to try a different one, please feel free!

1. Go to [DeepSeek's chat interface](https://chat.deepseek.com/).
2. Consider what kind of text analysis you want to do (word frequencies, bi-grams and tri-grams frequencies, collocates, etc.) Ask DeepSeek if it can do the kind of text analysis you want to do if you upload a document.
3. Read the answer.
4. Using the information in its answer, devise a prompt asking DeepSeek to perform some kind of text analysis on the document you will upload. Some things to consider:
   - You may want to start by telling the app to assume a role (researcher, student, digital humanities scholar, professor, whatever you think is a good role for the task). Write a command asking it to assume that role. That's the first sentence of your prompt.
   - Continue your prompt by instructing DeepSeek to perform some form of text analysis that we already have done with Voyant or AntConc: bi-grams or tri-grams frequencies, word frequencies, collocates.
   - Consider whether you want DeepSeek to do text analysis including stop words or ignoring stop words. Include that information in your prompt.
5. When you give DeepSeek the prompt, also click on the paperclip icon to upload your text to analyze and enter the prompt and text.
6. Copy your prompt to another document
7. Copy the results to another document
8. If you don't get any results or your results look really wrong, you may need to give it another prompt to give it more detail on what to do or tell it what it's doing wrong.
9. Now look at the results and evaluate them:
   - do they look plausible?
   - is there anything strange? (For example: when I asked for top 25 tri-grams, numbers 8 through 25 were _the same trigram!_ I had to ask it to fix it.)
10. Ask Deepseek to explain its method or process in doing this text analysis. Copy the results to another document
11. Now select this entire transcript and copy that to another document. Be sure to save all the documents!
12. Do not close the chat

#### Compare DeepSeek's results to Voyant ####
1. Navigate to https://voyant-tools.org
2. upload the same document to Voyant that you used in DeepSeek
3. In the Cirrus/Word Cloud Tool, you can click the option to see the list of word frequencies. Do that. (Or look at the other tools like collocates, and for n-grams open the Voyant tool called "phrases")
4. Set the settings in Voyant (the little icon that looks like a toggle button) so that you have the same settings regarding stop words
5. Look at the word frequencies in Voyant.
   - Are they the same as the results in DeepSeek?
   - If they're not the same, are they similar?
   - One thing I noticed in my test: Voyant counts a possessive word ("father's") as a separte word from the plain word ("father"). Some gen AI transformers tokenize the 's as its own word.
   - If the frequencies are very similar but a bit different for some words, you might try searching both forms of the relevant word in Voyant (type underneath the word list "father" and "father's" and it will tell you the frequencies of those two words.)
   - download the result
   - *you can also do the above in AntConc if you'd like!*
6. If the results are different, go back to DeepSeek and tell it there is a difference in Voyant. Tell it what the difference is and ask it why.
7. Copy your question and results to a new document
8. Consider what you think is going on: is the gen AI accurate but using different methods (like different tokenizing) or is it inaccurate?

#### For your Lab Report ####
Write up your evaluation of generative AI for text analysis. Document your tool, source, etc., as usual. 
Tell me how well the app performed in the task. You can compare it to Voyant or AntConc's results.

Consider: does the generative AI app provide good results? Is there anything this generative AI app can't do that Voyant and AntConc can do? (If so, there may be a paid app out there that does, just fyi. You can search for it.)

I don't expect more than a paragraph or two for this section.

### 3. Document Transcription with ChatGPT or Gemini ###
Again: keep in mind that the _free_ versions of these apps limit the number of documents you can upload and the size of documents. 
- If you already have a subscription to a paid version of ChatGPT, Gemini, Copilot, Claude, etc., you may want to use that.
- If you are using a free version, be certain you are uploading the document you want. Depending on the app, you might only be able to upload one document per day.

1. Select and download an image from the ones I provide on Canvas. All of them are from the OU Western History collections. *When you write your Lab Report, be sure to cite item at the Western History website.*
2. Navigate either to [ChatGPT](https://chatgpt.com) or to [Google Gemini](https://gemini.google.com). (In my experience DeepSeek was not as accurate, and Copilot could not process the pdf of a letter I gave it but refused to process the jpg without upgrading to the paid version. So use ChatGPT or Gemini.)
3. Compose a prompt asking the app to transcribe a handwritten document in the file you will give it. Be sure to tell it if the image is of two pages facing each other (like an open book) or one page. You might want to give it a role (archivist? historian? family member reading a letter?)
4. Type in the prompt and upload the image. (Be sure you upload the one you want-ChatGPT will only let you do one a day).
5. Copy your prompt and results into a separate document.
6. If you don't get any output, you may have to revise the prompt and prompt it again.
7. Evaluate the results. How many letters does it get wrong?

#### For your Lab Report ####
Write up your evaluation of generative AI for handwritten text recognition. Document your tool, source, etc., as usual. 
Tell me how well the app performed in the task. Consider: does the generative AI app provide good results? Would you use it if you were conducting historical research?

I don't expect more than a paragraph or two for this section.

## Attach prompts and output ##
At the end of your lab report, copy over the relevant transcripts of your conversations for the above. 

