# sketchbot
SketchBot is a research prototype for formative feedback on ray-tracing sketches in computer graphics education. Learners draw task-specific ray constructions; the system sends a screenshot, task rubric, and reference answer to a vision-language model (VLM), then presents concise feedback for revision.

This repository contains the code for the paper "SketchBot: Towards a VLM-Based Formative Feedback Tool for Ray-Tracing Sketches in Computer Graphics Education." 

We will be updating the code and adding supplementary results.

| Path                       | Contents                                                                                |
| -------------------------- | --------------------------------------------------------------------------------------- |
| `data/reference-images/`   | One canonical set of the four reference answers and task scene image.                   |
| `data/simulated-sketches/` | 85 researcher-created simulated learner sketches across four tasks.                     |
| `data/model-evaluations/`  | Outputs for 7B/32B and task-only/criteria-and-reference conditions.                     |
| `data/expert-ratings/`     | Anonymized expert ratings and non-identifying aggregate summaries.                      |
| `docs/`                    | Dataset and reproduction notes.                                                         |

## License

Source code and the included research materials are released under the [MIT License](LICENSE). Third-party model weights and services remain subject to their respective licenses and terms.
