---
layout: default
---

# Rules

## Protocol

<p style='text-align: justify;'>
We will consider using and will conduct beta testing of fully fledged platforms such as Codalab or Huawei Cloud Competition for hosting the competition. Alternatively, we may use online forms on the website for registration and submissions. Participants will follow the outlined steps to register for the competition:

* <p style='text-align: justify;'>The participants register on the website by entering their team name, email address, and affiliations using a form. Then, they receive an ID code to identify their submissions. 
* <p style='text-align: justify;'>During registration process, the participant is asked to agree to abide by the rules of the competition.
* <p style='text-align: justify;'>The participant can download the starter kit and the dataset from given repository and download links and follow the Tutorial notebook to learn about the dataset format, data
readers, evaluation protocol and the details of the baseline models.
<p style='text-align: justify;'>
  
Registered participants will need to include the following in their submission:
  
* <p style='text-align: justify;'>Same ID code given after registration to identify their multiple submissions
* <p style='text-align: justify;'>A Poetry configuration to manage the participant’s Python library dependencies in a deter-ministic way. We will give a template and tutorial to participants.
* <p style='text-align: justify;'>A brief description of their method will required for the winning submissions.
<p style='text-align: justify;'>
Please note that the above submission process might slightly change if we can test and successfully adopt of competition platform.
<p style='text-align: justify;'>
Tsssso prevent cheating, we will keep the test set confidential before, during and after the competition is finished. We will also review every potentially winning submission to check for cheating.

## Evaluation

The evaluation process in our competition will include two stages.

<p style='text-align: justify;'> <b>The first stage:</b> the submitted models will be evaluated on a diverse subset of the OpenCompass benchmark, including CSQA, BIG-Bench Hard, GSM8K, LongBench, HumanEval, TruthfulQA, CHID, along with a set of secret holdout tasks to avoid overfitting. A self-contained code base will be provided to facilitate participants in easily evaluating their models on seven diverse tasks via the OpenCompass benchmark. </p>

* <p style='text-align: justify;'> Each submission will be ranked individually for each task, with the top 10 submissions with the highest score per task receiving scores from 10 to 1. The score of each task is calculated as the average score of the three models for the first track. For the second track, the score is the score of the submitted model. </p>

* <p style='text-align: justify;'> We will measure the models' throughput on a smartphone platform provided by the sponsor. Submissions will be ranked based on throughput. To emphasize the importance of inference speed, the score for the throughput task will be <b>doubled</b>, ranging from 20 to 2 for the top 10 submissions. To assist participants in improving the speed of their models, we will provide an easy-to-run pipeline to measure throughput on a GPU, where the throughput values are roughly scaled to those on the smartphone platform.</p>

* <p style='text-align: justify;'> We will measure the inference memory usage of all models. Submissions with models that exceed 12GB of memory usage for inference will be disqualified.</p>

* <p style='text-align: justify;'> The final rank of submissions will be determined by the sum of scores across all evaluation tasks including seven diverse tasks as shown in the Table below (100 scores in total), maximum 70 scores, one secret holdout task (maximum 10 scores), and the throughput measurement (maximum 20 scores). </p>

<p style='text-align: justify;'> The top 15 teams with the highest scores will be displayed on the leaderboard. Participants are required to submit their source codes, evaluation log files, and models to the organizers (Check <i>Submission</i> section for details). </p>

<p style='text-align: justify;'>Participating teams are encouraged to submit their models for a preliminary review on the 25th of August to identify potential bugs and format issues, ensuring that the final submissions are in the correct format. Each team can make three submissions to each track after the deadline of the preliminary review. The best-performing model will be used to rank the team on the leaderboard and selected for the final model evaluation.</p>

<p style='text-align: justify;'> <b>The second stage:</b>  After the competition is closed on October 25th, 2024, we will contact the top 3 teams with the highest scores in both tracks, requesting that they submit all necessary code and data to reproduce their results. We will then replicate their entire process, to ensure it is fully repeatable and the final model can be run on a smartphone with 12 GB RAM with the same results. If the top-scoring model cannot be reproduced under these imposed conditions or can not fit the smartphone, we will move on to consider the next highest-scoring submission in the category, until a reproducible and high-performing submission is selected. </p>

<p style='text-align: justify;'> Our evaluation will leverage an extensive array of rigorously curated datasets across multiple fundamental dimensions: language comprehension, knowledge precision, logical deduction, mathematical problem-solving, programming proficiency, extended text analysis, and intelligent agent engagement. Details of the evaluation tasks we chose are shown below: </p>

