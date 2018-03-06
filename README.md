# Evaluating OCR data: an introductory guide
## What to Evaluate
In general, when evaluating the quality of an OCR corpus, we consider three features:
1. Character accuracay rate: the percentage of characters that have been accurately transcribed.
2. Word accuracy rate: the the percentage of words that have been accurately transcribed.
3. Error distribution: the ways that errors are distributed across pages and documents.

### Further reading on evaluation:

## How to evaluate:
To evaluate word and character accuracy, there are several approaches.

1. Ground-truth transcription: In this approach, you can hand-transcribe a subset of the documents in your corpus, and compare the results with the OCR output. This is the simplest method, but it has some costs: not all pages will have the same accuracy rates; hand transcription can be time intensive; hand-transcription can introduce errors.
2. Dictionary evaluation: In this approach, the words in the OCR corpus are compared to words in a dictionary. This can give you a rough estimate of the "wordiness" of your corpus, but it comes with costs, especially if your corpus is multilingual or has a lot of proper nouns or uncommon vocabulary.
3. Language models: more sophisticated models can evaluate, not simply whether the words exist in a dictionary, but rather the degree to which the words in your corpus look like they could be words in real life. This method will allow for a much more complex vocabulary, and the models can be quite sophisticated, but it might miss character-level errors that produce an output that looks like words, but aren't.

### Further reading on evaluation methods.

## Resources:
* Automatic Evaluation of OCR quality. https://ryanfb.github.io/etc/2015/03/16/automatic_evaluation_of_ocr_quality.html
* A half-decent OCR normalizer for English texts after 1700. https://tedunderwood.com/2013/12/10/a-half-decent-ocr-normalizer-for-english-texts-after-1700/
* How good are our texts, really? https://cligs.hypotheses.org/371
