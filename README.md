<a name="top"></a>
# Charting New Territories

[**Charting New Territories: Exploring the Geographic and Geospatial Capabilities of Multimodal LLMs**](https://arxiv.org/abs/2311.14656)

**CVPR 2024 EarthVision Workshop [Oral]**

Jonathan Roberts, Timo Lüddecke, Rehan Sheikh, Kai Han, Samuel Albanie

We conduct a series of experiments exploring various vision capabilities of multimodal large language models (MLLMs) within these domains, particularly focusing on the frontier model GPT-4V, and benchmark its performance against open-source counterparts. Our methodology involves challenging these models with a small-scale geographic benchmark consisting of a suite of visual tasks, testing their abilities across a spectrum of complexity. The analysis uncovers not only where such models excel, including instances where they outperform humans, but also where they falter, providing a balanced view of their capabilities in the geographic domain.

[Repo Overview](#top)
  - [Experiments Taxonomy](#experiments-taxonomy)
  - [Takeaways](#key-takeaways)
  - [Data](#data)
  - [Prompts](#prompts)
  - [Citation](#citation)
  - [Questions](#questions)

## Experiments Taxonomy
- Localisation
  - GeoGuessr 
- Remote sensing
  - Classification
  - Change detection
  - Segmentation
  - Bounding boxes
  - Counting
- Mapping
  - Region identification
    - State name from outline
    - City name from maps
    - Island and water body naming from maps
  - Localisation
    - Real-world -> map
    - Map -> real-world
- Flags
  - Identification
- Failure cases
  - Identifying multiple states

## Key takeaways
* Of all the evaluated models, GPT-4V can perform the broadest range of tasks. However, it does not always perform best, e.g., satellite image detection and classification tasks. In general, it recognizes fine-detail well but tends to fail when 
precise localisation is required.
* More broadly, the best model choice depends on the task at hand. Qwen-VL and LLaVA-1.5 in particular often demonstrate good localisation performance.
* Enforcing a specific output format is challenging, models often resort to explanations why they are not capable of performing the task. Among the evaluated models GPT-4V was least susceptible to this behaviour.
* The current generation of leading MLLMs suffer a performance penalty when processing multi-object images, relative to their performance on single object images.

## Data
Data for the majority of the experiments can be found in ```Data```.

## Prompts
Coming soon!

## Citation
If you found our work useful in your own research, please consider citing our paper:

```latex
@article{roberts2023charting,
  title={{Charting New Territories: Exploring the geographic and geospatial capabilities of multimodal LLMs}},
  author={Roberts, Jonathan and L{\"u}ddecke, Timo and Sheikh, Rehan and Han, Kai and Albanie, Samuel},
  journal={arXiv preprint arXiv:2311.14656},
  year={2023}
}
```

## Questions
If you have any questions about our work, please open an issue in this repository.
