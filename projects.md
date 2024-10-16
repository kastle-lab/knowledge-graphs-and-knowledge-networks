## Projects

1. [Data-driven KG Generation from Human Interactions to Inform HRC](#data-driven-kg-generation-from-human-interactions-to-inform-hrc)
2. [Human Action Reasoning Using Knowledge Graphs for Task-Driven VR Biometrics](#human-action-reasoning-using-knowledge-graphs-for-task-driven-vr-biometrics)
3. [Semantic Analysis of Embeddings from Text Corpus](#semantic-analysis-of-embeddings-from-text-corpus)
4. [Semantic Fine-tuning of Pre-Trained Models](#semantic-fine-tuning-of-pre-trained-models)
5. [Knowledge Graph Visualization](#knowledge-graph-visualization)
6. [Utilizing GNNs for Interpretable Analysis of Biological Data](#utilizing-gnns-for-interpretable-analysis-of-biological-data)
7. [Micro-domain Experts using Bibliometric KGs and RAG](#micro-domain-experts-using-bibliometric-kgs-and-rag)
8. [Optimization Techniques in KGs for Topological Network Optimization](#optimization-techniques-in-kgs-for-topological-network-optimization)
9. [Generalizability-Enhanced GNNs: Addressing Real-World Graph Challenges](#generalizability-enhanced-gnns-addressing-real-world-graph-challenges)
10. [KG-based Self-Powered IoT System](#kg-based-self-powered-iot-system)

### Data-driven KG Generation from Human Interactions to Inform HRC

**Overview.** The objective of the proposed work is to investigate generating knowledge graphs from
unstructured multimodal data of human task performance to inform human-robot interaction (HRC).
Knowledge graphs provide the potential in HRC to fill in knowledge gaps that the
agents—whether human or artificial—may have and that can prohibit accomplishment of tasks such as
assembly, disassembly, object handover, or collaborative object handling. However, limited work
exists on automated creation of knowledge graphs that inform HRC tasks. Current methods are
largely restricted to deconstructing 3D models into assembly sequences. An open scope
exists in creating knowledge graphs by studying the interactions performed by humans during
the collaborative process. The work will contributed novel approaches that automatically con-
struct knowledge graphs by analyzing 3D data on multi-person interactions during tasks such as
handover and assembly using the PI’s pre-collected and publicly available Human-Object-Human
(HOH) dataset and the publicly available Assembly101 dataset. The research will involve investi-
gating unsupervised techniques to cluster pre-generated trajectories in the HOH and
Assembly101 datasets into distinct components representing individual units of action (e.g., grasping,
handing, connecting), detectors such as YOLO-v8 and OpenPose to conduct object, body
pose, and hand pose detection, and semi-supervised methods to develop graphical
representations of the activity where nodes consist of entities involved (object parts, hands, persons), and
edges consist of the action performed. Metrics reported will include accuracy and mean average
precision (mAP) of detecting individual entities, and the graph edit distance between constructed
knowledge graphs and ground truth labeled graphs.

**Intellectual Merit.** The proposed work greatly advances current knowledge in HRC by providing a
grounded approach to create knowledge graphs from unstructured data to inform a range of
collaborative tasks that traditionally rely on structured graphical knowledge. By focusing on automated
detection of relationships between fundamental entities, i.e., body and object parts, the research
ensures generalizability of the proposed methods to inferring knowledge graphs from data
collected in a wide range of collaborative scenarios. Knowledge graphs generated by the proposed
work provide the potential of enabling downstream tasks such as knowledge gap filling or provision
of alternatives for parts and actions. The generation of semantically interpretable relationships and
their use to drive robotic algorithms provides the benefit of ensuring predictable behavior to the
human involved in HRC.

**Broader Impacts.** Successful accomplishment of the proposed work ensures that robotic
assistants deployed in collaborative environments in home, work, and industrial settings demonstrate
knowledge of human preferences and predictable behavior, benefiting safe HRC. By providing a
consistent ontology for the behaviors of human and robot collaborators, the proposed work
improves explainability of robot actions, benefiting dissemination of knowledge in HRC to a wider
community. The PI plans to leverage her lab’s tutorials website to disseminate findings from
the research, the resulting knowledge graphs, and their impact toward HRC in the form of course
modules on integrating robotic control with knowledge on human activity during collaborative tasks.

### Human Action Reasoning Using Knowledge Graphs for Task-Driven VR Biometrics

**Overview.** Task-driven VR biometrics involves identifying or authenticating users based on the
actions of a user in a virtual environment. Existing approaches for task-driven VR biometrics
rely on a manual approach for determining body parts, such as wrist or arm or legs, objects, ball or
bat, and actions, bend or grab or lift, to determine the actions needed to perform the VR task and
the corresponding movements for security. Recent approaches on using visual knowledge graphs
for reasoning on human actions from video offer an automated approach for inferring the body
parts, objects, and actions needed to develop immersive environments that enable task-driven
VR biometrics. Currently, there exists no work on leveraging visual knowledge graphs based on
human action reasoning to generate immersive environments for task-driven VR biometrics. The
goal of the proposed research is to automatically generate body parts, objects, and actions for
creating task-driven immersive environments for VR biometrics based on visual knowledge graphs
of human action recognition. To conduct human action recognition, the proposed work will use the
Kinetics-TPS dataset, which provides 7.9 million annotations of 10 human body parts along with
7.9 million part states, in other words an understanding of how the human body moves, from 24
action classes. The work will use the approach of Ma et al. to generate visual knowledge
graphs consisting of body parts, interactive objects, and actions from the ’front raises’, ’skipping
rope’, ’hitting baseball’, ’lunge’, ’hammer throw’, and ’throwing discus’ activities in the
Kinetics-TPS dataset. Corresponding immersive VR applications will be developed for each activity that
ensures the relationships with the body parts, interactive objects, and actions are maintained to
enable a 1-1 relationship between the real-world and VR activity. The work will compare
deep-learning based approaches using knowledge-graph enhanced activities versus traditional
approaches using standardized metrics such as accuracy and equal error rate.

**Intellectual Merit.** The proposed work advances the current body of knowledge in VR biometrics
by leveraging visual knowledge graphs to automatically generate body parts and their
corresponding action sequences based on automated reasoning from videos of human activities. By focusing
on the automated detection of relevant body parts, actions, and their relationships, the research
enables bias-free generation of tasks, parts, and actions that can be leveraged to create synthetic
environments for securing serious immersive spaces. The visual knowledge graphs generated by
the research can enable researchers in security and human-computer interaction fields to jointly
reason on the impact on VR-based security measures that rely on free-form human activity in
immersive spaces. Through the generation of visual knowledge graphs researchers can infer
alternate body parts, actions, or relationships to enable diverse user bases to interact in VR while
maintaining overall security.

**Broader Impacts.** The successful accomplishment of the proposed research ensures that as
immersive spaces in serious applications in healthcare, education, military, and finance that will
rely on the tasks performed by the user in the VR space to secure them demonstrate awareness of
the real-world physical dynamics of human motion. By leveraging reasoning through observations
of human behavior from video data, the research enables explainability of the underlying security
algorithms to ensure that learning algorithms do not make incorrect assumptions of how humans
move. The PI will release the visual knowledge graphs generated through video-based reasoning,
the resultant immersive VR applications, trajectories of human action, and benchmark algorithms
through his research website (http:.//tars-home.github.io).

### Semantic Analysis of Embeddings from Text Corpus

**Overview.** While a traditional dictionary describes different senses of a word or provides synonyms and
antonyms associated with a word as textual description, this description is inadequate for gleaning
computable semantics for flexible processing. So, vector embeddings have been used to capture
meanings of words based on their usage pattern in a large corpus. However, the
embeddings capture the semantics based on the notion of substituitivity of usage, potentially intermingling
multiple senses. Further, the well-known cosine similarity (that is, normalized dot product) cannot
cleanly separate notions of synonymy and antonymy (opposites) because it measures
substitutivity, not sense, thereby confounding the two in practice.

**Intellectual Merit.** In this project, we propose to visualize the vector embeddings on a low
dimensional space to see how synonymy, antonymy, and ambiguity manifests to get a deeper visual
understanding of the relationships among the meanings of words. We then explore if we can
segregate a vector embedding in terms of various primitive functional senses using context, and
embeddings of synonyms, antonyms, and completely independent words are related (shedding
light on the nuances of cosine similarity). We will do all this through concrete examples first. We
will then explore the science of vector embeddings, attempting to distil formal properties and their
relationship to more fundamental functional senses.

**Broader Impacts.** Vector embedding-based semantics has been used extensively in Large
Language Models. Understanding the nature of vector embeddings will help us improve the design
and analysis of vector operations by promoting their interpretability and applicability.

### Semantic Fine-tuning of Pre-Trained Models

**Overview.** Developing application specific Large Language Models (LLMs) from scratch are computationally
prohibitive. So, exploring application specific fine-tuning provides a viable cost-effective approach.
We investigate how to adapt vector embeddings of known concepts gleaned from large text corpus
using information in (knowledge) graphs to obtain contextually rich and application-relevant vector
embeddings to enhance semantic processing.

**Intellectual Merit.** Integration of vector embeddings gleaned from text-corpus as well as
(knowledge) graphs can promote contextual relevance and reliable reasoning. This exercise can
provide a deeper understanding of the interplay between parameterized knowledge incorporated in
pre-trained LLMs, locally adapted application-specific LLMs using graph-based context, and
use-specific prompts for minimizing hallucinations.

**Broader Impacts.** We propose to analyze cell-gene-differential expression graph to explore how
to seed the vector embeddings of concepts from background knowledge, use graph neural network
algorithms to synthesize richer application-specific embeddings, and then use those for predictive
analytics.

### Knowledge Graph Visualization

**Overview.** Graph data, including KG data, is frequently difficult to visualize, due to the complexity
of the involved information. Dense interconnections can obfuscate data, but viewing by only a
few relations (edges) at a time may lose capacity for visual inference. In this topic, students will
develop visualization methods for graphically representing knowledge graphs: cognitive science
mechanisms for the limits of human ingestion of (knowledge) graph data; understanding top-level
aspects of a KG through query-driven visualizations; or even using visualization techniques to
compare and understand differences in latent spaces. Where possible, we will leverage open
source toolkits to derive the visual representations.

**Intellectual Merit.** The use of KGs in machine learning (i.e., an aspect of neurosymbolic AI) is
of growing popularity. In particular, KG embeddings are one way that this is accomplished, which
provide capacity to perform, for example, link prediction between entities. Understanding exactly
how these models work in a human intuitive manner is fundamental to progressing our intuition
of latent spaces, which for a human, generally requires a visual component. This would provide
straightforward access to what the KG encodes. As a result, students engaged with this topic will
learn to understand different visualization tools and how to apply them to (knowledge) graph data.

**Broader Impacts.** Engaging with this topic will broaden the students’ understanding of the KGs
and how one can derive a better understanding of the data and how to derive inferences based on
the knowledge graph through leveraging visual representations.

### Utilizing GNNs for Interpretable Analysis of Biological Data

**Overview.** The proposed project aims to leverage the power of Graph Neural Networks (GNNs)
to analyze and interpret complex biological data. GNNs, a cutting-edge development in
machine learning, are particularly well-suited for this task due to their ability to capture relationships
and interactions in data structured as graphs. Biological data, such as protein-protein
interaction networks, gene regulatory networks, and metabolic pathways, naturally fit this
representation.

Our approach will focus on constructing comprehensive graph representations of biological datasets
and applying GNNs to extract meaningful patterns and insights. By doing so, we aim to overcome
the limitations of traditional methods that often struggle with the complexity and high
dimensionality of biological data. The intellectual merit of this project lies in its potential to provide
more interpretable and accurate models for biological data analysis, which could lead to significant
advancements in understanding biological processes and disease mechanisms.

**Intellectual Merit.** The project will be executed by applying Graph-based machine learning
algorithms, e.g., Laplacian Eigenmaps, Graph Neural Networks, etc, on high-dimensional
biological data sets which are publicly available (e.g., ALLAML, GLIOMA, Prostate_GE). The
performance of the student will be measured based on their ability to set new experiments to test
a hypothesis about the data, train a graph machine learning model and evaluate its performance
on the biological data, and the ability to visualize the data, etc.

**Broader Impacts.** The broader impact of this project extends to multiple domains within and
beyond biological research. Improved interpretability of biological data can accelerate discoveries in
genomics, proteomics, and systems biology, leading to novel therapeutic targets and personalized
medicine strategies. Moreover, the methodologies developed could be applied to other fields that
utilize graph-based data, such as social network analysis, and cybersecurity.

### Micro-domain Experts using Bibliometric KGs and RAG

**Overview.** Large language models (LLMS) have become increasingly capable of complex tasks in
the scientific domain including summarizing existing literature, comparison of scientific papers, and
making recommendations for papers to read based on scientific interests. One limitation of LLMs
is the significant computation, memory, and power requirements associated with training (and in
many cases, even tuning) them. As modern LLMs are becoming capable of very long (25,000+
word) prompts, a great deal of information can be carried along with a prompt to impart information
to the LLM that was not present at the time of training. Retrieval augmented generation (RAG)
has taken advantage of this capability to improve the ability of LLMs to respond to prompts with
specific known facts, reducing hallucinations and other artifacts of LLM training. By creating and
maintaining a citation-based knowledge graph (KG) in a particular domain area, RAG may allow
an LLM to serve as an expert advisor in a specific domain. The KG will allow the LLM to maintain
currency and relevancy between training and tuning cycles.

**Intellectual Merit.** This project will explore the capabilities of LLM/RAG based domain experts
in specific scientific domains, and will establish baseline performance for comparison with other
approaches. Citation-based KGs will be explored as a vehicle for maintaining knowledge of the
current state of the art in specific scientific domains.

**Broader Impacts.** The KGs and RAG systems created will be valuable tools in their domains,
which will include evaluation of pediatric medical records for indications of specific interventions,
and scientific recommendations in the social psychology domain. In addition, student participants
will be trained in several of the most current and active areas of research in the artificial intelligence
domain, helping to prepare them to enter graduate studies in this field.

### Optimization Techniques in KGs for Topological Network Optimization

**Overview.** This research investigates the application of optimization algorithms within knowledge
graphs to address complex topological network optimization problems.

Knowledge graphs represent data in a structured manner, capturing
relationships and entities in a network-like format. By leveraging these graphs,
we can formulate and solve optimization problems that involve finding
optimal paths, resource allocation, and network design.

**Intellectual Merit.** This research aims to advance the theoretical
foundations of optimization in knowledge graphs and enhance practical
methodologies for network design and analysis. The implementation of
optimization techniques in the context of knowledge graphs can lead to efficient
algorithms and innovative solutions to problems such as network
congestion, routing, and topology management. The implementation of
optimization techniques in the context of knowledge graphs can lead to innovative
solutions to problems e.g., network congestion and topology management.

**Broader Impacts.** This research is expected to touch upon multiple domains such as
telecommunications, transportation, and cybersecurity. In telecommunications, optimizing network topologies
can lead to more efficient data transmission and reduced operational costs. In transportation,
improved network design can enhance real-time route planning and reduce travel times. In
cybersecurity, optimizing network topology can help in detecting vulnerabilities and strengthening
defenses. Additionally, the methodologies developed could be applied to other areas where
knowledge graphs are used, such as recommendation systems, semantic search, and bioinformatics,
broadening the impact of the research.

### Generalizability-Enhanced GNNs: Addressing Real-World Graph Challenges

**Overview.** Graphs represent natural, yet complex, relationships between objects, which find
extensive applications in numerous real-world domains, such as social network analysis,
molecular chemistry, and fraud/spam detection. To perform such tasks, various
graph neural networks (GNNs) have been developed as prevalent models to aggregate
neighborhood information and boost performance. However, despite their remarkable
representation learning and inference ability, GNNs often fail to generalize to specific scenarios, such as
labeled data scarcity, class imbalance, graph heterophily with dissimilar connections,
adversarial graph manipulation, and graph over-density. These frequently arise in
practical applications, underscoring the gap between theoretical assumptions and real-world limitations.

**Intellectual Merit.** In this project, students will be exposed to state-of-the-art GNNs with spatial
and spectral designs by exploring their fundamental structures, layerwise computations, training
process, and adaptations into different downstream tasks. Building on this foundational knowledge,
they will engage in hands-on experiments to investigate how various graph challenges, including
class imbalance, few-shot learning, graph heterophily, over-smoothing, and adversarial attacks,
impact GNN performance. By analyzing these effects, students will develop innovative strategies for
addressing these challenges and enhancing the generalizability of GNN models. Specific solutions
will include: (1) graph oversampling to generate a balanced class distribution, (2) pseudo-labeling
with graph active learning to enrich label information for few-shot learning, (3) adaptive message
aggregation to employ separate filters for neighborhood aggregations, (4) edge dropping for graph
sampling to reduce graph density, and (5) adversarial training to self-perturb node features and
graph structures against malicious attacks.

**Broader Impacts.** This project will significantly enhance students’ understanding of both
theoretical and practical aspects of GNNs, contributing to the development of more effective and adaptable
models for a range of real-world applications. In addition to advancing technical knowledge,
students will acquire invaluable experience in research methodologies, problem-solving, and critical
thinking. This hands-on experience will not only prepare them for future careers in academia or
industry but also equip them with skills to tackle complex problems and drive innovation in diverse
and dynamic settings. The project’s emphasis on real-world challenges and applications will foster
a deeper appreciation of the societal impacts of graph learning, promoting responsible and ethical
use of these techniques.

### KG-based Self-Powered IoT System

**Overview.** Over 90% of wetlands in Ohio have been lost due to conversion and development around lakes and
water-ways, which far exceeds the national average of 50%. Monitoring these natural environments is
crucial for their protection, yet is time-consuming and expensive.
Internet of Things (IoT) offers an efficient
solution by providing ubiquitous intelligence and
interconnections among diverse physical
objects and enabling real-time monitoring
and decision-making. However, the
heterogeneity of IoT devices (e.g., protocols and
companies) prohibits cost-effective
automatic anomaly detection. The nature of
IoT environment monitoring system,
characterized by temporal, spatial, and topological
properties, are well represented as KGs.
Specifically, the proposed
interdisciplinary KG-powered research includes (1)
designing a surrogate model for the environment
monitoring IoT system using KGs; (2)
augmenting the surrogate model with real-world
environment infrastructure; and (3) anomaly
detection with cascading impacts predictions,
allowing timely corrective actions.

**Intellectual Merit.** The proposed work will revolutionize the wetland monitoring system by
transforming environment protection and expert knowledge into customized knowledge-based graph
models, enabling predictions of anomalies ahead of time and automating the monitoring in remote
and maintenance tasks. Transforming interdisciplinary knowledge of IoT, embedded systems, and
AI into actionable insights paves the way for new developments in the field.

**Broader Impacts.** By leveraging IoT, environmental monitoring systems can achieve better
coverage, accuracy, and responsiveness, ultimately contributing to more effective environmental
protection and conservation efforts. Early detection of environmental issues is crucial for timely
interventions, preventing further degradation, and promoting conservation. The proposed project
advances towards a fully sensed digital twin of the environment monitoring system by augmenting
the surrogate model, enhancing monitoring and management capabilities.
