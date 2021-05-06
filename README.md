# Predatory Wasp of the Palisades: Man's Quest for Meaning Through the Eyes of the Machine

# 1) Problem Framing 

- **Problem**: 

  - When we think of the two words, "assisted" and "vision", a few things come to mind; The visually impaired, high-tech glasses with infrared capabilities and sci-fi, Terminator Esque visual assessment. Though the last two were in jest, assisted vision research inches us ever closer to making those types of ideas realities. In a nutshell, assisted vision is a form of artificial intelligence that allows us to interact with our visual world in more interactive, intuitive, and intelligent ways, letting the machine "see" for us. And for obvious reasons, the research and advancements could prove to be especially beneficial to the visually impaired and blind community.\
285 million people globally are visually impaired, 39 million of whom are blind. An analysis of the 1999 Survey of Income and Program Participation (CDC, 2001) revealed blindness or vision problems to be among the top 10 disabilities among adults aged 18 years and older. Vision loss has serious consequences for the individual as well as those who care for and about people who have compromised vision, because it impedes the ability to read, drive, prepare meals, watch television, and attend to personal affairs. Reduced vision among mature adults has been shown to result in social isolation, family stress, and ultimately a greater tendency to experience other health conditions or die prematurely.\
Assisted vision can aid in adding accessibility for the entire community through interactive technologies, however, those same technologies can potentially prove to be beneficial for various disenfranchised groups as well. Globally, 12% of the world are considered functionally illiterate and of that 126 million are children (source: UIS, 2014). A large factor lending to mass illiteracy is the lack of qualified teachers in rural areas. With assisted vision technology, a highly trained model can be just as good as a human in teaching children the basics of reading and speech through automated captioning.


- **Porposed Solution**:  
  - The field of assisted vision technology is expansive, though still relatively untapped in terms of its potential. Many papers and journals have been published expounding on the subject, though few tackle the added functionality of incorporating machine conversational capabilities and text to speech integration. I intend to add to the conversation and lay the groundwork for future research and development by building and implementing three different auto-captioning, assisted vision models based on the top research papers on the subject.

- **Ideal Outcome**: 
  - The ideal outcome would be deploying a web hosted model that can generate human like, accurate image descriptions and conversational responses through speech-to-text and text-to-speech. 

- **Success Metrics**:
  - Success will be based on the interpreability of the AI's initial descriptions and responses. Because the target variable isn't quantifiable, it largely depends on the models ability to "sound" human, or at the very minimum to give responses that can be understood by humans.

- **Evaluation Metrics**:

  - Automatically describing an image with a sentence is a long-standing challenge in computer vision and natural language processing. Due to recent progress in object detection, attribute classification, action recognition, etc., there is renewed interest in this area. However, evaluating the quality of descriptions has proven to be challenging. For that reason there are a wide range of project specific evaluation metrics that will be used to evaluate our model:

    - *Ramakrishna Vedantam, et al. of Cornell University proposed an automated metric, Consensus-based Image Description Evaluation (CIDEr) that evaluates the quality of the description based on captured human concensus. A publically available version of the metric, the CIDEr-D, is available through Microsoft's COCO evaluation Server.*
   
    - *METEOR, or the Metric for Evaluation of Translation with Explicit ORdering, is a metric for the evaluation of machine translation output. The metric is based on the harmonic mean of unigram precision and recall, with recall weighted higher than precision. It also has several features that are not found in other metrics, such as stemming and synonymy matching, along with the standard exact word matching.*

    - *BLEU, or the bilingual evaluation understudy,  is an algorithm for evaluating the quality of text which has been machine-translated from one natural language to another. Quality is considered to be the correspondence between a machine's output and that of a human.*

    - *ROUGE, or the Recall-Oriented Understudy for Gisting Evaluation, is a set of metrics and a software package used for evaluating automatic summarization and machine translation software in natural language processing. The metrics compare an automatically produced summary or translation against a reference or a set of references (human-produced) summary or translation.*

    - *NIST is a method for evaluating the quality of text which has been translated using machine translation. It is based on the BLEU metric, but with some alterations. Where BLEU simply calculates n-gram precision adding equal weight to each one, NIST also calculates how informative a particular n-gram is. That is to say when a correct n-gram is found, the rarer that n-gram is, the more weight it will be given.*

- **Final Problem Statement**: 

  - Blindness and illiteracy are two seemingly disconnected global issues, both responsible for the degradation of the quality of life for millions around the world. However, unrelated they may be, I propose that with the aid of technology, both groups can enjoy better lives, increased quality of living, and new, better opportunities to live as normal lives as possible. Though the road towards tackling these issues is a long one, I hypothesize that with Deep Learning we can begin making strides on that path. I set out to use a myriad of machine learning techniques through translating and implementing algorithms from three research papers, taking three different approaches to the same Data Science problem, to create a model that can generate human-like image descriptions.

--------

# 2) Data Construction 

* Link to raw dataset(s) here:
  - [Training Images](http://images.cocodataset.org/zips/train2014.zip)

  - [Testing Images](http://images.cocodataset.org/zips/test2014.zip)

  - [Validation Images](http://images.cocodataset.org/zips/val2014.zip)

  - [Image Caption Annotation](http://images.cocodataset.org/zips/val2014.zip)

  - [Yandex.Toloka NLP Dataset](http://convai.io/data/data_tolokers.json)

  - [DeepHack.Chat NLP Dataset](summer_wild_evaluation_dialogs.json.)


- Data Citations/Sources:
  - [Common Objects in Context Website](https://cocodataset.org/#download/)
  - [ConvAI3 Website](http://convai.io/data/)

----------

# 3) Sources
 - [Bahdanau Attention Documentation](https://d2l.ai/chapter_attention-mechanisms/bahdanau-attention.html)

 - [Haoran Wang, Yue Zhang, and Xiaosheng Yu: An Overview of Image Caption Generation Methods](https://www.hindawi.com/journals/cin/2020/3062706/)

 - [Evergreen Team Blog](https://evergreen.team/articles/automatic-image-captioning.html)

- [IBM Research Blog](https://www.ibm.com/blogs/research/2020/07/image-captioning-assistive-technology/)

- [Visual Dialog](https://visualdialog.org)

- [Department of Computer Science, Cornell University: Learning to Evaluate Image Captioning](https://vision.cornell.edu/se3/wp-content/uploads/2018/03/1501.pdf)

- [Dzmitry Bahdanau, KyungHyun Cho Yoshua Bengio: Neural Machine Translation by Jointly Learning to Align and Translate ](https://arxiv.org/pdf/1409.0473.pdf)

- [Ramakrishna Vedantam, C. Lawrence Zitnick, Devi Parikh: CIDEr: Consensus-based Image Description Evaluation](https://arxiv.org/abs/1411.5726)

- [Peter Anderson, et al: Bottom-Up and Top-Down Attention for Image Captioning and Visual Question Answering](https://arxiv.org/pdf/1707.07998.pdf)

- [Steven Rennie, et al: Self-critical Sequence Training for Image Captioningt](https://arxiv.org/pdf/1612.00563.pdf)

- [Kelvin Xu, et al: Show, Attend and Tell: Neural Image Caption Generation with Visual Attention](https://arxiv.org/pdf/1502.03044.pdf)
---

