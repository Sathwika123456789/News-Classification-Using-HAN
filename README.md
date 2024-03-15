Introduction:

Text classification has evolved into one of the most difficult tasks to do in the wake of the
rise of artificial intelligence. One of the essential tasks in natural language processing is text
classification. The objective is to give text labels. Topic labelling, sentiment categorization,
and spam detection are just a few of its many uses. A linear model or kernel methods are
then applied to this representation in traditional approaches to text classification. These
approaches describe documents with sparse lexical characteristics, such as n-grams. We can
state that artificial intelligence is a field that works to create intelligent models that are
similar to humans in order to make our tasks easier as a whole. Although many advanced
NLP algorithms have tried, they have not been able to match our astonishing proficiency in
text classification.
Hence, the question is, what makes us humans different from other animals? How are texts
categorised?
First off, we understand many words—not all of them—and we can infer even obscure
terms from the way sentences are put together. The meaning that is implied by that string
of words (sentence) is then clear. The meaning of a paragraph or article is then deduced
from that string of sentences. In the Hierarchical Attention model, a similar strategy is
employed.
In order to extract the words that are crucial to the meaning of the sentence and aggregate
the representation of those informative words to build a sentence vector, it uses stacked
recurrent neural networks on the word level, followed by an attention model. The derived
sentence vectors are then subjected to the same process, which creates a vector that
understands the content of the provided document and can then be used for text
categorization.
"Words make sentences, and sentences make documents," is the central tenet. The goal is
to determine a sentence's meaning from its words, and then use those sentences to
determine a document's meaning. Nevertheless, not all words have the same weight. More
so than others, some of them define a sentence. So that sentence vector can pay greater
attention to "important" words, we employ the attention model.
Bidirectional RNN and Attention networks make up the two components of the attention
model. Whereas a bidirectional RNN learns the meaning of the words in a sequence and
produces a vector for each word, an attention network uses a shallow neural network to
obtain weights for each word vector. The representation of those words is then combined
to create a sentence vector by computing the weighted sum of each vector. The entire
sentence is contained in this weighted sum. To ensure that the final vector captures the
essence of the entire document, the same process is used for sentence vectors. Hierarchical
attention networks are what it is called since it features a two-level attention model.
In contrast to most implementations of text classification, a Hierarchical Attention Network
(HAN) also takes into account the hierarchical structure of documents (document -
sentences - words) and has an attention mechanism that can locate the most crucial words
and sentences in a document while taking context into account. Some approaches merely
provide relevance weights based on the words that came before them.
In conclusion, HAN seeks to address the following issues that earlier studies did not:
• It's not necessary to grasp every word of every sentence in order to comprehend the
primary point of a document.
• It is important to take into account how a word's meaning can change based on the
situation. The word "beautiful," for instance, can have different connotations depending on
how it is used: "The bouquet of flowers is gorgeous" and "The cuisine is pretty terrible."
As a result, HAN is more accurate in determining the class of a given document.
Look at this example:
Five sentences make up this Yelp review that we have here. The sentences that are
highlighted in red have a stronger significance than the rest, and therein, the adjectives
amazing and delicious are mainly responsible for the review's upbeat tone. This example
demonstrates the Same claim we made earlier, which we also intuitively understand: not all
sections of a document are equally important to understand its fundamental meaning.

Architecture Diagram:
![image](https://github.com/Sathwika123456789/News-Classification-Using-HAN/assets/138215124/531f5cfb-2199-4ae4-bd6c-0e9355269207)

Dataset:
https://www.kaggle.com/code/hsankesara/news-classification-using-han/input?select=News_Category_Dataset_v2.json
