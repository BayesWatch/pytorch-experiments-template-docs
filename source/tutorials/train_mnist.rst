========================
Train a network on MNIST
========================

If you haven't already, start by following the :ref:`Setup Instructions`.

A straightforward training run on MNIST can be run with:

.. code-block:: bash
    
    python train.py --experiment_name mnist_example --dataset mnist --num_gpus_to_use 1 --max_epochs 20 --model.type ResNet9


The rest of the hyperparameters will be filled in via the default argparse arguments at the start of the train file:
- the optimiser used will be ``Adam``
- the learning rate will be scheduled with ``CosineAnnealing``
- batch size will be 256
- ... and many other choices to be aware of 
 
If you don't want to rely on all of these defaults, and don't want to have to type out all of the arguments, you can run your experiment from a configuration file. For example, the above configuration could look like the following, put in a ``.yaml`` file in the folder ``experiment_files``:

.. code-block:: yaml

    experiment_name: mnist_example
    dataset: mnist
    num_gpus_to_use: 1
    
    # hyperparameters
    max_epochs: 20

    # model choices
    model.type: ResNet9

And then run: ``python train.py -config experiment_files/mnist_config.yaml``. You can also use ``JSON``.