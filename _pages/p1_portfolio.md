---
layout: menu_page
title: Portfolio
permalink: /portfolio/
image: ../images/menu/photo_portfolio.jpg
---

<meta charset="UTF-8">

<img src="../images/menu/photo_portfolio.jpg" style="width:0%; height:0%; top:0; bottom:0">

<div class="container">
  <div style="width:100%;height:0; padding-top:50%;position:relative;">
    <img src="../images/menu/photo_portfolio.jpg" style="width:100%; opacity:0.8; position:absolute; top:0; left:0">
  </div>  
  <div class="content">
    <h1>Portfolio</h1>
    <p><span class="cover-desc" style="color:var(--page-desc-color)">My public ML portfolio includes projects on different topics, including generative AI, NLP, computer vision, and tabular data. To see more of my work, visit my <a href="https://github.com/kozodoi">GitHub page</a>, download my <a href="https://kozodoi.me/cv.pdf">CV</a> or check out the <a href="https://kozodoi.me/about/">about</a> page.</span></p>
  </div>
</div>

<p><span class="page-desc">My public ML portfolio includes projects on different topics, including generative AI, NLP, computer vision, and tabular data. To see more of my work, visit my <a href="https://github.com/kozodoi">GitHub page</a>, download my <a href="https://kozodoi.me/cv.pdf">CV</a> or check out the <a href="https://kozodoi.me/about/">about</a> page.</span></p>


<!----------------------------------------------------------------------------->

<script src="{{ base.url | prepend: site.url }}/assets/js/read_more.js"></script>
<script src="{{ base.url | prepend: site.url }}/assets/js/accordion.js"></script>

<hr style="height:1px; visibility:hidden;" />

<div style="font-size: 100%;">

  <p>My portfolio features the following projects:</p>

  <ul style="margin-top: -10px;">
  <li> &#128214; <a href="#PROJECT_1">Transformer from Scratch(Implementing ML Papers)</a></li>
  <li> &#129516; <a href="#PROJECT_2">Finetuning Minstral 7b for Curriculam Based Question Generation</a></li>
  <li> &#128200; <a href="#PROJECT_3">Retrieval Augmented Generation Model from LLaMa-2</a></li>
  <li> &#128200; <a href="#PROJECT_3">Disease Recognizer using word vector embeddings</a></li>
  </ul>

  <p>Scroll down to see more generative AI and ML projects grouped by application domains. Click "read more" to see project summaries, and follow GitHub links for code and documentation. </p>

</div>


<!----------------------------------------------------------------------------

<hr style="height:1px; visibility:hidden;" />

<a id="PROJECT_1"></a>
<div class="card">
  <h2><b> Text Readability Prediction with Transformers </b></h2>
  <img src="https://kozodoi.me/images/portfolio/fig_books.jpg" alt="Notebook" style="width:100%">
  <h3> Highlights </h3>
  <ul>
  <li> developed a comprehensive PyTorch / HuggingFace text classification pipeline </li>
  <li> build multiple transformers including BERT and RoBERTa with custom pooling layers </li>
  <li> implemented an interactive web app for custom text reading complexity estimation </li>
  </ul>
  <p> <b>Tags:</b> natural language processing, deep learning, web app </p>
  <span id="dots1"><p></p></span>
  <span id="more1">
  <h3> Summary </h3>
  <p> Estimating text reading complexity is a crucial task for school teachers. Offering students text passages at the right level of challenge is important for facilitating a fast development of reading skills. The existing tools to estimate text complexity rely on weak proxies and heuristics, which results in a suboptimal accuracy. In this project, I use deep learning to predict the readability scores of text passages. </p>
  <p> My solution implements eight transformer models, including BERT, RoBERTa and others in PyTorch. The models feature a custom regression head that uses a concatenated output of multiple hidden layers. The modeling pipeline includes text augmentations such as sentence order shuffle, backtranslation and injecting target noise. The solution places in the top-9% of the Kaggle competition leaderboard. </p>
  <p> The project also includes <a href="https://kozodoi-text-readability-prediction-web-app-ddrfmw.streamlit.app">an interactive web app</a> built in Python. The app allows to estimate reading complexity of a custom text using two of the trained transformer models. The code and documentation are available <a href="https://github.com/kozodoi/Text_Readability_Prediction">on GitHub</a>. </p>
  <img src="https://kozodoi.me/images/portfolio/gif_books.gif" alt="Notebook" style="width:100%">
  </span>
  <button class="btn" onclick="read_more(dots_id='dots1', mor_id='more1', btn_id='btn1')" id="btn1">&#128220; Read more</button>
  <button class="btn" onclick="window.open('https://github.com/kozodoi/Kaggle_Readability')" type="button">&#128187; GitHub repo</button>
  <button class="btn" onclick="window.open('https://kozodoi-text-readability-prediction-web-app-ddrfmw.streamlit.app')" type="button">&#128202; Web app</button>
  <button class="btn" onclick="window.open('https://kozodoi.me/blog/20211121/text-readability')" type="button">&#128203; Blog post</button>
</div>

<!----------------------------------------------------------------------------

<br>

<a id="PROJECT_3"></a>
<div class="card">
  <h2><b> Image-to-Text Translation of Molecules with Deep Learning </b></h2>
  <img src="https://kozodoi.me/images/portfolio/fig_inchi.jpg" alt="Notebook" style="width:100%">
  <h3> Highlights </h3>
  <ul>
  <li> built a CNN-LSTM encoder-decoder architecture to translate images into chemical formulas </li>
  <li> developed a comprehensive PyTorch GPU/TPU image captioning pipeline </li>
  <li> finished in the top-5% of the Kaggle competition leaderboard with a silver medal </li>
  </ul>
  <p> <b>Tags:</b> computer vision, natural language processing, deep learning </p>
  <span id="dots3"><p></p></span>
  <span id="more3">
  <h3> Summary </h3>
  <p>Organic chemists frequently draw molecular work using structural graph notations. As a result, decades of scanned publications and medical documents contain drawings not annotated with chemical formulas. Time-consuming manual work of experts is required to reliably convert such images into machine-readable formulas. Automated recognition of optical chemical structures could speed up research and development in the field.</p>
  <p>The goal of this project is to develop a deep learning based algorithm for chemical image captioning. In other words, the project aims at translating unlabeled chemical images into the text formula strings. To do that, I work with a large dataset of more than 4 million chemical images provided by Bristol-Myers Squibb.</p>
  <p>My solution is an ensemble of CNN-LSTM Encoder-Decoder models implemented in PyTorch.The solution reaches the test score of 1.31 Levenstein Distance and places in the top-5% of the competition leaderboard. The code is documented and published on <a href="https://github.com/kozodoi/BMS_Molecular_Translation">GitHub</a>.</p>
  </span>
  <button class="btn" onclick="read_more(dots_id='dots3', mor_id='more3', btn_id='btn3')" id="btn3">&#128220; Read more</button>
  <button class="btn" onclick="window.open('https://github.com/kozodoi/BMS_Molecular_Translation')" type="button">&#128187; GitHub repo</button>
  <button class="btn" onclick="window.open('https://www.kaggle.com/c/bms-molecular-translation/discussion/243845')" type="button">&#128214; Writeup on Kaggle</button>
</div>

<!----------------------------------------------------------------------------

<br>

<a id="PROJECT_2"></a>
<div class="card">
  <h2><b>Fair Machine Learning in Credit Scoring</b></h2>
  <img src="https://i.postimg.cc/j2Px4VLN/fig-pipeline.jpg" alt="Notebook" style="width:100%">
  <h3> Highlights </h3>
  <ul>
  <li> benchmarked eight fair ML algorithms on seven credit scoring data sets </li>
  <li> investigated profit-fairness trade-off to quantify the cost of fairness </li>
  <li> published a paper with the results at the European Journal of Operational Research </li>
  </ul>
  <p> <b>Tags:</b> tabular data, fairness, profit maximization </p>
  <span id="dots2"><p></p></span>
  <span id="more2">
  <h3> Summary </h3>
  <p> The rise of algorithmic decision-making has spawned much research on fair ML. In this project, I focus on fairness of credit scoring decisions and make three contributions: </p>
  <ul>
  <li> revisiting statistical fairness criteria and examining their adequacy for credit scoring </li>
  <li> cataloging algorithmic options for incorporating fairness goals in the ML model development pipeline </li>
  <li> empirically comparing different fairness algorithms in a profit-oriented credit scoring context using real-world data </li>
  </ul>
  <p>The code and documentation are available <a href="https://github.com/kozodoi/Fair_Credit_Scoring">on GitHub</a>. A detailed walkthrough and key results are published in <a href="https://arxiv.org/abs/2103.01907">this paper</a>.</p>
  <p>The study reveals that multiple fairness criteria can be approximately satisfied at once and recommends separation as a proper criterion for measuring scorecard fairness. It also finds fair in-processors to deliver a good profit-fairness balance and shows that algorithmic discrimination can be reduced to a reasonable level at a relatively low cost.</p>
  <img src="https://i.postimg.cc/5yB7y21M/fair-gif.gif" alt="Notebook" style="width:100%">
  </span>
  <button class="btn" onclick="read_more(dots_id='dots2', mor_id='more2', btn_id='btn2')" id="btn2">&#128220; Read more</button>
  <button class="btn" onclick="window.open('https://github.com/kozodoi/Fair_Credit_Scoring')" type="button">&#128187; GitHub repo</button>
  <button class="btn" onclick="window.open('https://arxiv.org/abs/2103.01907')" type="button">&#128213; Paper</button>
</div>

<!----------------------------------------------------------------------------

<hr style="height:10pt; visibility:hidden;" />

<h1> Further projects </h1>

Want to see more? Check out my further ML projects grouped by application areas below. You can also visit my <a href="https://github.com/kozodoi">GitHub page</a>, check my recent <a href="https://kozodoi.me">blog posts</a>, watch <a href="https://kozodoi.me/talks/">public tech talks</a> and read <a href="https://kozodoi.me/papers/">academic publications</a>.

<div>
  <button class="project_accordion">Generative AI</button>
  <div class="project_panel">

    <div class="card">
      <h3>Medical Content Generation with LLMs</h3>
      <img src="https://kozodoi.me/images/portfolio/fig_content.png" alt="Notebook" style="width:100%">
      <p><ul>
      <li> developed LLM-powered end-to-end content generation solution on AWS </li>
      <li> the system provides generation, revision, and fact-checking capabilities </li>
      <li> implemented an interactive web app and backend as infrastructure-as-code </li>
      </ul></p>
      <button class="btn" onclick="window.open('https://aws.amazon.com/blogs/machine-learning/medical-content-creation-in-the-age-of-generative-ai/')" type="button">&#128203; Blog post</button>
    </div>

    <br>

    <div class="card">
      <h3>Improving RAG with User Interaction Tool</h3>
      <img src="https://kozodoi.me/images/portfolio/fig_rag.png" alt="Notebook" style="width:100%">
      <p><ul>
      <li> integrated a human feedback tool into a RAG agent </li>
      <li> published a blog post and the code of the solution </li>
      </ul></p>
      <button class="btn" onclick="window.open('https://github.com/aws-samples/rag-with-human-support')" type="button">&#128187; GitHub repo</button>
      <button class="btn" onclick="window.open('https://aws.amazon.com/blogs/machine-learning/improve-llm-responses-in-rag-use-cases-by-interacting-with-the-user/')" type="button">&#128203; Blog post</button>
    </div>

  </div>
</div>

<!----------------------------------------------------------------------------

<div>
  <button class="project_accordion">Computer Vision</button>
  <div class="project_panel">
    <div class="card">
      <h3>Pet Popularity Prediction</h3>
      <img src="https://i.postimg.cc/43yC8KyY/header.png" alt="Notebook" style="width:100%">
      <p><ul>
      <li> built a PyTorch pipeline for predicting pet cuteness from image and tabular data </li>
      <li> reached top-4% in the Kaggle competition using Transformers and CNNs </li>
      <li> implemented an interactive web app for estimating cuteness of custom pet photos </li>
      </ul></p>
      <button class="btn" onclick="window.open('https://github.com/kozodoi/Pet_Pawpularity')" type="button">&#128187; GitHub repo</button>
      <button class="btn" onclick="window.open('https://kozodoi-pet-pawpularity-web-app-kvzxqr.streamlit.app')" type="button">&#128202; Web app</button>
    </div>
    
    <br>

    <div class="card">
      <h3>Cassava Leaf Disease Classification</h3>
      <img src="https://i.postimg.cc/jdtWjXyF/cassava-sample.png" alt="Notebook" style="width:100%">
      <p><ul>
      <li> built CNNs and Vision Transformers in PyTorch to classify plant diseases </li>
      <li> constructed a stacking ensemble with multiple computer vision models </li>
      <li> finished in the top-1% of the Kaggle competition with a gold medal </li>
      </ul></p>
      <button class="btn" onclick="window.open('https://github.com/kozodoi/Kaggle_Leaf_Disease_Classification')" type="button">&#128187; GitHub repo</button>
      <button class="btn" onclick="window.open('https://www.kaggle.com/c/cassava-leaf-disease-classification/discussion/220751')" type="button">&#128214; Writeup on Kaggle</button>
    </div>

    <br>

    <div class="card">
      <h3>Catheter and Tube Position Detection on Chest X-Rays</h3>
      <img src="https://i.postimg.cc/tT6b3KGN/xray-sample.png" alt="Notebook" style="width:100%">
      <p><ul>
      <li> built deep learning models to detect catheter and tube position on X-ray images </li>
      <li> developed a comprehensive PyTorch GPU/TPU computer vision pipeline </li>
      <li> finished in the top-5% of the Kaggle competition leaderboard with silver medal </li>
      </ul></p>
      <button class="btn" onclick="window.open('https://github.com/kozodoi/Kaggle_RANZCR_Challenge')" type="button">&#128187; GitHub repo</button>
      <button class="btn" onclick="window.open('https://www.kaggle.com/c/ranzcr-clip-catheter-line-classification/discussion/226664')" type="button">&#128214; Writeup on Kaggle</button>
    </div>

    <br>

    <div class="card">
      <h3>Detecting Blindness on Retina Photos</h3>
      <img src="https://i.postimg.cc/dVjwCDr2/blindness.png" alt="Notebook" style="width:100%">
      <p><ul>
      <li> developed CNN models to identify disease types from retina photos </li>
      <li> written a detailed report covering problem statement, EDA and modeling </li>
      <li> submitted as a capstone project within the Udacity ML Engineer program </li>
      </ul></p>

      <button class="btn" onclick="window.open('https://github.com/kozodoi/Udacity_Blindness_Detection')" type="button">&#128187; GitHub repo</button>
      <button class="btn" onclick="window.open('https://kozodoi.me/blog/20200711/blindness-detection')" type="button">&#128203; Blog post</button>
      <button class="btn" onclick="window.open('https://github.com/kozodoi/Udacity_Blindness_Detection/raw/master/report.pdf')" type="button">&#128214; Detailed report</button>
    </div>

  </div>
</div>

<!----------------------------------------------------------------------------

<div>
  <button class="project_accordion">Tabular Data and Graph ML</button>
  <div class="project_panel">

    <div class="card">
      <h3>Probabilistic Demand Forecasting with Graph Neural Networks</h3>
      <img src="https://kozodoi.me/images/portfolio/fig_gnn.jpg" alt="Notebook" style="width:100%">
      <p><ul>
      <li> developed a novel probabilistic demand forecasting architecture combining GNNs and DeepAR </li>
      <li> proposed article similarity based data-driven similarity matrix construction </li>
      <li> published a paper demonstrating monetary and accuracy gains from the proposed model </li>
      </ul></p>
      <button class="btn" onclick="window.open('https://www.amazon.science/publications/probabilistic-demand-forecasting-with-graph-neural-networks')" type="button">&#128213; Paper</button>
      <button class="btn" onclick="window.open('https://kozodoi.me/talks/ECML_2023.pdf')" type="button">&#128202; Slides</button>
    </div>

    <div class="card">
      <h3>Profit-Driven Demand Forecasting with Gradient Boosting</h3>
      <img src="https://kozodoi.me/images/portfolio/fig_custom_loss.png" alt="Notebook" style="width:100%">
      <p><ul>
      <li> developed a two-stage demand forecasting pipeline with LightGBM models </li>
      <li> performed a thorough cleaning, aggregation and feature engineering on transactional data </li>
      <li> implemented custom loss functions aimed at maximizing the retailer's profit </li>
      </ul></p>
      <button class="btn" onclick="window.open('https://github.com/kozodoi/DMC_2020')" type="button">&#128187; GitHub repo</button>
      <button class="btn" onclick="window.open('https://kozodoi.me/blog/20200727/demand-forecasting')" type="button">&#128203; Blog post</button>
    </div>

    <br>

    <div class="card">
      <h3>Google Analytics Customer Revenue Prediction</h3>
      <img src="https://i.postimg.cc/MTZpw33J/google-importance.png" alt="Notebook" style="width:100%">
      <p><ul>
      <li> worked with two-year transactional data from a Google merchandise store </li>
      <li> developed LightGBM models to predict future revenues generated by customers </li>
      <li> finished in the top-2% of the Kaggle competition leaderboard with silver medal </li>
      </ul></p>
      <button class="btn" onclick="window.open('https://github.com/kozodoi/Kaggle_Google_Analytics')" type="button">&#128187; GitHub repo</button>

    </div>
  </div>
</div>

<!----------------------------------------------------------------------------

<div>
  <button class="project_accordion">Software Packages</button>
  <div class="project_panel">

    <div class="card">
      <h2> <code>fairness</code>: Package for Computing Fair ML Metrics </h2>
      <img src="https://kozodoi.me/images/portfolio/fig_fairness.png" alt="Notebook" style="width:100%">
      <p><ul>
      <li> developing and actively maintaining an R package for fair machine learning </li>
      <li> the package offers calculation, visualization and comparison of algorithmic fairness metrics </li>
      <li> the package is published on CRAN and has more than 16k total downloads </li>
      </ul></p>
      <button class="btn" onclick="window.open('https://github.com/kozodoi/fairness')" type="button">&#128187; GitHub repo</button>
      <button class="btn" onclick="window.open('https://kozodoi.me/blog/20200501/fairness-tutorial')" type="button">&#128203; Blog post</button>
    </div>

    <br>

    <div class="card">
      <h2><b> <code>dptools</code>: Package for Data Processing and Feature Engineering </b></h2>
      <img src="https://i.postimg.cc/0yVqMHfM/data-cover.jpg" alt="Notebook" style="width:100%">
      <p><ul>
      <li> Python package with helper functions to simplify common data processing tasks </li>
      <li> functions cover feature engineering, data aggregation, working with missings and more </li>
      <li> the source code and documentation are available on <a href="https://github.com/kozodoi/dptools">GitHub</a> and <a href="https://pypi.org/project/dptools/">PyPi</a> </li>
      </ul></p>
      <button class="btn" onclick="window.open('https://github.com/kozodoi/dptools')" type="button">&#128187; GitHub</button>
    </div>

  </div>
</div>

<!----------------------------------------------------------------------------

<script>
var acc = document.getElementsByClassName("project_accordion");
var i;

for (i = 0; i < acc.length; i++) {
  acc[i].addEventListener("click", function() {
    this.classList.toggle("project_active");
    var project_panel = this.nextElementSibling;
    if (project_panel.style.maxHeight) {
      project_panel.style.maxHeight = null;
    } else {
      project_panel.style.maxHeight = project_panel.scrollHeight + "px";
    }
  });
}
</script>
-->
