# Enhanced Location Filtering for CAIDA's IPMap Tool Using LLMs

## Purpose

This project aims to refine and restrict the input locations fed into CAIDA's IPMap tool by employing Large Language Models (LLMs), ensuring more accurate and relevant geolocation data processing. Our approach focuses on intelligently filtering and interpreting geolocation hints from RDNS hostnames to enhance the specificity and accuracy of the tool's input data.

## Motivation

Identifying the physical location of Internet routers is crucial for assessing the resilience of network infrastructure, optimizing forwarding paths, and understanding communications' geographic constraints. Utilizing LLMs allows for an intelligent first pass through potential locations, significantly reducing inaccuracies by excluding unsuitable candidates. This project leverages LLMs' natural language processing capabilities to enhance geolocation tools, contributing to more effective routing and communication solutions.

## Limitations of Current Initiatives

Traditional methods rely on regex to decipher geohints in RDNS hostnames, a process hampered by lack of standardization and the potential for misclassification. Our LLM-based approach aims to overcome these limitations by providing flexible, context-aware interpretation of hostname-encoded geolocation hints.

## Why LLMs?

LLMs excel in short-term language processing and interpretation, making them highly suitable for resolving ambiguities in RDNS hostnames. Their ability to reason about unfamiliar or ambiguous data surpasses traditional methods, offering a promising avenue for geolocation enhancement.

## Method of Geolocation Hint Solving

### Fine-Tuning LLMs

We plan to fine-tune a pre-trained LLM on a dataset comprising RDNS hostnames and their known geolocations, enhancing the model's ability to extract and interpret geolocation hints accurately.

### Prompt Engineering

Effective prompt design will guide the LLM in accurately identifying geolocation hints, utilizing a range of queries to accommodate the diversity of hostname formats and conventions.

## Experiments to Conduct

1. **Baseline Performance Assessment**: Establish the accuracy baseline of the current IPMap tool for comparison.
2. **LLM Fine-Tuning Efficacy**: Evaluate improvements in geolocation hint solving accuracy post fine-tuning.
3. **Prompt Engineering Effectiveness**: Determine the most effective prompts through comparative analysis.
4. **Comparative Analysis with Existing Methods**: Compare the LLM-enhanced method against traditional regex-based techniques and other state-of-the-art geolocation methods.
5. **Error Analysis and Model Interpretability**: Analyze errors and experiment with techniques to improve model interpretability.
6. **Sensitivity and Scalability Testing**: Assess the model's performance across different conditions and scales.

## Establishing Ground Truth

### Utilizing Public Datasets

Employing datasets with known locations of network elements as anchor points for establishing ground truth.

### Active Geolocation Techniques

Implementing methods like CBG and TBG to estimate router locations based on network measurements.

### Machine Learning with Human-in-the-Loop

Incorporating expert feedback into the learning process to refine model predictions and ground truth data.

### Delay-based Validation

Using RTT measurements to validate and adjust geolocation predictions, enhancing the ground truth's reliability.

### Integration of Multiple Data Sources

Combining various data sources to validate and corroborate geolocation hints, ensuring robust ground truth data.

## Conclusion

This project represents a significant step forward in the application of LLMs to the domain of network geolocation. By addressing the challenges of interpreting RDNS hostnames and establishing a reliable ground truth, we aim to significantly enhance the accuracy and utility of CAIDA's IPMap tool.

## Collaborators

Daniyal Latif, Ali Levin, Bert Yan

## Acknowledgments

The CAIDA Macroscopic Internet Topology Data Kit - <release dates >,
https://www.caida.org/catalog/datasets/internet-topology-data-kit

---

*This project is a collaborative effort aimed at advancing in Internet router geolocation techniques.*
