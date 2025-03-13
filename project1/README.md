# classification using nearest neighbor biomedical data
- Task goal: 
  - The goal is a binary classification problem where we determine whether a patient has an abnormal spinal condition (AB) or a normal spine (NO).
  - Note: the original dataset had more specific labels (Disk Hernia (DH), Spondylolisthesis (SL), Normal (NO), and Abnormal (AB)), but in this case, the task simplifies them into just Normal (0) and Abnormal (1).
---
- Dataset Overview: each patient is described using six biomechanical attributes
  - Independent Variables: Pelvic incidence, Pelvic tilt, Lumbar lordosis angle, Sacral slope, Pelvic radius,Degree of spondylolisthesis (float/int)
  - Dependent varaible: spine condition (binary class)
---
- Model Overview:
  - Framework: sklearn.neighbors.KNeighborsClassifier
    - Method overveiw:
      - Determine Optimal k – Start with a small value of k and increment until the lowest test error is found.
      - Distance Metric – Use Euclidean distance to identify the k nearest neighbors.
      - Decision Rule – Classify using majority voting among the k neighbors.
      - Comparison – Experiment with Minkowski (Manhattan/Chebyshev) and Mahalanobis distances and compare results with Euclidean distance.
     


