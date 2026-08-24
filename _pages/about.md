---
permalink: /
excerpt: "Ph.D. candidate at the Indian Institute of Science, Bangalore, working on trustworthy machine learning: machine unlearning, data attribution, differential privacy, and uncertainty quantification."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  a:link    { color: RoyalBlue; background-color: transparent; text-decoration: none; }
  a:visited { color: Purple;    background-color: transparent; text-decoration: none; }
  a:hover   { color: RoyalBlue; background-color: transparent; text-decoration: underline; }
  a:active  { color: DarkRed;   background-color: transparent; text-decoration: underline; }
</style>

<p align="justify">Hi, thanks for your interest!</p>

<p align="justify">I am a final year Ph.D. student at the Representation Learning Lab, <a href="https://ece.iisc.ac.in/">Department of Electrical Communication Engineering</a>, <a href="https://iisc.ac.in/">Indian Institute of Science (IISc)</a>, Bangalore, advised by <a href="https://sites.google.com/view/prathosh/home">Prof. Prathosh A. P.</a> Over the course of my doctoral research I have been fortunate to be mentored by <a href="http://theertha.info/">Dr. Ananda Theertha Suresh</a>, <a href="https://spkreddy.org/">Prof. Sai Praneeth Karimireddy</a>, <a href="https://sites.google.com/view/shubhada-agrawal/home">Prof. Shubhada Agrawal</a>, and <a href="https://debabrota-basu.github.io/">Prof. Debabrota Basu</a>. Before commencing my doctoral studies, I completed my post-graduate studies in Statistics at the <a href="https://www.isichennai.res.in/">Indian Statistical Institute (ISI)</a>, Chennai, under the supervision of <a href="https://www.isichennai.res.in/~skkattu">Prof. Sudheesh Kumar K.</a>, and my undergraduate studies in ECE at the <a href="https://www.iiests.ac.in/">Indian Institute of Engineering Science and Technology (IIEST)</a>, Shibpur.</p>

<p align="justify">I have also gained research experience in industry. Most recently I was a Ph.D. research intern at <a href="https://research.adobe.com/careers/bangalore/">Adobe Research</a>, Bangalore, working on data attribution for vision-language models. Before that I spent a brief but enriching period as a Research Associate at <a href="https://www.oneirix.com/">Oneirix Labs</a>, developing algorithms grounded in <i>applied mathematics</i> and <i>computational statistics</i>, with a particular emphasis on Medical AI. During my undergraduate studies I was a research intern at the <i>Laboratory for Electro-Optics Systems (LEOS)</i>, <a href="https://www.isro.gov.in/LEOS.html">Indian Space Research Organisation</a>.</p>

<font color="SteelBlue">Research Focus:</font> Trustworthy Machine Learning &mdash; understanding and controlling the contribution of individual data points to a learned model
<br />
<font color="SteelBlue">Main Research Area:</font> Privacy- and uncertainty-aware learning algorithms: <a href="https://ojs.aaai.org/index.php/AAAI/article/view/32682">Machine Unlearning</a>, <a href="https://arxiv.org/pdf/2510.10510">Influence Estimation (Data Attribution)</a>, and <a href="https://en.wikipedia.org/wiki/Differential_privacy">Differential Privacy</a>
<br />

<p align="justify" style="margin-bottom: 0;"><font color="SteelBlue">Related Research Areas:</font> <a href="https://arxiv.org/pdf/2510.04058">Diffusion Models</a>, <a href="https://arxiv.org/pdf/2604.14876">fragility of Bandit Algorithms</a>, Conformal Prediction, Calibration, Statistical Optimal Transport, Learning Theory, and Information Theory.</p>

<br />

<details>
<summary><span style="color:SteelBlue;"><font color="SteelBlue">Brief Research Summary</font></span></summary>
<span class="abstract-text" style="font-size:1em; color:Black; text-align: justify">
<p align="justify">My broader research interest lies in <b>Trustworthy Machine Learning</b>. My thesis centres on a single question: what is the contribution of an individual training point to what a model has learned, and how can that contribution be measured and, when necessary, removed? I approach this from two complementary directions. <a href="https://en.wikipedia.org/wiki/Differential_privacy">Differential Privacy</a> offers a powerful theoretical lens on the question, giving formal limits on how much any one data point can influence a trained model. <a href="https://arxiv.org/pdf/2510.10510">Influence Estimation (Data Attribution)</a> and <a href="https://ojs.aaai.org/index.php/AAAI/article/view/32682">Machine Unlearning</a> provide the practical tools: the former to <i>estimate</i> the effect of specific data, the latter to <i>undo</i> it in pre-trained classifiers, GANs, and diffusion models without retraining from scratch.
<br /><br />
Alongside this, I work on uncertainty quantification &mdash; conformal prediction and calibration &mdash; as the natural counterpart to privacy: both are statements about what a model does <i>not</i> know. I am also interested in the fragility of optimal <a href="https://arxiv.org/pdf/2604.14876">bandit algorithms</a>, where policies that are optimal in expectation can nevertheless incur heavy-tailed regret, and in <i>Statistical Optimal Transport</i> as a tool for comparing learned distributions. My work draws on statistics, learning theory, and information theory throughout. Please feel free to reach out if you would like to discuss any of these topics!</p>
</span>
</details>

<br />

<a href="#selected_publications">[Selected Papers]</a> &nbsp; <a href="/publications/">[Full List]</a> &nbsp; <a href="https://scholar.google.co.in/citations?hl=en&amp;user=gYUOZNQAAAAJ" target="_blank">[Google Scholar]</a> &nbsp; <a href="https://arxiv.org/search/?searchtype=author&amp;query=Subhodip+Panda" target="_blank">[arXiv]</a> &nbsp; <a href="/files/CV_subhodip_updated.pdf" target="_blank">[CV]</a>

<br /><br />

<p align="justify" style="margin-bottom: -15px;"><font color="SteelBlue"><b>Open to Opportunities:</b></font> I will be completing my Ph.D. degree this year and am currently seeking <b>full-time research positions</b>. My <a href="/files/CV_subhodip_updated.pdf" target="_blank">CV</a> is available here &mdash; please do reach out if you have a relevant opening, or simply if our research interests align and you would like to collaborate.</p>

<h2 style="color:SteelBlue;"><a id="selected_publications">Selected Papers:</a></h2>

<ul style="margin:1;padding:1">

<li><b>Regret Tail Characterization of Optimal Bandit Algorithms with Generic Rewards.</b> <a href="https://arxiv.org/pdf/2604.14876" target="_blank">[arXiv version]</a>
<br />
Subhodip Panda, Shubhada Agrawal
<br />
IEEE International Symposium on Information Theory, ISIT 2026</li>

<li><b>f-INE: A Hypothesis Testing Framework for Estimating Influence under Training Randomness.</b> <a href="https://arxiv.org/abs/2510.10510" target="_blank">[arXiv version]</a>
<br />
Subhodip Panda, Dhruv Tarsadiya, Shashwat Sourav, Prathosh A. P., Sai Praneeth Karimireddy
<br />
International Conference on Learning Representations, ICLR 2026</li>

<li><b>Concept Forgetting via Label Annealing.</b> <a href="https://openreview.net/pdf?id=2L7KQ4qbHi" target="_blank">[Paper]</a>
<br />
Subhodip Panda, Ananda Theertha Suresh, Atri Guha, Prathosh A. P.
<br />
Conference on Uncertainty in Artificial Intelligence, UAI 2025</li>

<li><b>Adapt then Unlearn: Exploiting Parameter Space Semantics for Unlearning in Generative Adversarial Networks.</b> <a href="https://arxiv.org/abs/2309.14054" target="_blank">[arXiv version]</a>
<br />
Piyush Tiwary, Atri Guha, Subhodip Panda, Prathosh A. P.
<br />
Transactions on Machine Learning Research, TMLR 2025</li>

<li><b>Partially Blinded Unlearning: Class Unlearning for Deep Networks a Bayesian Perspective.</b> <a href="https://ojs.aaai.org/index.php/AAAI/article/view/32682" target="_blank">[Paper]</a>
<br />
Subhodip Panda, Shashwat Sourav, Prathosh A. P.
<br />
AAAI Conference on Artificial Intelligence, AAAI 2025</li>

<li><b>FAST: Feature Aware Similarity Thresholding for Weak Unlearning in Black-Box Generative Models.</b> <a href="https://ieeexplore.ieee.org/abstract/document/10754629" target="_blank">[Paper]</a>
<br />
Subhodip Panda, Prathosh A. P.
<br />
IEEE Transactions on Artificial Intelligence, TAI 2024</li>

<li><b>Unlearning in Diffusion Models under Data Constraints: A Variational Inference Approach.</b> <a href="https://arxiv.org/pdf/2510.04058" target="_blank">[arXiv version]</a>
<br />
Subhodip Panda, Varun M. S., Shreyans Jain, Sarthak Maharana, Prathosh A. P.
<br />
NeurIPS 2024 Workshop on SafeGenAI</li>

</ul>

<hr style="color:black;" />
