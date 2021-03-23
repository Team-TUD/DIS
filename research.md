---
layout: page
title: Research
---
{::options parse_block_html="true" /}
<a name="top"></a> 


Our research themes span in the following areas. 

- [Robust, private, fair learning](#RPFlearning)
- [Edge federated learning and inference](#eLInf)
- [Resourcement managment for deep neural networks clusters](#resource)


# Robust, Private, Fair Learning<a name="RPFlearning"></a> 

Artificial intelligence (AI) and machine learning (ML) are ubiquitous in our daily lives in the form of search engines, machine translation, self-driving cars and much more. The prevailing assumptions of existing ML algorithms are that data is neutral and can be freely accessed (without breaching privacy). As a result, the existing algorithms fall short of addressing challenges in realistic scenarios, i.e., against adversarial examples, dirty data, and unreliable execution environments while still preserving data privacy. These issues are further exacerbated by large and distributed learning problems, the data for which is collected over multiple sources and must be computed on distributed nodes.

In this line of research, we are designing robust, privacy-preserving and fair learning algorithms. Topics include:
- [Robust and Adversarial Machine Learning](#Robust): designing learning algorithms that are robust to dirty data inputs.
- [Synthetic Data Generation](#GAN): using Generateive Adversarial Networks to synthesize tabular data. 
- [Fair Information Maximization on Social Media](#FairIM) designing learning algorithms that can be debiased, for example in terms of gender or race, via data selection and objective modification of learning algorithms.
-	Adversarial learning: designing adversarial attacks and defense mechanisms for deep models.
-	Differential private (deep) learning: designing effective differential private ML models with precise accuracy accounting.

<figure>
 <a href="#top">
  <img src="../images/up.png" alt="top" style="float: right;" width="30" height="22">
 </a>
</figure>

# Edge federated learning and Inference<a name="eLInf"></a> 
Data is constantly generated and collected by edge devices (of the network) to power up today’s AI and ML analyses. With the advancement of algorithmic compression techniques and hardware technology, the ability to train neural networks and run inference on edge devices has gone from myth to reality. Federated learning (FL) is an emerging learning paradigm where distributed edge nodes collaboratively learn the weights of neural networks iteratively without directly sharing data. It is largely unexplored how existing deep learning algorithms can be realized within a FL framework, thereby overcoming network communications and adversarial threats. Moreover, owing to the vast number of available trained models and highly heterogeneous mobile devices, it is no mean feat to identify and deploy the right model for individual edge devices.

In this line of research, we are designing learning algorithms and prototyping system solutions for ML training and inference on distributed edge devices. Topics include:
- [Federated Learning Systems](#Federated): designing efficient communication protocols and incentive mechanisms for edge learners.
- [Deep Model Inferences on Edge Devices](#EdgeInf): designing and prototyping an inference engine that can search for optimal models and configurations for edge devices at scale.
-	Secure edge learning and inference: developing prototypes to leverage trusted execution environments and differential privacy for securing edge devices from adversaries. 

<figure>
 <a href="#top">
  <img src="../images/up.png" alt="top" style="float: right;" width="30" height="22">
 </a>
</figure>





# System and Data Management for Deep Clusters<a name="resource"></a> 
There is a surging number of deep training/inference jobs, e.g., convolutionary networks to classify images, and the Bert language model to classify text running on cloud datacenters. Such learning jobs form a unique class of workloads that have a large number of tuning parameters and repetitive computation routines in iterations, and they rely on the acceleration of specialized computing units such as GPU. The resulting computational time and energy computation can be daunting. This raises questions about how to design resource management policies for such clusters such that running deep network training/inference jobs is truly accessible, sustainable, and affordable for the public. 

In this line of research, we are seeking novel resource management solutions for such deep neural network clusters ranging from building a systematic understanding of workloads to developing specific scheduling policies to minimize their resource dependency without sacrificing metrics of interest, such as accuracy, at the job level. Topics include:
-	[Hyperparameter and system tuning](#Tune): jointly tuning network hyperparameters, mini-batch sizes, and system parameters such as parallel threads.
- [Tucker Tensor Decomposition](#Tucker): learning the lower-rank representation of data inputs to accelereate the computation efficiency.
-	Workload characterization: mapping the resource demands of computation routines and identifying resource bottlenecks for different classes of neural networks.
-	SlimML: exploring different data subsampling strategies to search for an optimal tradeoff between learning accuracy and resource efficiency.

<figure>
 <a href="#top">
  <img src="../images/up.png" alt="top" style="float: right;" width="30" height="22">
 </a>
</figure>



## Robust and Adversarial Machine Learning<a name="Robust"></a> 

**Research questions**: Can today's deep neural networks handle noisy data sets, namely corrupted inputs and labels? How to design novel learning algorithms to dstill the data quality and enhance the robustness of learning models when encountering noisy and adversarial input? 

{: .box-note}
We are working on noise resilient learning frameworks, leveraging adversarial examples, expert judgement, and robust loss functions.


<figure>
 <a href="#top">
  <img src="../images/up.png" alt="top" style="float: right;" width="30" height="22">
 </a>
</figure>

<br>


## Optimization for Machine Learning Services and Clusters<a name="Tune"></a> 
-----
**Research questions**: Training deep models consumes tremendous computing time and resources; however tuning the hyperparameter of deep models is even multiple fold higher. Can one design efficient and accurate tuning framework for deep neural networks such that the optimal parameters can be found at minimum computational resources?

{: .box-note}
We are working on accelerating processing strategies that only execute critical data and leverage the workload similarities when tuning hyperparameters and training a wide range of ML models.  


<figure>
 <a href="#top">
  <img src="../images/up.png" alt="top" style="float: right;" width="30" height="22">
 </a>
</figure>

<br>

## Deep Model Inferences on Edge Devices<a name="EdgeInf"></a> 
----
**Research questions**: How to choose suitable trained models from the plethoral of existing ones and deploy at the edge devices? How to optimize the performance of deep models on the edge devices? Can today's edge devices efficiently execute multiple DNNs at the same time, e,.g., extracting information of people, aged and gender from images?

{: .box-note}
We are working on various scheduling and model selection algorithms to adaptively run multiple DNNs on resource limited edge devices, in fulfilling various users’ requirements. 
 

<figure>
 <a href="#top">
  <img src="../images/up.png" alt="top" style="float: right;" width="30" height="22">
 </a>
</figure>

<br>

## Synthetic Data Generator<a name="GAN"></a> 
-----
**Research questions**: While big data is powering up the deep learning models, it is costly and inevitably intrudes privacy to curate such data. Synthetically generated data not only alleviates the cost of collecting data but also overcome the privacy concerns and legislation boundary. How to generate synthetic data that fulfilll the requirements of data similarity, analysis utility, privacy and generalization?

{: .box-note}
We are working on various synthetic generation methods for table and image data, e.g., generative adversarial networks. We are in collaboration with companies in the finance sector. 


<figure>
 <a href="#top">
  <img src="../images/up.png" alt="top" style="float: right;" width="30" height="22">
 </a>
</figure>

<br>


## Federated Learning Systems: Incentive and Backdoor<a name="Federated"></a> 
-----
**Research questions**: Federated learning framework preserves privacy by design as user data stays on devices. How to provide the incentives for users at the federated learning systems? How to value the contributed models from other users? Can we trust the models provided by other users?

{: .box-note}
We are designing incentive mechanisms and defense strategies against backdoor attacks for the federated learning systems, from Bayesian models to deep neuralnetworks.


<figure>
 <a href="#top">
  <img src="../images/up.png" alt="top" style="float: right;" width="30" height="22">
 </a>
</figure>

<br>

## Sparse Tucker Decomposition <a name="Tucker"></a> 
-----
**Research questions**: Sparse Tucker decomposition (sTD) is widely used in low-rank representation learning for sparse big data analysis. Due to the entanglement problem  of  core  tensor  and  factor  matrices,  the  computational process  for  STD  faces  the challenge of   intermediate  variables  explosion. How to design an efficient optimization algorithm for STD without degrading approximation accuracy?

{: .box-note}
We are working on various optimization techniques to accelerate the sparse matrix factorization, particularly for tucker tensor decomposition.


<figure>
 <a href="#top">
  <img src="../images/up.png" alt="top" style="float: right;" width="30" height="22">
 </a>
</figure>

<br>

## Fair Information Maximization on Social Media<a name="FairIM"></a> 
-----
**Research questions**: Users on social media with high visibility are often selected as seeds to spread information and affect their adoption in target groups. Even though female users are more active on social media than male users, males are regarded as influential in various centrality measures.

{: .box-note}
We are trying to answer how gender differences and similarities can impact the information spreading process on social media. We are developing  disparity-aware seeding algorithms.


<figure>
 <a href="#top">
  <img src="../images/up.png" alt="top" style="float: right;" width="30" height="22">
 </a>
</figure>

<br>


