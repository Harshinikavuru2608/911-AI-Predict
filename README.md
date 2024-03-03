# 911 AI Predict
## The 911 Artificial Intelligence Platform for Recognition of Emergencies through DIrected ClassificaTion
## Abstract
Modern technology is transforming emergency response processes with the 911 Artificial Intelligence (AI) Platform for Recognition of Emergencies through Directed Classification (911-AI-PREDICT) system.
By utilizing the capabilities of real-time AI-driven decision assistance, this system seeks to enhance the early and accurate detection of life-threatening medical situations reported through 911 calls. 
A real-time transcriber and a real-time classifier make up the system, which works in tandem to extract crucial information from emergency calls and identify potentially fatal conditions. 
The 911-AI-PREDICT system enables the quick and correct allocation of resources to emergency scenarios, providing speedy and efficient emergency medical services (EMS) care. 
It does this by merging AI components with existing emergency dispatch systems. Transcription models, data connecting models, and ML classification models are all used in the system's implementation. 
Future work will involve expanding call-relevant features, enabling data linkage for non-standard locations, fine-tuning the model, creating the whole end-to-end solution, and ongoing monitoring and evaluation. 
By providing prompt and accurate assistance to people in life-threatening situations, the implementation of the 911-AI-PREDICT system has the potential to save lives and change how emergency response is conducted.
![Picture1](https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/212a3228-61fd-41c1-a35a-65a719a092e5)
![Picture2](https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/297d107c-9b08-438a-80ec-a6839e271f08)


## Introduction
Current 911 dispatch technologies create complex issues and place a significant load on human operators. Dispatchers must multitask by receiving the distress call, questioning anxious callers, determining the nature of the problem, and sending the proper emergency response personnel. Despite well-trained systems, this procedure frequently experiences delays and errors. Furthermore, because current dispatch systems rely primarily on manual entry for record-keeping, audio data is kept in raw formats that are difficult to study and analyze. 
To solve these problems, novel methods are needed to improve the effectiveness of information gathering from callers, hasten and improve the accuracy of information synthesis, and hasten the detection of potentially life-threatening illnesses.![Picture13png](https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/cd7086aa-6c1d-4054-835f-ff29b0eee496)
![Picture4](https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/dab7d2c7-5b12-4bc8-8e21-f18b704ae360)
![Picture5](https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/a9daa6c8-a478-4cd5-acbe-b1ea26a71fda)

The 911 Artificial Intelligence (AI) Platform for Recognition of Emergencies through Directed Classification (911-AI-PREDICT) system aims to fundamentally improve the early and precise identification of life-threatening medical emergencies reported through emergency 911 calls, revolutionizing emergency response procedures. This cutting-edge technology intends to direct the allocation of relevant resources to the emergency scenario, providing a quick and effective reaction by leveraging the power of real-time AI-driven decision support. 
Two key AI components make up the proposed 911 Artificial Intelligence (AI) Platform for Recognition of Emergencies through Directed Classification (911-AI-PREDICT) system. First, a real-time transcriber, or listener, will pay close attention to live emergency calls in order to capture salient details and important information. Second, a real-time classifier will use the material that was extracted and the contextual audio features to foretell the existence of potentially fatal disorders including cardiac arrest, myocardial infarction, stroke, or trauma. The 911-AI-PREDICT system seeks to greatly improve the responsiveness and effectiveness of emergency dispatch systems by merging these AI components. With this development, communities will be able to quickly provide the necessary emergency medical services (EMS) care to the right place at the right time.
The introduction of this platform has the potential to transform emergency response by guaranteeing that those in danger of losing their lives receive aid more promptly and accurately.
![Picture16png](https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/49296f11-a8b4-49d1-8704-1319f1712ae5)<img width="469" alt="Picture7" src="https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/52af51e9-a998-4835-84f9-d301aff0eaf1">

<img width="468" alt="Picture8" src="https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/0db940c9-5896-4e90-9c3e-3fe8d284f1af">
<img width="468" alt="Picture9" src="https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/42da3354-0cc6-4b17-9118-056b774c185b">
![Picture10](https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/2f31f5e0-b9d2-4fbd-96ef-15735dad6007)
<img width="323" alt="Picture11" src="https://github.com/Harshinikavuru2608/911-AI-Predict/assets/125713954/355d6582-0b1b-43f8-b2ca-91384b5e8f3b">



## STEPS:
1) Managed comprehensive, unordered datasets from the 911 call center, focusing on data integrity and confidentiality. Given the challenge of handling huge, dynamic datasets, I developed an efficient database system using MongoDB. Later organized the data, meticulously removing all redundant information and thereby ensuring the database’s effectiveness and reliability for the project.
2) Ensured data integrity and confidentiality, and implemented robust data backup and disaster recovery protocols using AWS S3 for high availability and data durability.
3) Developed an impeccable rule-based call screener algorithm, efficiently filtering out ’noise’ calls with a 100% success rate
4) Used the latest voice recognition tools like Whisper, Otter AI, and Google API, to achieve nearly perfect transcription accuracy
5) Utilized smart Heuristic techniques to link the calls to their EMS record, and they achieved a linkage rate of close to 98% when the call has an extractable address and a geocode fence representing the jurisdiction of the dispatch center.
6) Delved into a variety of encoding methods to create embeddings. I started with Doc2Vec, progressed to BERT sentence transformers, and then applied a version of BERT that had been fine-tuned with medical documents.
7) Validated the quality of the embeddings, by employing t-SNE visualization, which revealed a significant improvement in the grouping of similar types of data.
8) Leveraged Hugging Face models for keyword extraction and used terminology matching to create more medical terms instead of lay-man terms, further refining the clustering effect in the t-SNE plots.
9) Utilized the linked dataset to train a machine-learning classifier, to identify the ”first impression” or the critical label of heart attack, trauma, difficulty breathing, fire with a F1 scores lying between 0.85 to 0.90 using a BERT fine-tuned model to generate embeddings of the transcription, followed by an SVM classifier.
10) Employed batch scripting to automate and streamline the execution of complex data processing tasks, the operation of AI models, including transcription accuracy enhancement, EMS record linkage, and machine learning classifier training, significantly enhancing project efficiency and reliability.

