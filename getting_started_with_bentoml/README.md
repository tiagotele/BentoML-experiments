# Experimenting BentoML

## Creating environment to test
```bash
(conda create --name ds_kernel python=3.9 -y) && (conda activate ds_kernel) && (pip install bentoml sklearn)
```

## Getting started with BentoML

Local experiments

### This run is registered at BentoML file structure
```bash
pytho3 create_iris.clf.py
```

### Listing models
```bash
bentoml models list
```

### Building a single Bento
```bash
bentoml build
```

### Building Docker image from Bento
```bash
bentoml containerize iris_classifier:latest
```

### Testing cals to iris model
```bash
curl \
  -X POST \
  -H "content-type: application/json" \
  --data "[[7, 3.2, 4.7, 1.4]]" \
```