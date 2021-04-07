=========================
Installation and Overview
=========================

------------
Installation
------------

In order to use this template, go to the GitHub repository and click the "Use this template" button:

.. image:: resources/use_this_template.png

Then you will want to clone and ``cd`` into your new repository.

Assuming you already have conda available, installing the dependencies of this template should be as easy as:

``conda env create -f environment.yml``

--------
Overview
--------
Since the project is relatively small, we can see a picture of the directories::

  ├── INSTALL.md
  ├── LICENSE
  ├── README.md
  ├── configs
  ├── datasets
  ├── log
  │   ├── dev
  │   │   ├── images
  │   │   │   ├── test
  │   │   │   ├── train
  │   │   │   └── val
  │   │   ├── saved_models
  │   │   └── summary_logs
  │   ├── experiment_ResNet9_cifar10_0_9add9a5.checkpoint
  │   └── snapshots
  │       └── resnet_101_cifar
  │           └── snapshot.tar.gz
  ├── models
  │   ├── __init__.py
  │   ├── auto_builder_models.py
  │   ├── densenet.py
  │   ├── resnet.py
  │   └── wresnet.py
  ├── notebooks
  │   ├── Cifar-10-results.pdf
  │   ├── Cifar-100-results.pdf
  │   ├── plot-results.ipynb
  │   └── utils.py
  ├── test
  │   └── auto_builder_models_test.py
  ├── train.py
  └── utils
      ├── arg_parsing.py
      ├── cinic_utils.py
      ├── custom_transforms.py
      ├── dataset_loading_hub.py
      ├── datasets.py
      ├── gpu_selection_utils.py
      ├── metric_tracking.py
      ├── storage.py
      └── torchsummary.py
