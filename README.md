# ScAA-Dataset

## License
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />ASER Dataset</span>  is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.


## About Pratham
Pratham was founded in 1995, to provide pre-school education to children in Mumbai slums. Over the last 20 years Pratham has grown to be India’s largest NGO working to provide quality education to underprivileged youth and 
children in over 21 states and union territories across the country, with a range of interventions. Pratham is a widely recognized organization, having received notable awards such as the WISE Prize for Innovation, 
Skoll Award for Social Entrepreneurship, the Henry R Kravis Prize in Leadership and the CNN-IBN Indian of the Year for Public Service. More info at: http://pratham.org/


## About ScAA Dataset
Automatic short answer grading (ASAG) techniques are designed to automatically assess short answers written in natural language. Apart from MCQs, evaluating free text answer is essential to assess the knowledge and understanding of children in the subject. But assessing descriptive answers in low resource languages in a linguistically diverse country like India poses significant hurdles. To solve this assessment problem and advance NLP research in regional Indian languages, we curated the Science Answer Assessment (ScAA) dataset of children’s answers in the age group of 8-14. This question answer dataset contains 10,988 and 1,955 pairs of natural answers along with model answers for Hindi and Marathi respectively for 32 questions.
The goal of this work is to make this dataset public to spur innovation and generate novel solutions for automation of short answer grading in Indian Languages.

Below we explain the Data Collection method, Statistics and Sample (model answer, user answer) set.

### Data Collection and Statistics

We curate Science Answer Assessment (ScAA) dataset in Hindi and Marathi language comprising of 8 science topics with 4 questions per topic, i.e. a total of 32 parallel question-model answer pairs in Hindi and Marathi. The dataset is created via three stages: Question and model answer curation, User answer collection, User answer evaluation. 

Examples of the questions and model answers
<table>
  <tr>
  <th>Topic</th>
  <th>Sample Question</th>
  <th>Model Answer</th>
  </tr>
  <tr>
    <td>Circulatory System</td>
    <td>प्लेटलेट की संख्या कम हो जाने से क्या होगा?</td>
    <td>जख्म होने पर थक्के ना ज़मने के कारण बहाव ज्यादा होगा</td>
  </tr>
  <tr>
    <td>Eye and Vision</td>
    <td>आंखों में धूल चली जाने पर आंसू क्यों आ जाते हैं?</td>
    <td>धूल के कण आंसुओं के साथ बाहर निकल आते है ताकि आंखों को हानि न पंहुचे</td>
  </tr>
  </table>

### Question and model answer curation
The questions were selected from Grade 8 level Science topics: Adaptation, Circulatory System, Eye and Vision, Heat, Simple Machine, Skeletal System, Sound, Water Chemistry.  The users here are children in the age group of 8-14 years from 3 states of India: Uttar Pradesh, Rajasthan and Maharashtra.

### User answer collection
The data is crowdsourced via an Android app developed by Pratham to enable children to take assessments anytime they want.  This Android Assessment App is available on play store at https://play.google.com/store/apps/details?id=com.pratham.assessment&hl=en_IN&gl=US 

Though there are various types of questions in one assessment, we focus on free text answer in this work. To answer an open-ended question, children could either type the answer directly using the phone keyboard or use Speech-to-Text (STT) service  and then edit it. 
     Over a period of 8 months, the app helped collect ~50,000 answers from 11,476 children to 32 science questions from 3 states of India.

### User answer evaluation
 The ScAA dataset was created by selecting a subset of these collected answers and getting each answer evaluated as correct or incorrect by two human annotators. The Cohen’s Kappa κ score indicating level of agreement between two annotators was 0.75. ScAA consists of answers where both human evaluators matched in their markings. The answers marked as 1 are correct and those marked as 2 are incorrect. 
 
Detailed statistics are listed below:

<table>
  <tr>
  <th></th>
  <th>Hindi</th>
  <th>Marathi</th>
  </tr>
  <tr>
    <td>Total Questions	</td>
    <td>32</td>
    <td>32</td>
   </tr>
    <tr>
    <td>Total Answers</td>
    <td>10988</td>
    <td>1955</td>
   </tr>
   <tr>
    <td>Total Unique Answers</td>
    <td>7205</td>
    <td>1435</td>
   </tr>
    <tr>
    <td>Total Correct Answers</td>
    <td>3843</td>
    <td>488</td>
   </tr>
   <tr>
    <td>Average # unique correct answers per question	</td>
    <td>41</td>
    <td>7</td>
   </tr>
    <tr>
    <td>Average answer length (in words)</td>
    <td>15</td>
    <td>15</td>
   </tr>
</table>

  ## Examples of different varieties of correct answers for the same question
  <table>
  <tr>
    <th>Question in Hindi</th>
    <th>Question in Marathi</th>
    <th> Correct user answers in Hindi</th>
    <th> Correct user answers in Marathi</th>
  </tr>
  <tr>
    <td rowspan=3>एक वयस्क मनुष्य के कंकाल का वजन लगभग कितना होता है?</td><td rowspan=3>एका प्रौढ व्यक्तीच्या सांगाड्याचे वजन अंदाजे किती असते? </td>
  <tr><td>एक वेस्ट मनुष्य के कंकाल का वजन लगभग 10 किलोग्राम होता है</td><td>10 किग्रॅ</td></tr>
  <tr><td>१० किग्रा</td><td>दहा किलो ग्रॅम</td></tr>
	<tr>  <td rowspan=6>	चाँद पर कोई किसी की आवाज क्यों नहीं सुन सकते?</td><td rowspan=6>अंतराळवीर चंद्रावर एकमेकांचे आवाज का ऐकू शकत नाहीत?</td><td>वायुमंडल नहीं है</td><td>वातावरण नसते</td>
	</tr>
  <tr><td>	क्योंकि वहां पर वायु नहीं है</td><td>तिथे हवा नाही</td></tr>
	<tr><td>	वायु मंडल का अनुपस्थिती के कारण</td><td>कारण तिथे हवा नाही</td></tr>
  </table>
  
  
