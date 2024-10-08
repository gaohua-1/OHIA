# OHIA
A new strategy focusing on feature interactions between objects for temporal action proposal generation
=
ABSTRACT
-
In this paper, we study the task of generating temporal action proposals. This task aims to determine the temporal boundaries of the start and end of each action instance in the untrimmed video. Inspired by the process of human perception of an action in real life, we focus on the information of various entities in the action scene and analyze the interaction between them. Entity information generally includes people, objects, and background information. Most of the existing methods, which do not explore the entity information sufficiently, simply stack and merge different types of entity information, or only explore the interactions between people and objects as well as people and people in the scene, ignoring the importance of the intrinsic connection between objects and objects, we believe that the objects in the video do not exist in isolation and that they interact with each other to form a variety of relationships, which can provide a rich context and information. Therefore, exploring the intrinsic connections between objects is crucial for the effective generation of temporal action proposals. Therefore, in this article, we examine the relationship between various entities from a new perspective and design the interaction analyzer (IA), which contains the Object Interaction Analyzer (OIA) and the Human-Object Interaction Analyzer (HOIA). The OIA further explores the correlation between objects and objects, while the HOIA conducts an in-depth analysis of the interaction between people and objects. They are used to fully tap the potential clue information of these entity relationships and help locate the boundary of the action. While fully exploring object-object and person-object relationships, we further consider that these relationships often also contain negative correlation information, which may interfere with identifying action boundaries or even play a reverse role. Based on this consideration, we designed the Relationship analyzer (RA) in the interaction analyzer to change these negative relationships, reduce their negative effects, and produce higher-quality temporal action proposals. In addition, to further validate the quality of the proposal, we comprehensively consider the association between atomic actions and integrity actions and propose a unity proposal classification strategy based on decomposition and integrity actions further to improve the recognition accuracy of proposal action categories. We conducted experimental exploration on the self-made action dataset and conducted comprehensive experiments and ablation experiments on the public dataset thumos14 to verify the effectiveness of our method. Finally, the performance of AR@100 and AR@200 on the thumos14 dataset reached the SOTA results. On the self-made dataset, AR@50 reached 34.89%, the performance of AR@100 reached 41.45%, and the performance of AR@200 reached 48.55%. The experimental results show the method has significant performance and generalization in TAPG and TAD. 

Activity RESULT
-
|Models| Feature|	AR@100	|AUC(val)|
| --- | --- | --- | --- |
|OURS|	C3D	|77.93%	|69.92%|

Thumos14 RESULT
-
|Models|	Feature|	AR@50	|AR@100	|AR@200|
| --- | --- | --- | --- | --- |
|OURS|	C3D|	44.77%|	52.63%|	58.71%|

CODE
-
code is coming soon
