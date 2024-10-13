---
layout: menu_page
title: Papers
permalink: /papers/
---

<script src="{{ base.url | prepend: site.url }}/assets/js/show_abstract.js"></script>

<div class="container">
  <div style="width:100%;height:0; padding-top:50%;position:relative;">
    <img src="../images/menu/photo_publications.jpg" style="width:100%; opacity:0.8; position:absolute; top:0; left:0">
  </div>  
  <div class="content">
    <h1>Research</h1>
    <p><span class="cover-desc" style="color:var(--page-desc-color)">This page summarizes my research activities, including publications in academic journals and conference papers.
    More to be added as the time passes by....</span></p>
  </div>
</div>

<p><span class="page-desc">This page summarizes my research activities, including publications in academic journals and conference papers.
More to be added as the time passes by....</span></p>


<!----------------------------------------------------------------------------->

<hr style="height:1px; visibility:hidden;" />

<div style="font-size: 100%;">

  <p>This page overviews my research activities:</p>

  <ul style="margin-top: -10px;">
  <li> &#128218; <a href="#PART_1">Selected academic publications </a></li>
  </ul>

</div>


<!----------------------------------------------------------------------------->

<hr style="height:1px; visibility:hidden;" />
<hr style="height:1px;border-width:0;color:rgb(50,50,50);background-color:rgb(50,50,50)">

<a id="PART_1"></a>

## Paper

### 2024

<ul>
  <li>
  Abhishek Singh, Krishnendu Ghosh
  <dd><b>Curriculum-based Question Generation for Mathematics and Science</b></dd>
  <dd>ArXiv preprint.</dd>
  </li>
</ul>
<ul class="no-bullets">
  <span id="dots9"></span>
  <li><span id="abs9"><p></p><b>Abstract:</b> The purpose of this study is to leverage the use of Natural Language Processing by using Large Language Models (LLMs) so that we can generate questions with respect to the curriculum for Mathematics and Science subjects. To achieve this, we implemented two principal methodologies from the field of Generative-AI: Fine-tuning and Retrieval Augmented Generation (RAG) are two of these approaches. The Fine-tuning approach which we are using is Transfer-Learning using unsloth, which offers two types of Hugging Face's trainers for fine-tuning in its \href{https://github.com/unslothai/unsloth#finetune-mistral-gemma-llama-2-5x-faster-with-70-less-memory}{GitHub repository}: Direct Performance Optimizer (DPO) and Supervised QA Fine-tuning using SFT Trainer. We have used the SFT Trainer, which requires reward modelling or reinforcement learning and works based on labelled data to fine-tune the pre-trained LLM for specific tasks \cite{li2024getting}.
To generate curriculum-based questions, we have used a supervised and labelled dataset of Mathematics questions \cite{hendrycksmath2021}. In contrast, for Science, we have used NCERT (National Council of Educational Research and Training) books issued by CBSE (Central Board of Secondary Education), a fine-tuned model for structured and supervised mathematical questions data, while RAG model for books' PDF for generating contextually appropriate science questions due to containing a large number of factual details in a book.

This research highlights how these approaches can be used to design highly effective instructional tools compatible with generating curriculum-based questions on required subjects. Thus, using these approaches, there is a possibility of developing educational content which is beneficial for students and teachers. </span></li>
  <li>
    <button class="btn" onclick="show_abstract(dots_id = 'dots9', abs_id = 'abs9', btn_id = 'b9')" id="b9">&#128220; Abstract</button>
    <button class="btn" onclick="window.open('https://arxiv.org/abs/2407.13009')" type="button">&#128214; PDF</button>
  </li>
</ul>
<p></p>
