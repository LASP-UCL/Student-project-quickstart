# Quickstart your project
Congratulation on your project!   
The purpose of this document is to guide you your journey on a short-term Machine Learning project. 
The document is split into three main parts: the main activities in which you will be involved: i) Reading, ii) Coding and iii) Writing.

To start a new project, please send an email to `lasp@live.ucl.ac.uk` with subject `Student project: <your-student-ID>, <name-surname>`.
There is a list of available projects to work on at [this link]().
In the email, please speficy which project you will work on, the GitHub username you will use throughout, and the url of the repository you just created (see XXX for guidelines on how to create the repository).
Please fill this form a week in advance you intend to start your project. This allows us enough time to grant you the necessary permissions on GitHub.

#### Skills we expect before you start
For a machine learning projects there are some skills that is useful to acquire or deepen:
- Have elements of linear algebra, statistics and a rough understanding of what machine learning is.
- Have a basic undertanding of the [experimental method](https://en.wikipedia.org/wiki/Experiment) for research.
- Have a basic understanding of [linux](https://ubuntu.com/tutorials/command-line-for-beginners#1-overview)
- Being able to write and run Python code
- Know how to compartmentalise running code, for example using [virtual environments](https://docs.python.org/3/library/venv.html) and [conda environments](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).

If you lack some of this skills, do not worry. Lower in this guide, there is a list of free resources to bridge the gaps. Please consider taking the time to engage in the study of the above, before starting your project. The average learning time is around a full two weeks of study.
In our experience, starting your project without the elements above could make it a very hard challenge to complete it.




## 1. Reading
As with every research journey, you will start from reading!
It is very likely that you will read a high number of documents, and get to the point when a minimal organisation of the literature is required.
There are a number of literature management software available for free, among which, we recommend:
- [`My Library` in Google Scholar](https://scholar.google.com/scholar?scilib=1&hl=en&as_sdt=0,5)
- [Zotero](https://www.zotero.org/)
- [Mendeley](https://www.mendeley.com/guides/desktop/)

Below are some reading resources concerning topics that you may encounter in your project.

### Statistics and Linear Algebra
To refresh some concepts from statistics and linear algebra, here are some pointers:
- "Machine Learning: A Probabilistic Perspective", by Murphy: Sections 2.1-2.4  (https://ebookcentral.proquest.com/lib/ucl/reader.action?docID=3339490)
- "Introduction to Applied Linear Algebra", by Boyd and Vandenberghe. Section 1, 2 (only 2.1), 3 (3.1, 3.2, 3.3), 6 (http://vmls-book.stanford.edu/vmls.pdf)


### Machine Learning
Your project will include machine learning aspects and it is of vital importance that you get a full understanding on the subject. The topic is vast and there are multiple tutorials and online courses that can introduce you to the topic. We strongly recommend you the [introduction to ML course](https://www.coursera.org/learn/machine-learning#syllabus) by Andrew Ng at Stanford or Coursera.


### Deep Learning
[Goodfellow, Y. Bengio, and A. Courville. Deep Learning. MIT Press, 2017.](http://www.deeplearningbook.org) is a great resource to learn about Deep Learning, convering a wide part of the subject with details.

- Deep Neural Networks
  - Essential introduction to NN in Chapter 6.
  - Regularization for neural networks: Sections 7.2 (norm constraints on weights), 7.4 (dataset augmentation), 7.8 (early stopping), 7.12 (dropout) in Chapter 7.
  - Chapter 8 will then lead to optimization for neural network training: Sections 8.3, 8.and 8.5.  
- Convolutional Neural Networks
  - Chapter 9: Sections 9.1 - 9.4 will provide you the key understanding of CNN while Section 9.7 will cover data types.
- Recurrent Neural Networks
  - Most of Chapter 10.
- Auto-encoders
  - Chapter 14  offers an overview auto-encoders including their architecture, optimization, regularization, and use-cases.
- Applications
  - Chapter 12  provides information on deep learning applications in computer vision (Section 12.2), natural language processing (Section 12.4) and recommender systems (Section 12.5.1). Additional / alternative applications will be presented during the session. 
- Transformers
  - A. Zhang, Z. C. Lipton, M. Li and A. J.Smola, “Dive into Deep Learning”, 2021 (https://d2l.ai/d2l-en.pdf). Particularly, Chapter 10 (Sections 10.6 and 10.7). 
  - The reader can also refer to the following tutorial: Benyamin Ghojogh and Ali Ghodsi, “Attention Mechanism, Transformers, BERT, and GPT: Tutorial and Survey”.

Many other excellent books are available and here we provide you few pointers:
- C. Bishop. Pattern Recognition and Machine Learning. Springer, 2006.
- S. Shalev-Shwartz and S. Ben-David. Understanding Machine Learning. Cambridge University Press, 2014.
- K. P. Murphy. Machine Learning: A Probabilistic Perspective. MIT Press, 2012. 


### Graph Signal Processing
If you have a project with us, chances are you will be working with graphs. We collected a number of overview papers at [this](https://www.dropbox.com/sh/r1atdx82zqqnu1q/AAAMFyldYIykg0rffjBtxiVba?dl=0) link .
The numbers in the paper suggest the order you should follow when reading them to ensure a smooth introduction to the topic. 
- Further material is available at https://geometricdeeplearning.com. 
- Perspectives on graph-based learning https://youtu.be/PLGcx65MhCc?t=1692 
- Course material offered by Stanford University, CS224W Machine Learning on Graphs 
- [slides] http://web.stanford.edu/class/cs224w/ 
- [lectures] https://www.youtube.com/playlist?list=PLoROMvodv4rPLKxIpqhjhPgdQy7imNkDn
- A Gentle Introduction to Deep Learning for Graphs: https://arxiv.org/pdf/1912.12693v2.pdf 
- Very introductory video to understand at how level GNNs https://www.youtube.com/watch?v=2KRAOZIULzw&t=409s
https://www.youtube.com/watch?v=wJQQFUcHO5U&t=363s


## 2. Coding and running code
To write your code we recommend [Visual Studio Code](https://code.visualstudio.com/) for its simplicity of use and its versatility with remote code execution. We also suggest these extensions for Visual Studio Code. See [here](https://code.visualstudio.com/docs/editor/extension-marketplace) for how to install extensions.
- Remote-SSH
- GitLens
- Jupyter

There are two main components that can help you organise your project and track your experiments: i) using version control on your code and ii) using a logging system for your experiments.

### Git and GitHub
We expect the code used to run your experiments to be hosted on GitHub. Note that this code is public.
Because this is your own personal project, we recommend hosting it on your own GitHub page. We will then [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) your repository in the https://github.com/LASP-UCL organisation.
If you are not familiar with Git or GitHub, [this](https://github.com/education/github-starter-course) preliminary introduction is a good start.

To initiate your project, create a new repository using [this](https://github.com/LASP-UCL/Your-project-title) template. [Here](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) is how to create a new repository from a template.

### Experiments log
[Weights and Biases](https://wandb.ai/) is a great free tool to maintain a log of your experiments, and strongly suggested.
[Here](https://docs.wandb.ai/quickstart) is a quickstart for wandb, and [here](https://docs.wandb.ai/guides/integrations/pytorch) is the bespoke guide for the Pytorch integration. You can use wandb also to communicate your results to us, either informally or using the useful _Reports_ feature.

### Machine Learning libraries
When writing your machine learning code, [Pytorch](https://pytorch.org/tutorials/beginner/basics/intro.html) could be a great library to start, for its trade-off between clarity and performance.

### Python tutorials
We recommend you to review some Python Tutorials available Linkedin Learning (https://www.ucl.ac.uk/isd/linkedin-learning) such as this tutorial (https://www.linkedin.com/learning/python-data-analysis-2015) or another tutorial (https://www.linkedin.com/learning/numpy-data-science-essential-training). 

### Pytorch Tutorials 
This course will also require you to develop programs within a Python deep learning framework. We recommend you review relevant PyTorch tutorials available at https://pytorch.org/tutorials/ (e.g. Learning the Basics and Learning Pytorch with Examples).

[Google Colab](https://colab.research.google.com/) is a very practical, and we encourage you to use it. 



### High Performance Computing (HPC) at UCL
UCL offers a High Performance Computing infrastructure to run expensive computation. In machine learning project, especially in Deep Learning and Deep Reinforcement Learning, it is very likely that you will need one or more GPU to run your experiments.
The Department of Electronic and Electrical Engineering has a very clear guide on the [servers available](https://intranet.ee.ucl.ac.uk/it/servers/gpu) and on how to [connect to them](https://intranet.ee.ucl.ac.uk/it/remote-access/remote-access-to-linux).
When using these servers, please minimise the amout of computation, and don't occupy GPUs that you do not need.


## 3. Writing (scientific reports)
Developing or improving your writing skills is of paramount importance for your project. Remember that you will be marked based on your report. We 
recommend the following, precious guidelines on how to write a literature review as well as how to report scientific work:
- Randolph, Justus. "A guide to writing the dissertation literature review." Practical Assessment, Research, and Evaluation 14.1 (2009): 13.
- Mack, Chris A. "How to write a good scientific paper: title, abstract, and keywords." Journal of Micro/Nanolithography, MEMS, and MOEMS 11.2 
(2012): 020101. 
You can find both PDFs at this link [here](https://www.dropbox.com/sh/fnipgnhykwbl787/AAB_SF3wVfn2u9dYhWE4JsIfa?dl=0).
