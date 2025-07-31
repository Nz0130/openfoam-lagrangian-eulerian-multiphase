# openfoam-lagrangian-eulerian-multiphase
Research-driven development of a hybrid Eulerian–Lagrangian multiphase solver with phase change modeling, based on OpenFOAM.
---

### 📄 `README.md`

# openfoam-lagrangian-eulerian-multiphase

🚀 **Research-driven development of a hybrid Eulerian–Lagrangian multiphase solver with phase change modeling**, based on OpenFOAM.


## 🔍 Overview

This project aims to build an open-source CFD solver that couples:

- **Eulerian fluid field** (e.g. water, air)
- **Lagrangian dispersed phase** (e.g. bubbles, droplets, particles)
- **Interphase mass and heat transfer** with **phase change** (evaporation, condensation)
- Future features: cavitation, bubble collapse, and coupling to deformable structures

It is intended as both:
- A scientific contribution to multiphase CFD modeling
- A personal job-oriented portfolio project demonstrating C++, OpenFOAM, and algorithm design skills

---

## 🧱 Solver Architecture

Planned core modules:
- 🔹 `lagrangianEulerFoam` — base solver (modified from `reactingParcelFoam`)
- 🔹 `phaseChangeModel` — custom model for evaporation/condensation
- 🔹 Support for spray-like droplet injection
- 🔹 Future: dynamic mesh / cavitation / FSI

---

## 📁 Folder Structure

```bash
.
├── lagrangianEulerFoam/       # Custom solver source
├── phaseChangeModel/          # Evaporation/condensation model
├── testCases/                 # Minimal working simulations
├── docs/                      # Theory, validation logs, references
├── tutorials/                 # Full simulation setups
└── README.md
````

---

## 🛠️ Build Instructions

> Requires OpenFOAM (v10 or later recommended)

```bash
cd lagrangianEulerFoam
wmake
```

---

## 🔬 Validation Plan

* [ ] Evaporating droplet in quiescent gas
* [ ] Bubble collapse near rigid wall
* [ ] Spray evaporation in cross flow
* [ ] Heat-driven condensation on cold wall

---

## 📚 References

* OpenFOAM Official Documentation
* Hani’s Training Materials: [https://www.tfd.chalmers.se/\~hani/](https://www.tfd.chalmers.se/~hani/)
* Lagrangian–Eulerian OpenFOAM literature (2021–2024)

---

## 📌 License

This project is open-source and licensed under the [GNU General Public License v3.0](LICENSE).

---

## 🙋 Author

**Nz0130** — [GitHub profile](https://github.com/Nz0130)

Feel free to fork, clone, and contribute!

```

---

Let me know if you'd like:
- A custom logo or banner for the top
- The first `wmake`-ready solver skeleton to go with this
- Or a `docs/TODO.md` roadmap with learning tasks!
```
