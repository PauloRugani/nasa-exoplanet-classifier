# NASA EXOPLANET CLASSIFIER

This project is a part of my group's (MoonMonkeys | Aracaju-SE / Brazil) **[NASA SPACE APPS](https://www.spaceappschallenge.org/2025/find-a-team/moonmonkeys2/?tab=project)** solution to the following problem:
- **A World Away: Hunting for Exoplanets with AI**.



 The solution uses **machine learning** to classify **exoplanets** (planets outside our solar system) based on observational data from NASA satellites. The goal is to determine whether a candidate is a **confirmed planet**, a **false positive**, or requires further investigation.

We implement supervised learning algorithms with the **scikit-learn** library.

---

## Data Used

The data for this project comes from the [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/), specifically:

* [KOI (Kepler Objects of Interest) Table](https://exoplanetarchive.ipac.caltech.edu/cgi-bin/TblView/nph-tblView?app=ExoTbls&config=cumulative): Information about all discovered exoplanets and candidates.
* [TOI (TESS Objects of Interest) Table](https://exoplanetarchive.ipac.caltech.edu/cgi-bin/TblView/nph-tblView?app=ExoTbls&config=TOI): Candidate detections from the **TESS** mission.

These datasets include details such as:

* **Stellar parameters**: Host star brightness, radius, and temperature.
* **Planetary parameters**: Radius, orbital period, mass (when available).
* **Detection metrics**: Signal-to-noise ratio, transit depth, and other observational features.

---

## Project Objective

The goal of this project is to build a model capable of **classifying exoplanet candidates** based on NASA’s observational data.

The model considers variables such as:

* Transit and orbital parameters
* Host star characteristics
* Detection reliability metrics

The classifier is trained and validated using historical datasets with confirmed labels provided by NASA.

---

## Project Structure

The project is organized as follows:

```
├── data/
├── model/
├── notebooks/
├── requirements.txt
└── README.md
```

---

## Requirements

This project was developed and tested with the following dependencies:

* Python 3.8 or higher
* Key libraries:

  * **pandas**: For data manipulation
  * **matplotlib** and **seaborn**: For data visualization
  * **scikit-learn**: For building and evaluating ML models
  * **xgboost**: For building and evaluating ML XGBoost model

### Installation

To install all necessary dependencies, use the following command:

```bash
pip install -r requirements.txt
```

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgements

Special thanks to **NASA Exoplanet Science Institute (NExScI)** for maintaining the [Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/), which provided the datasets used in this project.

---

