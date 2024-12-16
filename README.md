# Mechanistic-Interpretability-paper-list

This is a list of papers on Mechanistic Interpretability, aiming to organize and share research progress in this field.

## Paper Collection
### Circuit
| Paper | Techniques | TL;DR | 
|------|----------------|------|
| [INTERPRETABILITY IN THE WILD: A CIRCUIT FOR INDIRECT OBJECT IDENTIFICATION IN GPT-2 SMALL](https://arxiv.org/abs/2211.00593) |path patching,Evaluation| This paper conducts a mechanistic interpretability study of GPT-2 Small for the Indirect Object Identification (IOI) task using circuit analysis. It identifies a circuit of 26 attention heads responsible for performing the task and introduces quantitative criteria—faithfulness, completeness, and minimality—to validate the circuit's explanation, providing evidence and methods for understanding larger language models.  |
| [Towards Automated Circuit Discovery for Mechanistic Interpretability(NeurIPS'23)](https://arxiv.org/pdf/2304.14997) | ACDC |The paper introduces Automatic Circuit Discovery (ACDC), a method to automate the identification of computational subgraphs (circuits) responsible for specific behaviors in neural networks, demonstrating its effectiveness by rediscovering known circuits in tasks performed by GPT-2 Small.|  
| [Attribution Patching Outperforms Automated Circuit Discovery(NeurIPS'23 ATTRIB Workshop)](https://arxiv.org/pdf/2310.10348) | Edge Attribution Patching (EAP) |This paper introduces Edge Attribution Patching (EAP), a novel method for automated circuit discovery that efficiently identifies relevant computational subgraphs (circuits) in neural networks by approximating activation patching, demonstrating higher accuracy and lower computational cost compared to existing methods like ACDC.  |  
| [Have Faith in Faithfulness: Going Beyond Circuit Overlap When Finding Model Mechanisms(COLM 2024)](https://arxiv.org/pdf/2403.17806) | Edge Attribution Patching with Integrated Gradients (EAP-IG) |This paper introduces Edge Attribution Patching with Integrated Gradients (EAP-IG), a novel method for identifying faithful computational circuits in language models, demonstrating improved faithfulness over traditional Edge Attribution Patching (EAP) while highlighting the limitations of using circuit overlap as a proxy for faithfulness. |  
| [Knowledge Circuits in Pretrained Transformers (NIPS 2024)](https://arxiv.org/pdf/2405.17969) | Knowledge Circuits |This paper introduces the concept of Knowledge Circuits, analyzing how components like attention heads and MLPs in Transformers collaborate to store and express knowledge, and using this framework to study tasks such as factual recall, bias, and language model behaviors like hallucinations and in-context learning.|  
| [Transformer Circuit Faithfulness Metrics are not Robust  (COLM 2024)](https://arxiv.org/pdf/2407.08734) | faithfulness metrics |This paper investigates the robustness of circuit faithfulness metrics in transformers, showing that small variations in ablation methodologies and metrics can significantly alter the evaluation of a circuit's faithfulness, emphasizing the need for clearer and more consistent methodologies in mechanistic interpretability research.|  
| [Circuit Component Reuse Across Tasks in Transformer Language Models(ICLR 2024)](https://arxiv.org/pdf/2310.08744) | circuit component reuse |This paper investigates circuit component reuse across different tasks in Transformer language models, demonstrating that circuits discovered for one task (e.g., Indirect Object Identification) are significantly reused for seemingly different tasks (e.g., Colored Objects), with 78% overlap in critical components, suggesting that models rely on general-purpose algorithmic building blocks.| 
| [Evaluating Brain-Inspired Modular Training in Automated Circuit Discovery for Mechanistic Interpretability](https://arxiv.org/pdf/2401.03646) | Brain-Inspired Modular Training |This paper evaluates Brain-Inspired Modular Training (BIMT) for enhancing neural network interpretability, demonstrating its ability to improve the efficiency and quality of Automated Circuit Discovery (ACD) by enabling the identification of sparse, interpretable circuits while addressing computational trade-offs in training and inference.| 
| [Sparse Feature Circuits: Discovering and Editing Interpretable Causal Graphs in Language Models(ICLR 2025)](https://arxiv.org/pdf/2403.19647) | Sparse Feature Circuits |This paper introduces Sparse Feature Circuits, a method to discover and edit human-interpretable causal subgraphs in language models, enabling fine-grained understanding and manipulation of unintended model behaviors through techniques like Sparse Human-Interpretable Feature Trimming (SHIFT).| 
| [Automatically Identifying Local and Global Circuits with Linear Computation Graphs(ICML 2024 MI Workshop Poster)](https://arxiv.org/pdf/2405.13868) | Transcoders |This paper introduces a novel framework for circuit discovery in Transformer language models using Sparse Autoencoders (SAEs) and Transcoders, enabling fine-grained analysis of local and global circuits through strictly linear computation graphs, and proposes Hierarchical | 
| [Attribution for scalable circuit isolation and evaluation.](https://arxiv.org/pdf/2407.00886) | Contextual Decomposition for Transformers (CD-T) |This paper introduces Contextual Decomposition for Transformers (CD-T), an efficient mathematical method for automated circuit discovery in large language models, enabling fine-grained analysis of transformer components with reduced runtime and improved faithfulness compared to existing methods like ACDC and EAP.| 
| [Sparse Autoencoders Enable Scalable and Reliable Circuit Identification in Language Models. ](https://arxiv.org/pdf/2405.12522) | SAE Circuit |This paper presents a method using Sparse Autoencoders (SAEs) to efficiently and reliably identify circuits in large language models by learning interpretable features from positive and negative examples, achieving superior precision and scalability compared to traditional methods like ablation-based techniques.| 
| [Transcoders Find Interpretable LLM Feature Circuits ](https://arxiv.org/pdf/2406.11944) | Transcoders |This paper explores Transcoders, a novel method for circuit analysis in language models, showing that they outperform Sparse Autoencoders (SAEs) in identifying faithful and interpretable circuits, enabling disentanglement of input-invariant and input-dependent information while scaling efficiently to larger models.| 
| [THE SAME BUT DIFFERENT STRUCTURAL SIMILARITIES AND DIFFERENCES IN MULTILINGUAL LANGUAGE MODELING ](https://arxiv.org/pdf/2410.09223) | Mutillingual Circuit |This paper investigates how multilingual language models (LLMs) represent structural similarities and differences across languages, showing that models employ shared circuits for similar morphosyntactic processes across languages while utilizing language-specific components for unique structures, such as tense marking in English but not in Chinese.|

##Recent Papers
- Transformers Struggle to Learn to Search [arxiv 2412](https://arxiv.org/abs/2412.04703) 
- Modular addition without black-boxes: Compressing explanations of MLPs that compute numerical integration [arxiv 2412](https://arxiv.org/abs/2412.03773)
- Monet: Mixture of Monosemantic Experts for Transformers [arxiv 2412](https://arxiv.org/abs/2412.04139)
- Understanding Multimodal LLMs: the Mechanistic Interpretability of Llava in Visual Question Answering [arxiv 2411](https://arxiv.org/abs/2411.10950)
- Towards a Mechanistic Explanation of Diffusion Model Generalization [arxiv 2411](https://arxiv.org/abs/2411.19339)
- Understanding Llava's Visual Question Answering in a Mechanistic View [arxiv 2411](https://arxiv.org/abs/2411.10950)
- How Transformers Solve Propositional Logic Problems: A Mechanistic Analysis [arxiv2411](https://arxiv.org/abs/2411.04105)
- New Faithfulness-Centric Interpretability Paradigms for Natural Language Processing [arxiv 2411](https://arxiv.org/abs/2411.17992)
- Revelio: Interpreting and leveraging semantic information in diffusion models [arxiv 2411](https://arxiv.org/abs/2411.16725)
- Do I Know This Entity? Knowledge Awareness and Hallucinations in Language Models [arxiv 2411](https://arxiv.org/abs/2411.14257)
- ULTra: Unveiling Latent Token Interpretability in Transformer Based Understanding [arxiv 2411](https://arxiv.org/abs/2411.12589)
- Towards Unifying Interpretability and Control: Evaluation via Intervention [arxiv 2411](https://arxiv.org/abs/2411.04430)
- Enhancing Neural Network Interpretability with Feature-Aligned Sparse Autoencoders [arxiv 2411](https://arxiv.org/abs/2411.01220)
- ADAPTIVE CIRCUIT BEHAVIOR AND GENERALIZATION IN MECHANISTIC INTERPRETABILITY [arxiv 2411](https://arxiv.org/abs/2411.16105)
- Mechanistic Interpretability of Reinforcement Learning Agents[arxiv 2411](https://arxiv.org/abs/2411.00867)
- Llama Scope: Extracting Millions of Features from Llama-3.1-8B with Sparse Autoencoders[arxiv 2410](https://arxiv.org/abs/2410.20526)
- Interpreting Affine Recurrence Learning in GPT-style Transformers[arxiv 2410](https://arxiv.org/abs/2410.17438)
- SCIURus: Shared Circuits for Interpretable Uncertainty Representations in Language Models[openreview](https://openreview.net/pdf/d6b53b87962a52c8b3d13ef23d9a52fff4ef5f3c.pdf)
- Interpretability as Compression: Reconsidering SAE Explanations of Neural Activations with MDL-SAEs [arxiv](https://arxiv.org/abs/2410.11179)
- HyperDAS: Towards Automating Mechanistic Interpretability with Hypernetworks [openreview](https://openreview.net/forum?id=6fDjUoEQvm)
- Identifying Sub-networks in Neural Networks via Functionally Similar Representations [arxiv 2410](https://arxiv.org/abs/2410.16484)
- Everything, Everywhere, All at Once: Is Mechanistic Interpretability Identifiable?[openreview](https://openreview.net/forum?id=5IWJBStfU7)
- Rethinking Evaluation of Sparse Autoencoders through the Representation of Polysemous Words[openreview](https://openreview.net/forum?id=HpUs2EXjOl)
- The Computational Complexity of Circuit Discovery for Inner Interpretability[arxiv 2410](https://arxiv.org/abs/2410.08025)
- Understanding Llava's Visual Question Answering in a Mechanistic View [arxiv 2411](https://arxiv.org/abs/2411.10950)
- Towards Principled Evaluations of Sparse Autoencoders for Interpretability and Control [arxiv 2405](https://arxiv.org/abs/2405.08366)

## Related Repositories

Here are some related repositories for Large Language Model (LLM) interpretability:

- [Awesome LLM Interpretability by cooperleong00](https://github.com/cooperleong00/Awesome-LLM-Interpretability)
- [Awesome Interpretability in Large Language Models by ruizheliUOA](https://github.com/ruizheliUOA/Awesome-Interpretability-in-Large-Language-Models)
- [awesome-mechanistic-interpretability-lm-papers](https://github.com/Dakingrai/awesome-mechanistic-interpretability-lm-papers)

