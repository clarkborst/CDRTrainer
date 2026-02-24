# CDRTrainer: 2D Aircraft Conflict Resolution – Reinforcement Learning Demonstrator

**Clark Borst**\
*Delft University of Technology*\
*Faculty of Aerospace Engineering*\
*Department: Control & Operations*\
*Section: Control and Simulation*\
*2629 HS, Delft, The Netherlands*\
https://cs.lr.tudelft.nl

This project provides an interactive JavaScript/HTML application that demonstrates reinforcement learning for two-dimensional aircraft conflict detection and resolution (CD&R).
The goal was to explore various options (i.e., action shielding, human feedback and expert demonstrations) to speed up learning and to make the agent demonstrate more operationally accepted behavior. 

The application simulates a **150 × 100 NM airspace sector** containing an ownship and an intruder aircraft. Random encounter geometries are generated to create potential conflicts. 
A reinforcement learning agent (linear Q-learning with function approximation) learns to:

- Avoid loss of separation  
- Restore the original flight heading after conflict resolution  
- Minimize cross-track deviation from the nominal route  
- Minimize the number of maneuver events  

The application and its source code is embedded in a single `HTML` file. Just run the file in your browser and you are ready to go!

More detailed documentation can be found in the `PDF` file named `CDRTrainer.pdf`.

![CDRTrainer_demo](https://github.com/user-attachments/assets/c88f51fc-cb3d-41e7-8dea-bff8a22e3030)

---

## Features

- Real-time visualization of aircraft trajectories  
- Configurable training parameters (learning rate, shielding, expert demonstrations, etc.)  
- Live plots for:
  - Episode reward  
  - Success and failure rates   
  - Feature importance (RMS-based relevance analysis)  
- Step-by-step execution log for traceability and debugging  
- Optional action shielding and expert (Velocity Obstacle-based) demonstrations  

---

## Purpose

This application is designed for **educational and research purposes** to explore how reinforcement learning behavior can be shaped to 
showcase more operationally accepted behavior through:

- Reward design  
- Feature engineering  
- Action shielding  
- Expert demonstrations  
- Human feedback mechanisms  

The demonstrator may highlight both the potential and the limitations of reinforcement learning in safety-critical decision-making tasks.

---

## Disclaimer

This software is intended solely for educational and research use.  
It is not certified, validated, or suitable for real-world aviation or air traffic control operations.

---

## 📜 License and Citation

This demonstrator is provided for **education, academic research and commercial use** under
the **GPL-3** license.

You are free to download and/or fork the project and:
- **Use** the demonstrator in research studies or teaching
- **Modify** or extend the code
- **Share** adapted versions under the same license

You must:
- **Attribute** the original author of the application
- **Cite** this repository (see citation below)
- **Distribute adaptations** under the same license

---

### 📖 Citation

If you use or adapt this application in your research or education, please cite it as follows:

#### APA format
> Borst, C. (2026). *CDRTrainer: Safe Reinforcement Learning with Human Feedback and Expert Demonstrations for 2D Aircraft Conflict Resolution.*  Delft University of Technology. DOI: https://doi.org/10.5281/zenodo.18715223. Available at: [https://github.com/clarkborst/CDRTrainer](https://github.com/clarkborst/CDRTrainer)

#### BibTeX
```bibtex
@misc{Borst_CDRTrainer_2026,
  author       = {Clark Borst},
  title        = {{CDRTrainer: Safe Reinforcement Learning with Human Feedback and Expert Demonstrations for 2D Aircraft Conflict Resolution}},
  year         = {2026},
  publisher    = {{D}elft {U}niversity of {T}echnology},
  doi          = {10.5281/zenodo.18715223},
  howpublished = {\url{https://github.com/clarkborst/CDRTrainer}},
  url          = {\url{https://github.com/clarkborst/CDRTrainer}},
  note         = {GPL-3 license.}
}
```
---

### Acknowledgements

Part of this work has been conducted within the AI4REALNET (AI for REAL-world 
NETwork operation) project (https://ai4realnet.eu/), which received funding from the European 
Union's Horizon Europe Research and Innovation programme under the Grant 
Agreement No 101119527, and from the Swiss State Secretariat for Education, 
Research and Innovation (SERI). Views and opinions expressed are however those 
of the author(s) only and do not necessarily reflect those of the European Union and SERI. Neither the European Union 
nor the granting authority can be held responsible for them.

