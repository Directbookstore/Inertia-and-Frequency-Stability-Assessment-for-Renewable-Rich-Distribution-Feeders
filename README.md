# Inertia and Frequency Stability Assessment for Renewable-Rich Distribution Feeders

This repository contains the simulation data, automation scripts, and co-simulation workflows used in our research on dynamic frequency stability mitigation in modern power grids. 

## 📚 Associated Publications
If you use this code, data, or methodology, please cite the following papers:

1. **Samuel A. Ibikunle**, Oyeniyi Akeem Alimi, and Evans E. Ojo, *“Inertia and Frequency Stability Assessment for Renewable-Rich Distribution Feeders,”* **Energies**, accepted for publication, 2026.
2. **Samuel A. Ibikunle**, Oyeniyi Akeem Alimi, and Evans E. Ojo, *“Frequency Stability Assessment in Active Distribution Networks: A Comparative Grid Code Analysis and Grid-Forming BESS Mitigation Framework,”* **2026 IEEE PES/IAS PowerAfrica Conference**, accepted, 2026.

### BibTeX Citations
```bibtex
@article{ibikunle2026inertia,
  title={Inertia and Frequency Stability Assessment for Renewable-Rich Distribution Feeders},
  author={Ibikunle, Samuel A. and Alimi, Oyeniyi Akeem and Ojo, Evans E.},
  journal={Energies},
  year={2026},
  note={Accepted for publication}
}

@inproceedings{ibikunle2026frequency,
  title={Frequency Stability Assessment in Active Distribution Networks: A Comparative Grid Code Analysis and Grid-Forming BESS Mitigation Framework},
  author={Ibikunle, Samuel A. and Alimi, Oyeniyi Akeem and Ojo, Evans E.},
  booktitle={Proceedings of the IEEE PES/IAS PowerAfrica Conference},
  year={2026},
  note={Accepted for publication}
}
```

## 🛠️ Software Stack & Prerequisites
To run these notebooks, you need an active installation and local licenses for the following:
* **DIgSILENT PowerFactory** (version 2026 recommended)
* **OpenModelica** (for advanced inverter controller differential equation modeling)
* **Python 3.x** with the following libraries:
  ```bash
  pip install pandas numpy matplotlib pandapower
  ```

## 📂 Repository Structure
* `pf_to_openmodelica_0_100_2MW_workflow_fixed_notebook.ipynb`: Core Jupyter Notebook automating the data bridge and co-simulation exchange between PowerFactory API and OpenModelica.
* `renewable_energy_integration.ipynb`: Automated RMS/EMT frequency assessment scripting.
* `ms-project (4).zip`: Packaged DIgSILENT PowerFactory project files (`.pfd`/`.dz`) containing the active distribution network topologies.
* `data (2).zip`: Pre-processed grid code verification datasets and simulation outputs.

## 🚀 Getting Started
1. Clone this repository to your local machine.
2. Unzip `ms-project (4).zip` and import the project into your local DIgSILENT PowerFactory workspace.
3. Open `pf_to_openmodelica_0_100_2MW_workflow_fixed_notebook.ipynb`.
4. Ensure your local PowerFactory python installation path is appended to your environment variables (`sys.path.append`) so Python can initialize `powerfactory.GetApplication()`.
5. Run the notebook cells sequentially to execute automated grid scenarios.
