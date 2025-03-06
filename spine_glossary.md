# SPINE Glossary (Alphabetically Sorted)

### Module: `/home/bilal/spine_documentation/spine/bin/__init__.py`

Folder with executables.

---
### Module: `/home/bilal/spine_documentation/spine/bin/larcv_check_valid.py`

Mark all bad LArCV ROOT files before merging them with hadd.

---
### Module: `/home/bilal/spine_documentation/spine/bin/larcv_count_entries.py`

Counts the number of events in a LArCV dataset.

---
### Module: `/home/bilal/spine_documentation/spine/bin/larcv_find_duplicates.py`

Finds duplicated files.

---
### Module: `/home/bilal/spine_documentation/spine/bin/larcv_find_run.py`

Builds a list of file which make a data run.

---
### Module: `/home/bilal/spine_documentation/spine/bin/larcv_inject_run_number.py`

Script which injects a run number in every event of every tree in a file or
a list of files.

---
### Module: `/home/bilal/spine_documentation/spine/bin/output_check_valid.py`

Check that all the input files were processed and produced an output with
the expected number of events for each input file.

---
### Module: `/home/bilal/spine_documentation/spine/bin/run.py`

Main driver for training, validation, inference and analysis.

---
### Module: `/home/bilal/spine_documentation/spine/spine/__init__.py`

Top-level module of the SPICE source code.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/__init__.py`

Analysis script module.

This module handles scripts using the output of the reconstruction chain
and the post-processor module to produce analyses. This may include:
    - Reconstruction performance metrics 
    - Topology selection
    - Energy reconstruction quality
    - etc.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/base.py`

Base class of all analysis scripts.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/diag/__init__.py`

Diagnostic analaysis scripts.

This submodule is use to run basic diagnostics analyses such as:
- Track dE/dx profile
- Track energy reconstruction
- Track completeness
- Shower start dE/dx
- ...

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/diag/shower.py`

Module to evaluate diagnostic metrics on showers.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/diag/track.py`

Module to evaluate diagnostic metrics on tracks.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/factories.py`

Construct a analysis script module class from its name.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/manager.py`

Manages the operation of analysis scripts.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/metric/__init__.py`

Reconstruction quality evaluation module.

This submodule is used to evaluate reconstruction quality metrics, such as:
- Semantic segmentation accuracy
- Clustering accuracy
- Flash matching efficiency
- ...

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/metric/cluster.py`

Analysis script used to evaluate the clustering accuracy.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/metric/optical.py`

Analysis script used to evaluate the semantic segmentation accuracy.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/metric/point.py`

Analysis script used to evaluate the point proposal accuracy.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/metric/segment.py`

Analysis script used to evaluate the semantic segmentation accuracy.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/script/__init__.py`

Module with all analysis scripts.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/script/event.py`

Analysis script used to store basic event information into CSV files.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/script/save.py`

Analysis script used to store the reconstruction output to CSV files.

---
### Module: `/home/bilal/spine_documentation/spine/spine/ana/template.py`

Analysis module template.

Use this template as a basis to build your own analysis script. An analysis
script takes the output of the reconstruction and the post-processors and
performs basic selection cuts and store the output to a CSV file.

---
### Module: `/home/bilal/spine_documentation/spine/spine/build/__init__.py`

Module that handles the construction of analysis data classes.

It produces the following classes:
- :class:`RecoFragment`, :class:`TruthFragment`
- :class:`RecoParticle`, :class:`TruthParticle`
- :class:`RecoInteraction`, :class:`TruthInteraction`

It operates two basic functions:
- Build the aforementioned classes based on the ML chain output
- Load the aforementioned classes from an analysis HDF5 file

---
### Module: `/home/bilal/spine_documentation/spine/spine/build/base.py`

Base class for all data representation builders.

---
### Module: `/home/bilal/spine_documentation/spine/spine/build/fragment.py`

Classes in charge of constructing Fragment objects.

---
### Module: `/home/bilal/spine_documentation/spine/spine/build/interaction.py`

Class in charge of constructing Interaction objects.

---
### Module: `/home/bilal/spine_documentation/spine/spine/build/manager.py`

Class to build all require representations.

---
### Module: `/home/bilal/spine_documentation/spine/spine/build/particle.py`

Classes in charge of constructing Particle objects.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/__init__.py`

Module which defines all the data structures used in the package.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/base.py`

Module with a parent class of all data structures.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/batch/__init__.py`

Data structures used to store batched data.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/batch/base.py`

Module with a base class for all batched data structures.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/batch/edge_index.py`

Module with a dataclass targeted at a batched edge index.

An edge index is a sparse representation of a graph incidence matrix.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/batch/index.py`

Module with a dataclass targeted at a batch index or list of indexes.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/batch/tensor.py`

Module with a dataclass targeted at batched matrix/tensors.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/crt.py`

Module with a data class object which represents CRT information.

This copies the internal structure of :class:`larcv.CRTHit`.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/list.py`

Module with a class object which represent object lists.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/meta.py`

Module with a data class object which represents rasterized images metadata.

This copies the internal structure of either :class:`larcv.ImageMeta` for 2D
images or :class:`larcv.Voxel3DMeta` for 3D images.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/neutrino.py`

Module with a data class object which represents true neutrino information.

This copies the internal structure of :class:`larcv.Neutrino`.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/optical.py`

Module with a data class object which represents optical information.

This copies the internal structure of :class:`larcv.Flash`.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/out/__init__.py`

Submodule which defines the local data structures.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/out/base.py`

Module with classes for all reconstructed and true objects.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/out/fragment.py`

Module with a data class objects which represent output fragments.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/out/interaction.py`

Module with a data class objects which represent output interactions.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/out/particle.py`

Module with a data class objects which represent output particles.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/particle.py`

Module with a data class object which represents true particle information.

This copies the internal structure of :class:`larcv.Particle`.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/run_info.py`

Module with a data class object which represents the run information.

It can extract run attributes from any event-level LArCV object.

---
### Module: `/home/bilal/spine_documentation/spine/spine/data/trigger.py`

Module with a data class object which represents trigger information.

This copies the internal structure of :class:`larcv.Trigger`.

---
### Module: `/home/bilal/spine_documentation/spine/spine/driver.py`

SPINE driver class.

Takes care of everything in one centralized place:
- Data loading
- ML model and loss forward pass
- Batch unwrapping
- Representation building
- Post-processing
- Analysis script execution
- Writing output to file

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/__init__.py`

IO module which contains all data read/write tools.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/collate.py`

Contains implementations of data collation classes.

Collate classes are a middleware between parsers and datasets. They are given
to :class:`torch.utils.data.DataLoader` as the `collate_fn` argumement.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/dataset.py`

Contains dataset classes to be used by the model.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/factories.py`

Functions that instantiate IO tools classes from configuration blocks.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/parse/__init__.py`

I/O parsers are used to read data products from a LArCV ROOT file.

Parsers are listed under :mod:`io.dataset.schema` in the configuration.
`schema` is a list of named values. Each name is arbitrary and will be
used as a key to access the output of the parser in a dictionary.

List of existing parsers
------------------------

.. csv-table:: Sparse parsers
    :header: Parser name, Description

    ``sparse2d``, Retrieve sparse tensor input from
    larcv::EventSparseTensor2D object
    ``sparse3d``, Retrieve sparse tensor input from
    larcv::EventSparseTensor3D object
    ``sparse3d_ghost``, Takes semantics tensor and turns its labels into
    ghost labels

.. csv-table:: Cluster parsers
    :header: Parser name, Description

    ``cluster2d``, Retrieve list of sparse tensor input from
    larcv::EventClusterPixel2D
    ``cluster3d``, Retrieve list of sparse tensor input from
    larcv::EventClusterVoxel3D

.. csv-table:: Particle parsers
    :header: Parser name, Description

    ``particle``, Retrieve array of larcv::Particle
    ``neutrino``, Retrieve array of larcv::Neutrino
    ``particle_points``, Retrieve array of larcv::Particle ground truth
    points tensor
    ``particle_coords``, Retrieve array of larcv::Particle coordinates
    (start and end) and start time
    ``particle_graph``, Construct edges between particles (i.e. clusters)
    from larcv::EventParticle
    ``single_particle_pid``, Get a single larcv::Particle PDG code
    ``single_particle_energy``, Get a single larcv::Particle initial
    energy

.. csv-table:: Miscellaneous parsers
    :header: Parser name, Description

    ``meta``, Get the meta information to translate into real world coordinates
    ``run_info``, Parse run info (run, subrun, event number)
    ``flash``, Parse optical flashes
    ``crthit``, Parse cosmic ray tagger hits
    ``trigger``, Parse trigger information


What does a typical parser configuration look like?
---------------------------------------------------
If the configuration looks like this, for example:

..  code-block:: yaml

    schema:
      input_data:
        parser: sparse3d
        sevent_list:
          - sparse3d_reco
          - sparse3d_reco_chi2

Where `input_data` is an arbitrary name chosen by the user, which will be the
key to access the output of the parser `sparse3d`. The parser arguments
can be ROOT TTree names that will be fed to the parser or parser arguments. The
arguments must be passed as a dictionary of (argument name, value) pairs. In
this example, the parser will be called with a list of 2 objects: A
:class:`larcv::EventSparseTensor3D` coming from the ROOT TTree `sparse3d_reco`,
and another one coming from the TTree `sparse3d_reco_chi2`.

How do I know what a parser requires?
-------------------------------------
To be completed.

How do I know what my ROOT file contains?
-----------------------------------------
To be completed.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/parse/base.py`

Contains Parser class which all parsers inherit from.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/parse/clean_data.py`

Module which contains functions used to clean up cluster data.

When loading :class:`larcv.Cluster3DVoxelTensor` objects into tensors,
there can be duplicate voxels. These routines are used to remove these
duplicates and ensure the ordering of the output.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/parse/cluster.py`

Module that contains all parsers related to LArCV cluster data.

Contains the following parsers:
- :class:`Cluster2DParser`
- :class:`Cluster3DParser`
- :class:`Cluster3DAggregateParser`
- :class:`Cluster3DChargeRescaledParser`

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/parse/misc.py`

Module that contains parsers that do not fit in other categories.

Contains the following parsers:
- :class:`Meta2DParser`
- :class:`Meta3DParser`
- :class:`RunInfoParser`
- :class:`OpFlashParser`
- :class:`CRTHitParser`
- :class:`TriggerParser`

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/parse/particle.py`

Module that contains all parsers related to LArCV particle data.

Contains the following parsers:
- :class:`ParticleParser`
- :class:`NeutrinoParser`
- :class:`ParticlePointParser`
- :class:`ParticleCoordinateParser`
- :class:`ParticleGraphParser`
- :class:`ParticlePIDParser`
- :class:`ParticleEnergyParser`

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/parse/sparse.py`

Module that contains all parsers related to LArCV sparse data.

Contains the following parsers:
- :class:`Sparse2DParser`
- :class:`Sparse3DParser`
- :class:`Sparse3DAggregateParser`
- :class:`Sparse3DChargeRescaledParser`
- :class:`Sparse3DGhostParser`

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/read/__init__.py`

Module containing data reader classes.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/read/base.py`

Contains the data reader base class.

Data readers are used to extract specific entries from files and store their
data products into dictionaries to be used downstream.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/read/hdf5.py`

Contains a reader class dedicated to loading data from HDF5 files.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/read/larcv.py`

Contains a reader class dedicated to loading data from LArCV files.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/sample.py`

Used to define which dataset entries to load at each iteration

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/write/__init__.py`

Module containing data writer classes.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/write/csv.py`

Module to write log files to CSV.

---
### Module: `/home/bilal/spine_documentation/spine/spine/io/write/hdf5.py`

Module to write the output of the reconstruction to file.

---
### Module: `/home/bilal/spine_documentation/spine/spine/main.py`

Main functions that call the Driver class.

This is the first module called when launching a binary script under the `bin`
directory. It takes care of setting up the environment and the `Driver`
object(s) used to execute/train ML models, post-processors, analysis
scripts, writers and profilers.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/__init__.py`

Module that handles the construction and executions of ML models.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/full_chain.py`

Module with the core full reconstruction chain.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/graph_spice.py`

Supervi dense clustering model and its loss.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/image.py`

Whole-image classification/regression tasks.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/__init__.py`

Contains reusable layers for various models. Layers are classified into three folders:

* `common` reusable by any models
* `cnn` reusable by CNN-based models
* `cluster` reusable by CNN-based clustering models
* `gnn` reusable by GNN-based models

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cluster/__init__.py`

Module with all methods to build Convolutional Neural Network clusterers.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cluster/factories.py`

Factories to build the CNN-based clustering model components.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cluster/graph_spice_embedder.py`

Feature embedding for pixel supervised connected-component clustering.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cluster/kernel.py`

Edge kernel functions that produce edge weights from node features.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cluster/loss/__init__.py`

Sparse CNN clustering losses.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cluster/loss/lovasz.py`

Lovasz-Softmax and Jaccard hinge loss in PyTorch
Maxim Berman 2018 ESAT-PSI KU Leuven (MIT License)

Original Paper: https://arxiv.org/pdf/1705.08790.pdf
Github: https://github.com/bermanmaxim/LovaszSoftmax

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cnn/act_norm.py`

Functions which initialize activation and normalization layers
used by CNNs. These factories build activations and normalizations layers
are based on the MinkowskiEngine package.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cnn/configuration.py`

Function which sets up the necessary configuration for all CNNs.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cnn/encoder.py`

Defines CNN encoder backbones for image feature extraction.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cnn/nonlinearities.py`

Custom non-linear activation functions.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cnn/normalizations.py`

Custom normalization layers.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/cnn/uresnet_layers.py`

Module with all the backbone components of UResNet.

Contains the following components:
  - `UResNetEncoder`: Encoder component of UResNet
  - `UResNetDecoder`: Decoder component of UResNet
  - `UResNet`: Full encoder/decoder architecture of UResNet

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/common/act_norm.py`

Functions which initialize activation and normalization layers
used generically by torch models. 

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/common/dbscan.py`

Module which does connected-components (dense) clustering using DBSCAN.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/common/evidential.py`

Defines a layer that converts logit output into an evidential output.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/common/final.py`

Defines models that take feature vector developped by a dedicated
feature extractor networks and produces the required type of output.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/common/losses.py`

Module with losses which are not generically provided by `PyTorch`.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/common/metric.py`

Modules used to evaluate model performance.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/common/mlp.py`

Module which defines a very generic multi-layer perceptron with
fully configurable parameters to be used elsewhere.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/factories.py`

Factories to build generic layers components.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/__init__.py`

Module with all methods to build Graph Neural Networks.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/encode/__init__.py`

GNN node and edge encoding module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/encode/cnn.py`

Module which defines encoders using convolutional neural networks.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/encode/empty.py`

Module which defines encoders that produce no features.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/encode/mixed.py`

Module which defines encoders that mix geometric and CNN features together.

See :mod:`spine.model.layer.gnn.encode.geometric` and
:mod:`spine.model.layer.gnn.encode.cnn` for more information.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/factories.py`

Factories to build the GNN model components.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/graph/__init__.py`

GNN input graph construction.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/graph/base.py`

Base class for all graph construction classes.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/graph/bipartite.py`

Bipartite graph constructor for GNNs.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/graph/complete.py`

Complete graph constructor for GNNs.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/graph/delaunay.py`

Delaunay graph constructor for GNNs.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/graph/knn.py`

k Nearest-neighbor (kNN) graph constructor for GNNs.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/graph/loop.py`

Loop graph constructor for GNNs.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/graph/mst.py`

MST graph constructor for GNNs.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/loss/edge_channel.py`

Module that defines an edge classification loss (ON vs OFF).

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/loss/node_class.py`

Module that defines a generic node classification loss.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/loss/node_orient.py`

Module that defines a generic node classification loss.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/loss/node_reg.py`

Module that defines a generic node classification loss.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/loss/node_shower_primary.py`

Module that defines an EM shower primary identification loss.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/loss/node_vertex.py`

Module that defines a vertex identification loss using node predictions.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/model/factories.py`

Module to build GNN message passing submodules.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/model/layer/agnnconv.py`

Module which defines a graph node feature update based on AGNNConv.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/model/layer/econv.py`

Module which defines a graph node feature update based on EdgeConv.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/model/layer/gatconv.py`

Module which defines a graph node feature update based on GATConv.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/model/layer/mlp.py`

Module which defines generic graph features update based on MLPs.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/model/layer/nnconv.py`

Module which defines a graph node feature update based on NNConv.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/layer/gnn/model/meta.py`

Module which contains a generic GNN message passing implementation.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/manager.py`

Centralize all methods associated with a machine-learning model.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/singlep.py`

Image classification module.

This module includes:
    - Single full image classification
    - Individual cluster classification
    - UQ implementations of the full image classification

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/uresnet.py`

UResNet segmentation model and its loss.

---
### Module: `/home/bilal/spine_documentation/spine/spine/model/uresnet_ppn.py`

Module that defines a model and a loss to jointly train the semantic
segmentation task and the point proposal task.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/__init__.py`

Post-processing module.

This module handles post-processors building upon the ouptut of the ML-based
reconstruction chain to produce high-level quantities. This may include:
    - Particle direction reconstruction
    - Range-based energy estimation
    - Optical flash matching
    - Cosmic ray tagger matching
    - etc.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/base.py`

Contains base class of all post-processors.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/crt/matcher.py`

CRT-TPC matcher interface.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/factories.py`

Construct a post-processor module class from its name.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/manager.py`

Manages the operation of post-processors.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/metric/__init__.py`

Reconstruction quality evaluation module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/metric/match.py`

Match objects and their label counterparts and vice versa.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/optical/barycenter.py`

Module that supports barycenter-based flash matching.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/optical/flash_matching.py`

Post-processor in charge of finding matches between charge and light.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/optical/likelihood.py`

Module which supports likelihood-based flash matchin (OpT0Finder).

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/__init__.py`

Reconstruction post-processor modules.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/calo.py`

Calorimetric energy reconstruction module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/cathode_cross.py`

Cathode crossing identification + merging module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/direction.py`

Particle direction reconstruction module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/geometry.py`

Detector-geometry-based reconstruction module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/label.py`

True particle children counting module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/mcs.py`

Multiple-Coulomb scattering (MCS) energy reconstruction module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/pid.py`

Particle identification modules.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/points.py`

Track end point assignment module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/ppn.py`

PPN point construction module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/tracking.py`

Tracking reconstruction modules.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/reco/vertex.py`

Interaction vertex reconstruction module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/template.py`

Post-processor module template.

Use this template as a basis to build your own post-processor. A post-processor
takes the output of the reconstruction and either
- Sets additional reconstruction attributes (e.g. direction estimates)
- Adds entirely new data products (e.g. trigger time)

---
### Module: `/home/bilal/spine_documentation/spine/spine/post/trigger/__init__.py`

Trigger information processing module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/adabound.py`

Local implementations of the AdaBound optimizers.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/augment.py`

Module with methods to augment the input data to SPINE.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/calib/__init__.py`

General calibration module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/calib/database.py`

SQLite calibration database parsing.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/calib/factories.py`

Construct a calibrator class from its name.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/calib/field.py`

Applies field non-uniformity corrections.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/calib/gain.py`

Applies conversion form ADC to number ionization electrons.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/calib/lifetime.py`

Apply electron lifetime corrections.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/calib/manager.py`

Loads all requested calibration modules and executes them
in the appropriate sequence.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/calib/recombination.py`

Applies electron recombination corrections.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/calib/transparency.py`

Apply wire transparency corrections.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/cluster/ccc.py`

Connected component clustering module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/cluster/fragmenter.py`

Classes to process the output of dense clustering algorithms into a set
of fragments.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/cluster/graph.py`

Class and methods to convert the output of Graph-SPICE into a set of
pixel cluster assignments using a graph.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/cluster/orphan.py`

Defines class used to assign orphaned points to a sensible cluster.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/conditional.py`

Module that handles conditional imports for optional packages.

Currently wraps the following packages:
- larcv: only needed when reading larcv-format data in parsers
- MinkowskiEngine: only needed when running sparse CNNs

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/config.py`

Module in charge of loading SPINE configuration files.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/dbscan.py`

Simple wrapper for sklearn's DBSCAN to turn its label output into
a list of clusters in the form of a point index list.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/energy_loss.py`

Module of functions that approximate the energy loss of particles through
matter. It includes function to compute the CSDA KE of particles given their
range and vice-versa.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/enums.py`

Module which contains enumerated variables shared across the project.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/factory.py`

Contains functions needed to instantiate a class from a dictionary.

This allows to generically convert a YAML block into an instatiated class
with all the appropriate checks that the class exists and is provided
with appropriate arguments.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/geo/__init__.py`

Detector geometry module.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/geo/detector/__init__.py`

Module which holds all detector component geometries.

This includes:
- :class:`TPCDetector` for a set of organized TPCs
- :class:`OptDetector` for a set of organized light collection detectors
- :class:`CRTDetector` for a set of organized CRT planes

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/geo/detector/base.py`

Basic detector components shared across multiple subsystems.

This currently handles:
- :class:`Box` which corresponds to box-shaped detector modules.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/geo/detector/crt.py`

CRT detector geometry classes.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/geo/detector/optical.py`

Optical detector geometry classes.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/geo/detector/tpc.py`

TPC detector geometry classes.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/geo/manager.py`

Module with a general-purpose geometry class.

This class supports the storage of:
- TPC boundaries
- Optical detector shape/locations
- CRT detector shape/locations

It also provides a plethora of useful functions to query the geometry.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/ghost.py`

Algorithms associated with the deghosting process.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/globals.py`

Module which contains all global variables shared across the project.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/gnn/cluster.py`

Module with functions that operate on collections of pixels (clusters).

A cluster is typically represented as a list of row indexes pointing at the
voxels that up the cluster out of a tensor of pixels.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/gnn/evaluation.py`

Module used to label or evaluate GNNs.

It contains two classes of functions:
- Functions used in GNN losses
- Functions used to quantify the performance of GNNs

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/gnn/network.py`

Functions used to manipulate a graph of nodes and edges.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/gnn/voxels.py`

Module with functions that operate on single voxels in the context of GNNs.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/inference.py`

Module with helper functions to run inference on a model configuration.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/logger.py`

Simple module which define logging module style and returns it.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/match.py`

Functions to find the best overlaps between point sets.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/metrics.py`

Various metrics used to evaluate clustering.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/numba_local.py`

Extensions to the basic Numba package.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/particles.py`

Particle truth information post-processors.

They add/correct information stored in LArCV particles.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/pid.py`

Module with functions/classes used to identify particle species.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/point_break_clustering.py`

Module with a class that leverages particle endpoints to do clustering.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/ppn.py`

Module which contains utility function to process PPN information.

It contains functions to produce PPN labels and functions to process the
PPN predictions into something human-readable.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/torch_local.py`

Simple local extensions to the current torch package.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/train.py`

Factory to build an optimizer function from a configuration dictionary.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/unwrap.py`

Module with the classes/functions needed to unwrap batched data.

---
### Module: `/home/bilal/spine_documentation/spine/spine/utils/weighting.py`

Module which contains methods to compute class weights.

All methods compute the weights based on the relative abundance of each class.

---
### Module: `/home/bilal/spine_documentation/spine/spine/version.py`

Module which stores the current software version.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/__init__.py`

Module which centralizes all tools used to visualize data.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/box.py`

Defines functions used to draw finite-sized boxes.

These tools are typically used to represent the extent of a voxel or
a voxel neighborhood in an image. In the context of the Point-Proposal Network,
this helps represent the region proposed by the network at layers
deeper than the original resolution of the image.

The :func:`box_trace` function is also used to represent the extent of the
active volume of the modules that make up a detector.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/cluster.py`

Tools to draw voxelized data organized in clusts.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/cone.py`

Module to convert a point cloud into an cone envelope.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/ellipsoid.py`

Module to convert a point cloud into an ellipsoidal envelope.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/evaluation.py`

Routines to produce reconstruction performance metric plots.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/geo.py`

Draw detectors based on their geometry definition.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/hull.py`

Module to convert a point cloud into an convex hull envelope.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/layout.py`

Defines default plotly layouts.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/metric/__init__.py`

Visualization tools dedicated to drawing full chain performance metrics.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/metric/confmat.py`

Visualization tools for confusion matrices.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/network.py`

Tools to draw voxelized data organized in clusts.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/out.py`

Draw reconstruction output-level objects

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/particle.py`

Tools to draw true particles information.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/point.py`

Tools to draw a (labeled) point cloud.

---
### Module: `/home/bilal/spine_documentation/spine/spine/vis/train.py`

Tools to monitor training/validation processes.

---
### Module: `/home/bilal/spine_documentation/spine/test/conftest.py`

Sets up fixtures general to the entire test suite of this package.

This file is read during the collection phase of pytest when running anything
inside this directory.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_io/test_collate.py`

Test that the collate function(s) work as intended.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_io/test_dataset.py`

Test that the dataset classes work as intended.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_io/test_parse/conftest.py`

Fixtures used to text the parsers.

These fixtures generate dummy LArCV data, which is what the parsers expect
to receive as an input.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_io/test_parse/test_cluster.py`

Test that the cluster data parsers work as intended.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_io/test_parse/test_misc.py`

Test that the miscellaneous data parsers work as intended.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_io/test_parse/test_particle.py`

Test that the particle/neutrino data parsers work as intended.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_io/test_parse/test_sparse.py`

Test that the sparse data parsers work as intended.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_io/test_read.py`

Test that the reader classes work as intended.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_io/test_sample.py`

Test that the collate function(s) work as intended.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_io/test_write.py`

Test that the writer classes work as intended.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_loader.py`

Test that the loading of data using a full-fledged configuration.

---
### Module: `/home/bilal/spine_documentation/spine/test/test_utils/test_unwrap.py`

Test that the batch objects can be unwrapped properly.

---
### FunctionDef: `__add__`

Overload the addition operator.

Parameters
----------
time : Time
    Other Time object

Returns
-------
Time
   Summed times

---
### FunctionDef: `__call__`

Append the HDF5 file with the content of a batch.

Parameters
----------
data : dict
    Dictionary of data products
cfg : dict
    Dictionary containing the complete SPINE configuration

---
### FunctionDef: `__call__`

Augment the data products in one event.

Parameters
----------
data : dict
   Data product dictionary

---
### FunctionDef: `__call__`

Build representations for a batch of data.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `__call__`

Build the representations for one entry.

Parameters
----------
data : dict
    Dictionary of input data and model outputs

Notes
-----
Modifies the data dictionary in place.

---
### FunctionDef: `__call__`

Calls the forward (and backward) function on a batch of data.

Parameters
----------
data : dict
    Dictionary of input data product keys which each map to its
    associated batched data product
iteration : int, optional
    Iteration number (relevant for time-dependant losses)

Returns
-------
dict
    Dictionary of model and loss outputs

---
### FunctionDef: `__call__`

Calls the post processor on one entry.

Parameters
----------
data : dict
    Dicitionary of data products
entry : int, optional
    Entry in the batch

Returns
-------
dict
    Update to the input dictionary

---
### FunctionDef: `__call__`

Constructs graphs for all the entries in a batch, one per shape.

Parameters
----------
coords : TensorBatch
    (N, 3) Point coordinates
features : TensorBatch
    (N, N_f) Set of graph embeddings
seg_label : TensorBatch
    (N, 1 + D + 1) Tensor of segmentation labels
    - 1 is the segmentation label
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels
    - N_c is is the number of cluster labels

---
### FunctionDef: `__call__`

Converts the batched raw output of PPN to a discrete set of
proposed points of interest.

Notes
-----
This function works on both wrapped (:class:`TensorBatch`) and
unwrapped (`List[np.ndarray]`) batches of data.

Parameters
----------
ppn_points : Union[TensorBatch, List[np.ndarray]]
     Raw output of PPN
ppn_coords : Union[List[TensorBatch], List[List[np.ndarray]]
     Coordinates of the image at each PPN layer
ppn_masks : Union[List[TensorBatch], List[List[np.ndarray]]
     Predicted masks of at each PPN layer
ppn_classify_endpoints : Union[TensorBatch, List[np.ndarray]], optional
     Raw logits from the end point classification layer of PPN
segmentation : Union[TensorBatch, List[np.ndarray]], optional
     Raw logits from the semantic segmentation network output
ghost : Union[TensorBatch, List[np.ndarray]], optional
     Raw logits from the ghost segmentation network output
entry : int, optional
     Entry in the batch for which to compute the point predictions
selection : Union[IndexBatch, List[np.ndarray]], optional
     List of indexes to consider exclusively (e.g. to get PPN
     predictions within a list of clusters)
**kwargs : dict, optional
     Extraneous outputs not used in this post-processor

Returns
-------
Union[TensorBatch, List[np.ndarray]]
    (N, P) Tensor of predicted points with P divided between
    [batch_id, x, y, z, validity scores (2), occupancy, type scores (5),
     predicted type, endpoint type]

---
### FunctionDef: `__call__`

Evaluate the agreement between each PID template and the particle
track of interest.

Parameters
----------
points : np.ndarray
    (N, 3) Track point coordinates
depositions : np.ndarray
    (N) Deposition values in MeV
end_point : np.ndarray
    (3) Coordinates of the end point of the track
start_point : np.ndarray, optional
    (3) Coordinates of the start point of the track

Returns
-------
int
    Best-fit particle ID
np.ndarray
    (P) One chi2 score per particle species candidate

---
### FunctionDef: `__call__`

Filters input to keep only what is needed to generate a graph.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Tensor of voxel/value pairs
clusts : IndexBatch
    (C) Cluster indexes
classes : TensorBatch, optional
    (C) List of cluster semantic class used to define the max length
groups : TensorBatch, optional
    (C) List of cluster groups which should not be mixed

Returns
-------
np.ndarray
    (2, E) Tensor of edges

---
### FunctionDef: `__call__`

Loop over the list of batch entries and semantic classes and
label points use connected-component clustering.

Parameters
----------
node_coords : TensorBatch
    (N, 3) Set of point coordinates
edge_index : TensorBatch
    (E, 2) Set of edge source and target indices
edge_assn : TensorBatch
    (E) Boolean assignment for each edge (0 for off, 1 for on)
node_clusts : List[List[List[int]]]
    (B, S) One list of node indices per (batch ID, shape) pair
edge_clusts : List[List[List[int]]]
    (B, S) One list of edge indices per (batch ID, shape) pair
min_size : int, optional
    Override the minimum cluster size set in the configuration

Returns
-------
TensorBatch
    (N) Cluster assignments for each of the points in the input

---
### FunctionDef: `__call__`

Main calibration driver.

Parameters
----------
points : np.ndarray, optional
    (N, 3) array of space point coordinates
values : np.ndarray
    (N) array of depositions in ADC
sources : np.ndarray, optional
    (N) array of [cryo, tpc] specifying which TPC produced each hit. If
    not specified, uses the closest TPC as calibration reference.
run_id : int, optional
    ID of the run to get the calibration for. This is needed when using
    a database of corrections organized by run.
track : bool, defaut `False`
    Whether the object is a track or not. If it is, the track gets
    segmented to evaluate local dE/dx and track angle.
meta : Meta, optional
    If provided, use to convert the coordinates from image pixel
    coordinates to detector coordinates
module_id : int, optional
    If provided, shift points to the requested module assuming that the
    points currently live in module ID 0

Returns
-------
np.ndarray
    (N) array of calibrated depositions in ADC, e- or MeV

---
### FunctionDef: `__call__`

Main unwrapping function.

Loops over the data keys and applies the unwrapping rules. Returns the
unwrapped versions of the dictionary

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
dict
    Dictionary of unwrapped data products

---
### FunctionDef: `__call__`

Move an image around within the the pre-defined volume.

Parameters
----------
data : dict
    Dictionary of data products to offset
meta : Meta
    Shared image metadata
keys : List[str]
    List of keys with coordinates to offset

Returns
-------
np.ndarray
    (N, 3) Translated points

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Parse one entry.

This is a place-holder, must be defined in inheriting class.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

---
### FunctionDef: `__call__`

Pass one batch of data through the analysis scripts

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `__call__`

Pass one batch of data through the post-processors.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `__call__`

Place-holder for a function which assigns labels to orphan points.

Parameters
----------
X : np.ndarray
    (N, 3) Coordinates of the points in the image
y : np.ndarray
    (N) Labels of the points (-1 if orphaned)

Returns
-------
np.ndarray
    (M) Labels assigned to each of the orphans

---
### FunctionDef: `__call__`

Produce instance clusters using the point-enhanced method.

Parameters
----------
voxels : np.ndarray
    (N, 3) Set of voxel coordinates
points : np.ndarray
    (P, 3) Set of particle end points
method : str, optional
    Override the method defined in the initialzer

Returns
-------
np.ndarray
    (N) Array of cluster assignments for each voxel in the input

---
### FunctionDef: `__call__`

Return the formatted label string.

*x* and *pos* are passed to `str.format` as keyword arguments
with those exact names.

---
### FunctionDef: `__call__`

Runs the analysis script on one entry.

Parameters
----------
data : dict
    Data dictionary for one entry

Returns
-------
dict
    Update to the input dictionary

---
### FunctionDef: `__call__`

Takes a list of parsed information, one per event in a batch, and
collates them into a single object per entry in the batch.

Parameters
----------
batch : List[Dict]
    List of dictionaries of parsed information, one per event. Each
    dictionary matches one data key to one event-worth of parsed data.

Returns
-------
Dict
    Dictionary that matches one data key to one batch-worth of data

Notes
-----
Assumptions:
- The input batch is a tuple of length >= 1. Length 0 tuple
  will fail (IndexError)
- The dictionaries in the input batch tuple are assumed to have
  an identical list of keys

---
### FunctionDef: `__eq__`

Checks that all attributes of two class instances are the same.

This overloads the default dataclass `__eq__` method to include an
appopriate check for vector (numpy) attributes.

Parameters
----------
other : obj
    Other instance of the same object class

Returns
-------
bool
    `True` if all attributes of both objects are identical

---
### FunctionDef: `__eq__`

Checks that all attributes of two class instances are the same.

This overloads the default dataclass `__eq__` method to include an
appopriate check for vector (numpy) attributes.

Parameters
----------
other : obj
    Other instance of the same object class

Returns
-------
bool
    `True` if all attributes of both objects are identical

---
### FunctionDef: `__eq__`

Overload the equality operator.

Parameters
----------
time : Time
    Other Time object

Returns
-------
bool
    True if both times are identical

---
### FunctionDef: `__getitem__`

Mirrors the `query` function.

Parameters
----------
run_id : int
    ID of the run to get the values for

Returns
-------
np.ndarray
    List of values per channel

---
### FunctionDef: `__getitem__`

Returns a specific entry in the file.

Parameters
----------
idx : int
    Integer entry ID to access

Returns
-------
dict
    One entry-worth of data from the loaded files

---
### FunctionDef: `__getitem__`

Returns a subset of the index corresponding to one entry.

Parameters
----------
batch_id : int
    Entry index

---
### FunctionDef: `__getitem__`

Returns a subset of the index corresponding to one entry.

Parameters
----------
batch_id : int
    Entry index

---
### FunctionDef: `__getitem__`

Returns a subset of the tensor corresponding to one entry.

Parameters
----------
batch_id : int
    Entry index

---
### FunctionDef: `__getitem__`

Returns an underlying TPC of index idx.

Parameters
----------
idx : int
    Index of the TPC within the module

Returns
-------
Chamber
    Chamber object

---
### FunctionDef: `__getitem__`

Returns an underlying module or TPC, depending on the index type.

If the index is specified as a simple integer, a module is returned. If
the index is specified with two integers, a specific chamber within a
module is returned instead.

Parameters
----------
idx : Uniont[int, List[int]]
    Module index or pair of [module ID, chamber ID]

Returns
-------
Union[Module, Chamber]
    Module or Chamber object

---
### FunctionDef: `__getitem__`

Returns one element of the dataset.

Parameters
----------
idx : int
    Index of the dataset entry to load

Returns
-------
dict
    Dictionary of data product names and their associated data

---
### FunctionDef: `__init__`

Check and store the values passed to the initializer,
set the seeds appropriately.

Parameters
----------
dataset : torch.utils.data.Dataset
    Dataset to sampler from
batch_size : int
    Number of samples to load per iteration
seed : int, optional
    Seed to use for random sampling
drop_last: bool, default True
    If `True`, drop the last batch to make the number of entries a
    multiple of the batch_size (if needed)

---
### FunctionDef: `__init__`

Constructor

Parameters
==========
cfg: dict
    The full chain config.

Methods
=======
TODO INSERT

---
### FunctionDef: `__init__`

Convert a basic sampler to an instance of a distributed sampler.

Parameters
----------
sampler : Sampler
    Input torch sampler
num_replicas : int
    Number of distributed samplers running concurrently
rank : int
    Rank of the current sampler

Notes
-----
Input sampler is assumed to be of constant size.

---
### FunctionDef: `__init__`

Give default values to the underlying class attributes.

---
### FunctionDef: `__init__`

Given a path to a calibration data base, load the information
into a dictionary.

Parameters
----------
db_path : str
    Path to a SQLite database
num_tpcs : int
    Expected number of TPCs
db_type : str, default 'value'
    Type of database (One 'value' or one 'map per TPC)
value_key : str, default 'scale'
    Name of the quantity to load for each bin when using 'map' db_type

Returns
-------
dict
    Dictionary which maps a run onto a set of values (one per TPC)

Notes
-----
This makes assumptions about how the database is structured for
ICARUS calibration for now as of the time of implementation.

---
### FunctionDef: `__init__`

Initalize the HDF5 file reader.

Parameters
----------
file_keys : list
    List of paths to the HDF5 files to be read
limit_num_files : int, optional
    Integer limiting number of files to be taken per data directory
max_print_files : int, default 10
    Maximum number of loaded file names to be printed
n_entry : int, optional
    Maximum number of entries to load
n_skip : int, optional
    Number of entries to skip at the beginning
entry_list : list
    List of integer entry IDs to add to the index
skip_entry_list : list
    List of integer entry IDs to skip from the index
run_event_list: list((int, int, int)), optional
    List of (run, subrun, event) triplets to add to the index
skip_run_event_list: list((int, int, int)), optional
    List of (run, subrun, event) triplets to skip from the index
create_run_map : bool, default False
    Initialize a map between (run, subrun, event) triplets and entries.
    For large files, this can be quite expensive (must load every entry).
build_classes : bool, default True
    If the stored object is a class, build it back
skip_unknown_attrs : bool, default False
    If `True`, allow a loaded object to have unrecognized attributes.
    This allows backward compatibility with old files, but use with
    extreme caution, as this might hide a fundamental issue with your code.
run_info_key : str, default 'run_info'
    Name of the data product which contains the run info of the event
allow_missing : bool, default False
    If `True`, allows missing entries in the entry or event list

---
### FunctionDef: `__init__`

Initalize the barycenter flash matcher.

Parameters
----------
match_method: str, default 'distance'
    Matching method (one of 'threshold' or 'best')
    - 'threshold': If the two barycenters are within some distance, match
    - 'best': For each flash, pick the best matched interaction
dimensions: list, default [1, 2]
    Dimensions involved in the distance computation
charge_weighted : bool, default False
    Use interaction pixel charge information to weight the centroid
time_window : List, optional
    List of [min, max] values of optical flash times to consider
first_flash_only : bool, default False
    Only try to match the first flash in the time window
min_inter_size : int, optional
    Minimum number of voxel in an interaction to consider it
min_flash_pe : float, optional
    Minimum number of total PE in a flash to consider it
match_distance : float, optional
    If a threshold is used, specifies the acceptable distance

---
### FunctionDef: `__init__`

Initalize the basic private stopwatch attributes.

---
### FunctionDef: `__init__`

Initialize attention mask.

Parameters
----------
score_threshold : float, default 0.5
    Score above which a voxel is considered positive

---
### FunctionDef: `__init__`

Initialize default anlysis script object properties.

Parameters
----------
obj_type : Union[str, List[str]]
    Name or list of names of the object types to process
run_mode : str, optional
    If specified, tells whether the analysis script must run on
    reconstructed ('reco'), true ('true') or both objects
    ('both' or 'all')
truth_point_mode : str, optional
    If specified, tells which attribute of the :class:`TruthFragment`,
    :class:`TruthParticle` or :class:`TruthInteraction` object to use
    to fetch its point coordinates
append : bool, default False
    If True, appends existing CSV files instead of creating new ones
overwrite : bool, default False
    If True and an output CSV file exists, overwrite it
log_dir : str
    Output CSV file directory (shared with driver log)
prefix : str, default None
    Name to prefix every output CSV file with

---
### FunctionDef: `__init__`

Initialize default post-processor object properties.

Parameters
----------
obj_type : Union[str, List[str]]
    Name or list of names of the object types to process
run_mode : str, optional
    If specified, tells whether the post-processor must run on
    reconstructed ('reco'), true ('true') or both objects
    ('both' or 'all')
truth_point_mode : str, optional
    If specified, tells which attribute of the :class:`TruthFragment`,
    :class:`TruthParticle` or :class:`TruthInteraction` object to use
    to fetch its point coordinates
truth_dep_mode : str, optional
    If specified, tells which attribute of the :class:`TruthFragment`,
    :class:`TruthParticle` or :class:`TruthInteraction` object to use
    to fetch its depositions
parent_path : str, optional
    Path to the parent directory of the main analysis configuration. This
    allows for the use of relative paths in the post-processors.

---
### FunctionDef: `__init__`

Initialize the ASPP block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
dimension : int, default 3
    Dimension of the input image
dilations : list, default [2, 4, 6, 8, 12]
    Dilation rates for atrous convolutions
width : int, default 5
    Width of atrous convolutions

---
### FunctionDef: `__init__`

Initialize the AdaBound optimizer

Parameters
----------
params : iterable
    Iiterable of parameters to optimize or dicts defining
    parameter groups
lr : float, default 1e-3
    Adam learning rate
betas : Tuple[float, float], default (0.9, 0.999)
    Coefficients used for computing running averages of gradient and
    its square
final_lr : float, default 0.1
    Final (SGD) learning rate
gamma : float, default 1e-3
    Convergence speed of the bound functions
eps : float, default 1e-8
    Term added to the denominator to improve numerical stability
weight_decay : float, default 0.
    Weight decay (L2 penalty)
amsbound : bool, default False
    If `True`, use the AMSBound variant of this algorithm

---
### FunctionDef: `__init__`

Initialize the AtrousII block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
dimension : int, default 3
    Dimension of the input image
activation : union[str, dict], default 'relu'
    activation function configuration
normalization : union[str, dict], default 'batch_norm'
    normalization function configuration

---
### FunctionDef: `__init__`

Initialize the CRT/TPC matching post-processor.

Parameters
----------
crthit_key : str
    Data product key which provides the CRT information
**kwargs : dict
    Keyword arguments to pass to the CRT-TPC matching algorithm

---
### FunctionDef: `__init__`

Initialize the CSV event logging class.

Parameters
----------
**kwargs : dict, optional
    Parameters to pass to :class:`AnaBase`

---
### FunctionDef: `__init__`

Initialize the CSV logging class.

If any of the `fragments`, `particles` or `interactions` are specified
as lists of strings, it will be used to restrict the list of
object attributes which get stored to CSV.

Parameters
----------
obj_type : Union[str, List[str]], default ['particle', 'interaction']
    Objects to build files from
fragment : List[str], optional
    List of fragment attributes to store
particle : List[str], optional
    List of particle attributes to store
interaction : List[str], optional
    List of interaction attributes to store
lengths : Dict[str, int], optional
    Lengths to use for variable-length object attributes
match_mode : str, default 'both'
    If reconstructed and truth are available, specified which matching
    direction(s) should be saved to the log file.
**kwargs : dict, optional
    Additional arguments to pass to :class:`AnaBase`

---
### FunctionDef: `__init__`

Initialize the Cascaded Atrous Convolution block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
dimension : int, default 3
    Dimension of the input image
depth : int, default 1
    Number of atrous convolutions layers
dilations : list, default [1, 2, 4, 8, 16, 32]
    Dilation rates for atrous convolutions
activation : union[str, dict], default 'relu'
    activation function configuration

---
### FunctionDef: `__init__`

Initialize the DBSCAN clustering algorithm.

Parameters
----------
eps : float, default 1.8
    The maximum distance between two samples for one to be considered
    as in the neighborhood of the other.
min_samples : int, default 1
    The number of samples (or total weight) in a neighborhood for a
    point to be considered as a core point.
min_size : int, default 3
    Minimum cluster size to stored in the final list of DBSCAN clusters
metric : str, default 'euclidean'
    Metric used to compute the pair-wise distances between space points
shapes : List[int], default [0, 1, 2, 3]
    List of semantic classes to run DBSCAN on
break_shapes : List[int], default [1]
    List of semantic shapes for which to use PPN to break down
break_mask_radius : str, default 5.0
    If using particle points to break up instances further, specifies
    the radius around each particle point which gets masked
break_track_method : str, default 'masked_dbscan'
    If using particle points to break up tracks, specifies the method
use_label_break_points : bool, default False
    Whether to use label points to break instances
track_include_delta : bool, default False
    If `True`, include delta points along with track point when
    running DBSCAN on track points (limits artificial track breaks)
ppn_predictor : cfg, optional
    PPN post-processing configuration

---
### FunctionDef: `__init__`

Initialize the EM shower primary identification loss function.

Parameters
----------
loss : str, default 'ce'
    Name of the loss function to apply
balance_loss : bool, default False
    Whether to weight the loss to account for class imbalance
high_purity : bool, default False
    Only apply loss to nodes which belong to a sensible group, i.e.
    one with exactly one primary in it (not 0, not > 1)
use_closest : bool, default False
    For each group, pick the fragment which is closest to the start
    point of the shower as the primary (more robust to fragment breaks)
use_group_pred : bool, default False
    Use predicted group to check for high purity
group_pred_alg : str, default 'score'
    Method used to form a predicted group ('threshold' or 'score')

---
### FunctionDef: `__init__`

Initialize the GrapPA loss function.

Parameters
----------
grappa_loss : dict
    Loss configuration
grappa : dict, optional
    Model configuration

---
### FunctionDef: `__init__`

Initialize the GrapPA model.

Parameters
----------
grappa : dict
    Model configuration
grappa_loss : dict, optional
    Loss configuration

---
### FunctionDef: `__init__`

Initialize the Graph-SPICE model.

Parameters
----------
graph_spice : dict
    Graph-SPICE configuration dictionary
graph_spice_loss : dict, optional
    Graph-SPICE loss configuration dictionary

---
### FunctionDef: `__init__`

Initialize the LArCV file reader.

Parameters
----------
file_keys : list
    List of paths to the HDF5 files to be read
tree_keys : List[str]
    List of data keys to load from the LArCV files
limit_num_files : int, optional
    Integer limiting number of files to be taken per data directory
max_print_files : int, default 10
    Maximum number of loaded file names to be printed
n_entry : int, optional
    Maximum number of entries to load
n_skip : int, optional
    Number of entries to skip at the beginning
entry_list : list
    List of integer entry IDs to add to the index
skip_entry_list : list
    List of integer entry IDs to skip from the index
run_event_list: list((int, int, int)), optional
    List of (run, subrun, event) triplets to add to the index
skip_run_event_list: list((int, int, int)), optional
    List of (run, subrun, event) triplets to skip from the index
create_run_map : bool, default False
    Initialize a map between (run, subrun, event) triplets and entries.
    For large files, this can be quite expensive (must load every entry).
run_info_key : str, optional
    Key of the tree in the file to get the run information from
allow_missing : bool, default False
    If `True`, allows missing entries in the entry or event list

---
### FunctionDef: `__init__`

Initialize the MBConv block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
expand_ratio : int, default 2
    Multiplicative factor to apply to the input number of features
dimension : int, default 3
    Dimension of the input image
dilation : int, default 1
    Convolution kernel dilation
kernel_size : int, default 3
    Convolution kernel size
stride : int, default 1
    Convolution kernel stride
activation : union[str, dict], default 'relu'
    activation function configuration
normalization : union[str, dict], default 'batch_norm'
    normalization function configuration
bias : bool, default False
    Whether to add a bias term to the kernel

---
### FunctionDef: `__init__`

Initialize the MBResConv block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
expand_ratio : int, default 2
    Multiplicative factor to apply to the input number of features
dimension : int, default 3
    Dimension of the input image
dilation : int, default 1
    Convolution kernel dilation
kernel_size : int, default 3
    Convolution kernel size
stride : int, default 1
    Convolution kernel stride
activation : union[str, dict], default 'relu'
    activation function configuration
normalization : union[str, dict], default 'batch_norm'
    normalization function configuration
bias : bool, default False
    Whether to add a bias term to the kernel

---
### FunctionDef: `__init__`

Initialize the MBResConvSE block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
se_ratio : int, default 8
    Squeezing ratio
expand_ratio : int, default 2
    Multiplicative factor to apply to the input number of features
dimension : int, default 3
    Dimension of the input image
dilation : int, default 1
    Convolution kernel dilation
kernel_size : int, default 3
    Convolution kernel size
stride : int, default 1
    Convolution kernel stride
activation : union[str, dict], default 'relu'
    activation function configuration
normalization : union[str, dict], default 'batch_norm'
    normalization function configuration
bias : bool, default False
    Whether to add a bias term to the kernel

---
### FunctionDef: `__init__`

Initialize the MLP which is used to update the edge features.

Parameters
----------
edge_in : int
    Number of input edge features
node_in : int
    Number of input node features
glob_in : int
    Number of input global features for the graph
mlp : dict
    Configuration of the edge update MLP

---
### FunctionDef: `__init__`

Initialize the MLP which is used to update the edge features.

Parameters
----------
glob_in : int
    Number of input global features for the graph
node_in : int
    Number of input node features
mlp : dict
    Configuration of the global representation update MLP
reduction : str, default 'mean'
    Message feature aggregation function

---
### FunctionDef: `__init__`

Initialize the MLP.

Parameters
----------
in_channels : int
    Number of input features
depth : int
    Number of hidden layers
width : Union[int, List[int]]
    Number of neurons in each hidden layer
activation : Union[str, dict]
    Activation function configuration
normalization : Union[str, dict]
    Normalization function configuration

---
### FunctionDef: `__init__`

Initialize the MLPs which are used to update the node features.

Parameters
----------
node_in : int
    Number of input node features
edge_in : int
    Number of input edge features
glob_in : int
    Number of input global features for the graph
activation : Union[str, dict], default 'relu'
    Activation function configuration
normalization : Union[str, dict], default 'batch_norm'
    Normalization function configuration
**kwargs : dict
    Extra parameters to be passed to the AGNNConv layer

---
### FunctionDef: `__init__`

Initialize the MLPs which are used to update the node features.

Parameters
----------
node_in : int
    Number of input node features
edge_in : int
    Number of input edge features
glob_in : int
    Number of input global features for the graph
message_mlp : dict
    Configuration of the message creation MLP
aggr_mlp : dict
    Configuration of the message aggregtion MLP
reduction : str, default 'mean'
    Message feature aggregation function
attention : bool, default False
    Whether or not to learn explicit attention to particular messages

---
### FunctionDef: `__init__`

Initialize the MLPs which are used to update the node features.

Parameters
----------
node_in : int
    Number of input node features
edge_in : int
    Number of input edge features
glob_in : int
    Number of input global features for the graph
mlp : dict
    Configuration of the node update MLP
aggr : str, default 'max'
    Node feature aggregation method
**kwargs : dict
    Extra parameters to be passed to the EdgeConv layer

---
### FunctionDef: `__init__`

Initialize the MLPs which are used to update the node features.

Parameters
----------
node_in : int
    Number of input node features
edge_in : int
    Number of input edge features
glob_in : int
    Number of input global features for the graph
out_channels : int
    Number of output node features
activation : Union[str, dict], default 'relu'
    Activation function configuration
normalization : Union[str, dict], default 'batch_norm'
    Normalization function configuration
**kwargs : dict
    Extra parameters to be passed to the GATConv layer

---
### FunctionDef: `__init__`

Initialize the MLPs which are used to update the node features.

Parameters
----------
node_in : int
    Number of input node features
edge_in : int
    Number of input edge features
glob_in : int
    Number of input global features for the graph
out_channels : int
    Number of output node features
mlp : dict
    Configuration of the node update MLP
aggr : str, default 'add'
    Node feature aggregation method
**kwargs : dict
    Extra parameters to be passed to the NNConv layer

---
### FunctionDef: `__init__`

Initialize the PPN post-processor.

Parameters
----------
score_threshold : float, default 0.5
     Score above which a point is considered to be active
type_score_threshold : float, default 0.5
     Score above which a type prediction must be to be considered
type_dist_threshold : float, default 1.999
     Distance threshold for matching with semantic type predictions
pool_score_fn : str, default 'max'
     Which operation to use to pool PPN points scores ('max' or 'mean')
pool_dist : float, default 1.999
     Distance below which PPN points should be merged into one (DBSCAN)
enforce_type : bool, default True
     Whether to force PPN points predicted of type X to be within N
     voxels of a voxel with same predicted semantic type
classes : List[int], default [0, 1, 2, 3]
     Number of semantic classes
apply_deghosting : bool, default False
     Whether to deghost the input, if a `ghost` tensor is provided

---
### FunctionDef: `__init__`

Initialize the ResNeXt block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
dimension : int, default 3
    Dimension of the input image
cardinality : int, default 4
    Number of different paths, see ResNeXt paper
depth : int, default 1
    Number of (convolutions + normalization + activation) layers
dilations : int, optional
    Dilation rates for each convolution layer inside the cardinal paths
kernel_sizes : int, default 3
    Kernel sizes for each convolution layer inside the cardinal paths
strides : int, default 1
    Strides for each convolution layer inside the carndinal paths
activation : union[str, dict], default 'relu'
    activation function configuration
normalization : union[str, dict], default 'batch_norm'
    normalization function configuration

---
### FunctionDef: `__init__`

Initialize the ResNet block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
stride : int, default 1
    Convolution kernel stride
dilation : int, default 1
    Convolution kernel dilation
dimension : int, default 3
    Dimension of the input image
activation : union[str, dict], default 'relu'
    activation function configuration
normalization : union[str, dict], default 'batch_norm'
    normalization function configuration
bias : bool, default False
    Whether to add a bias term to the kernel

---
### FunctionDef: `__init__`

Initialize the SE block.

Parameters
----------
channel : int
    Number of input features
ratio : int, default 8
    Squeezing ratio
dimension : int, default 3
    Dimension of the input image

---
### FunctionDef: `__init__`

Initialize the SEResNet block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
se_ratio : int, default 8
    Squeezing ratio
stride : int, default 1
    Convolution kernel stride
dilation : int, default 1
    Convolution kernel dilation
dimension : int, default 3
    Dimension of the input image
activation : union[str, dict], default 'relu'
    activation function configuration
normalization : union[str, dict], default 'batch_norm'
    normalization function configuration

---
### FunctionDef: `__init__`

Initialize the SPP block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
kernel_sizes : int, optional
    Kernel sizes for each pooling operation
dilations : int, optional
    Dilation rates for atrous convolutions. Note that
    `kernel_size == stride` for an SPP layer.
mode : str, default 'avg'
    Pooling mode (one of 'avg', 'max' and 'sum'
dimension : int, default 3
    Dimension of the input image

---
### FunctionDef: `__init__`

Initialize the TPC object.

Parameters
----------
position : np.ndarray
    (3) Position of the center of the TPC
dimensions : np.ndarray
    (3) Dimension of the TPC
drift_dir : np.ndarray
    (3) Drift direction vector

---
### FunctionDef: `__init__`

Initialize the UResNet backbone.

Parameters
----------
cfg : dict
    Decoder configuration block

---
### FunctionDef: `__init__`

Initialize the UResNet+PPN model loss.

Parameters
----------
uresnet : dict
    UResNet configuration dictionary
ppn : dict
    PPN configuration dictionary
uresnet_loss : dict, optional
    UResNet loss configuration
ppn_loss : dict, optional
    PPN loss configuration

---
### FunctionDef: `__init__`

Initialize the UResNet+PPN model.

Parameters
----------
uresnet : dict
    UResNet configuration dictionary
ppn : dict
    PPN configuration dictionary
uresnet_loss : dict, optional
    UResNet loss configuration
ppn_loss : dict, optional
    PPN loss configuration

---
### FunctionDef: `__init__`

Initialize the analysis manager.

Parameters
----------
cfg : dict
    Analysis script configurations
log_dir : str
    Output CSV file directory (shared with driver log)
prefix : str, optional
    Input file prefix. If requested, it will be used to prefix
    all the output CSV files.

---
### FunctionDef: `__init__`

Initialize the analysis script.

Parameters
----------
arg0 : type
    Description of arg0
arg1 : type
    Description of arg1
obj_type : Union[str, List[str]]
    Name or list of names of the object types to process
run_mode : str, optional
    If specified, tells whether the analysis script must run on
    reconstructed ('reco'), true ('true') or both objects
    ('both' or 'all')
append_file : bool, default False
    If True, appends existing CSV files instead of creating new ones
overwrite_file : bool, default False
    If True and the output CSV file exists, overwrite it
output_prefix : str, default None
    Name to prefix every output CSV file with

---
### FunctionDef: `__init__`

Initialize the analysis script.

Parameters
----------
num_classes : int, default 4
    Number of pixel classses, excluding the ghost class
label_key : str, default 'seg_label'
    Name of the tensor which contains the segmentation labels
endpoints : bool, default False
    Evaluate the accuracy of end point classification
**kwargs : dict, optional
    Additional arguments to pass to :class:`AnaBase`

---
### FunctionDef: `__init__`

Initialize the analysis script.

Parameters
----------
obj_type : Union[str, List[str]], optional
    Name or list of names of the object types to process
use_objects : bool, default False
    If `True`, rebuild the clustering assignments for truth and reco
    from the set of truth and reco particles
per_object : bool, default True
    Evaluate the clustering accuracy for each object type (not relevant
    if running GrapPA standalone)
per_shape : bool, default True
    Evaluate the clustering accuracy for each object shape (not
    relevant in the case of interactions)
metrics : Tuple[str], default ('pur', 'eff', 'ari')
    List of clustering metrics to evaluate
label_key : str, default 'clust_label_adapt'
    Name of the tensor which contains the cluster labels, when
    using the raw reconstruction output
label_col : str, optional
    Column name in the label tensor specifying the aggregation label_col
**kwargs : dict, optional
    Additional arguments to pass to :class:`AnaBase`

---
### FunctionDef: `__init__`

Initialize the analysis script.

Parameters
----------
radius : Union[float, List[float]]
    Radius around the start point for which evaluate dE/dx
**kwargs : dict, optional
    Additional arguments to pass to :class:`AnaBase`

---
### FunctionDef: `__init__`

Initialize the analysis script.

Parameters
----------
summary : bool, default True
    If `True`, summarize the confusion matrix for each entry. If
    `False`, store one row per pixel in the image (extremely memory
    intensive but gives details about pixel scores).
num_classes : int, default 5
    Number of pixel classses, excluding the ghost class
ghost : bool, default False
    Evaluate deghosting performance
use_fragments : bool, default False
    If `True`, rebuild the segmentation for truth and reco from the
    shape of truth and reco fragments. This method is exact, as long as
    there is no ghost points and the cluster label tensor is untouched.
    If the label tensor is adapted, the original fragment boundaries are
    lost.
use_particles : bool, default False
    If `True`, rebuild the segmentation for truth and reco from the
    shape of truth and reco particles. This method is imperfect, as the
    shape of showers is determined by the primary shape, which may not
    match the secondary fragment shapes in the original segmentation.
    This method is not compatible with ghost points.
label_key : str, default 'seg_label'
    Name of the tensor which contains the segmentation labels
**kwargs : dict, optional
    Additional arguments to pass to :class:`AnaBase`

---
### FunctionDef: `__init__`

Initialize the analysis script.

Parameters
----------
time_window : List[float]
    Time window within which to include particle (only works for `truth`)
**kwargs : dict, optional
    Additional arguments to pass to :class:`AnaBase`

---
### FunctionDef: `__init__`

Initialize the analysis script.

Parameters
----------
time_window : List[float], optional
    Time window (in ns) for which interactions must have matched flash
neutrino_only : bool, default False
    If `True`, only check if neutrino in-time activity is matched for
    the efficiency measurement (as opposed to any in-time activity)
max_num_flashes : int
    Maximum number of flash matches to store
match_mode : str, default 'both'
    If reconstructed and truth are available, specified which matching
    direction(s) should be saved to the log file.
**kwargs : dict, optional
    Additional arguments to pass to :class:`AnaBase`

---
### FunctionDef: `__init__`

Initialize the attributes of the class.

If the edge index corresponds to an undirected graph, each edge
should have its reciprocal edge immediately after, e.g.

.. code-block:: python

    [[0,1,0,2,0,3,...],
     [1,0,2,0,3,0,...]]

Parameters
----------
data : Union[np.ndarray, torch.Tensor]
    (2, E) Batched edge index
counts : Union[List[int], np.ndarray, torch.Tensor]
    (B) Number of index elements per entry in the batch
offsets : Union[List[int], np.ndarray, torch.Tensor]
    (B) Offsets between successive indexes in the batch
directed : bool
    Whether the edge index is directed or undirected

---
### FunctionDef: `__init__`

Initialize the attributes of the class.

Parameters
----------
data : Union[np.ndarray, torch.Tensor, 
             List[Union[np.ndarray, torch.Tensor]]]
    Simple batched index or list of indexes
offsets : Union[List[int], np.ndarray, torch.Tensor]
    (B) Offsets between successive indexes in the batch
counts : Union[List[int], np.ndarray, torch.Tensor], optional
    (B) Number of indexes in the batch
single_counts : Union[List[int], np.ndarray, torch.Tensor], optional
    (I) Number of index elements per index in the index list. This
    is the same as counts if the underlying data is a single index
batch_ids : Union[List[int], np.ndarray, torch.Tensor], optional
    (I) Batch index of each of the clusters. If not specified, the
    assumption is that each count corresponds to a specific entry
batch_size : int, optional
    Number of entries in the batch. Must be specified along batch_ids
is_numpy : bool, default True
    Default type of index. Provide if `data` may be empty

---
### FunctionDef: `__init__`

Initialize the attributes of the class.

Parameters
----------
data : Union[np.ndarray, torch.Tensor, ME.SparseTensor]
    (N, C) Batched tensors
counts : Union[List[int], np.ndarray, torch.Tensor]
    (B) Number of data rows in each entry
batch_size : int, optional
    Number of entries that make up the batched data
is_sparse : bool, default False
    If initializing from an ME sparse data, flip to True
has_batch_col : bool, default False
    Wheather the tensor has a column specifying the batch ID
coord_cols : Union[List[int], np.ndarray], optional
    List of columns specifying coordinates

---
### FunctionDef: `__init__`

Initialize the augmenter.

Parameters
----------
translate : dict, optional
    Translation confiugration (move input image around)

---
### FunctionDef: `__init__`

Initialize the basics of the output file.

Parameters
----------
file_name : str, default 'output.csv'
    Name of the output CSV file
overwrite : bool, default False
    If True, overwrite the output file if it already exists
append : bool, default False
    If True, add more rows to an existing CSV file
accept_missing : bool, default True
    Tolerate missing keys

---
### FunctionDef: `__init__`

Initialize the box object.

Parameters
----------
lower : np.ndarray
    (3) Lower bounds of the box
upper : np.ndarray
    (3) Upper bounds of the box

---
### FunctionDef: `__init__`

Initialize the calibration manager.

Parameters
----------
do_tracking : bool, default False
    Segment track to get a proper local dQ/dx estimate
**cfg : dict
    Calibration manager configuration

---
### FunctionDef: `__init__`

Initialize the calibration map.

Parameters
----------
dims : List[int]
    List of dimensions (0: x, 1: y, 2: z)
bins : List[int]
    Number of bins in each dimension
range : List[List[float]]
    Axis range in each dimension
values : np.ndarray
    Values in each bin
dummy : float
    Dummy values which should be overwritten with 1. (no information)

---
### FunctionDef: `__init__`

Initialize the cathode crosser finder algorithm.

Parameters
----------
crossing_point_tolerance : float
    Maximum allowed distance in the cathode plane (in cm) between two
    fragments of a cathode crosser to be considered compatible
offset_tolerance
    Maximum allowed discrepancy between end-point to cathode offsets of
    two fragments of a cathode crosser to be considered compatible
angle_tolerance : float
    Maximum allowed angle (in radians) between the directions of two
    fragments of a cathode crosser to be considered compatible
adjust_crossers : bool, default True
    If True, shifts existing cathode crossers to fix the small breaks
    that may exist at the level of the cathode
merge_crossers : bool, default True
    If True, look for tracks that have been broken up at the cathode
    and merge them into one particle
detector : str, optional
    Detector to get the geometry from
geometry_file : str, optional
    Path to a `.yaml` geometry file to load the geometry from

---
### FunctionDef: `__init__`

Initialize the children counting parameters.

Parameters
----------
mode : str, default 'shape'
    Attribute name to categorize children. This will count each child
    object for different category separately.

---
### FunctionDef: `__init__`

Initialize the cluster graph constructor.

Parameters
----------
graph : dict
    Graph construction configuration dictionary
shapes : List[str]
    List of shape names to construct clusters for
edge_threshold : float
    Edge score below which it is disconnected (or above which it is,
    if the `inverted` parameter is turned on
kernel_fn : callable, optional
    Kernel function computing edge scores from edge features
min_size : int, default 0
    Minimum number of points below which pixels are considered orphans
    to be merged into touching larger clusters
invert : bool, default True
    Invert the edge scores so that 0 is on an 1 is off
label_edges : bool, default False
    If `True`, use cluster labels to label the edges as on or off
target_col : int, default CLUST_COL
    Index of the column which specifies the label cluster ID for each point
training : bool, default False
    If `True`, this constructor is being used at train time
orphan : dict, optional
    Orphan clustering configuration dictionary

Raises
------
ValueError
    If the graph type is not supported.

---
### FunctionDef: `__init__`

Initialize the collation parameters.

Parameters
----------
split : bool, default False
    Whether to split the input by module ID (each module gets its
    own batch ID, multiplies the number of batches by `num_modules`)
target_id : int, default 0
    If split is `True`, specifies where to relocate the points
detector : str, optional
    Name of a recognized detector to the geometry from
geometry_file : str, optional
    Path to a `.yaml` geometry file to load the geometry from
overlay : dict, optional
    Image overlay configuration
source : dict, optional
    Dictionary which maps keys to their corresponding sources. This can
    be used to split tensors without having to check the geometry

---
### FunctionDef: `__init__`

Initialize the connected component constructor.

Parameters
----------
min_size : int, default 0
    Minimum number of points in a label cluster to be considered
    already assigned. If below this value, it is considered an orphan.
orphan : dict
    Orphan assigner configuration dictionary

---
### FunctionDef: `__init__`

Initialize the containment conditions.

If the `source` method is used, the cut will be based on the source of
the point cloud, i.e. if a point cloud was produced by TPCs i and j, it
must be contained within the volume bound by the set of TPCs i and j,
and whichever volume is present between them.

Parameters
----------
margin : Union[float, List[float], np.array]
    Minimum distance from a detector wall to be considered contained:
    - If float: distance buffer is shared between all 6 walls
    - If [x,y,z]: distance is shared between pairs of falls facing
      each other and perpendicular to a shared axis
    - If [[x_low,x_up], [y_low,y_up], [z_low,z_up]]: distance is
      specified individually of each wall.
cathode_margin : float, optional
    If specified, sets a different margin for the cathode boundaries
detector : str, optional
    Detector to get the geometry from
geometry_file : str, optional
    Path to a `.yaml` geometry file to load the geometry from
mode : str, default 'module'
    Containement criterion (one of 'global', 'module', 'tpc'):
    - If 'tpc', makes sure it is contained within a single tpc
    - If 'module', makes sure it is contained within a single module
    - If 'detector', makes sure it is contained within the
      outermost walls
    - If 'source', use the origin of voxels to determine which TPC(s)
      contributed to them, and define volumes accordingly
    - If 'meta', use the metadata range as a basis for containment.
      Note that this does not guarantee containment within the detector.
allow_multi_module : bool, default False
    Whether to allow particles/interactions to span multiple modules
min_particle_sizes : Union[int, dict], default 0
    When checking interaction containment, ignore particles below the
    size (in voxel count) specified by this parameter. If specified
    as a dictionary, it maps a specific particle type to its own cut.

---
### FunctionDef: `__init__`

Initialize the convolution block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
stride : int, default 1
    Convolution kernel stride
dilation : int, default 1
    Convolution kernel dilation
dimension : int, default 3
    Dimension of the input image
activation : union[str, dict], default 'relu'
    activation function configuration
normalization : union[str, dict], default 'batch_norm'
    normalization function configuration
bias : bool, default False
    Whether to add a bias term to the kernel

---
### FunctionDef: `__init__`

Initialize the decoder.

Parameters
----------
cfg : dict
    Decoder configuration block

---
### FunctionDef: `__init__`

Initialize the drawer attributes

Parameters
----------
data : dict
    Dictionary of data products
draw_mode : str, default 'both'
    Drawing mode, one of 'reco', 'truth' or 'both'
truth_point_mode : str, optional
    If specified, tells which attribute of the :class:`TruthFragment`,
    :class:`TruthParticle` or :class:`TruthInteraction` object to use
    to fetch its point coordinates
split_scene : bool, default True
    If True and when drawing both reconstructed and truth information,
    split the traces between two separate scenes
detector : str, optional
    Name of the detector to be drawn
detector_coords : bool, default True
    Whether the object coordinates are expressed in detector coordinates
**kwargs : dict, optional
    Additional arguments to pass to the :func:`layout3d` function

---
### FunctionDef: `__init__`

Initialize the drawer.

Parameters
----------
log_dir, str
    Path to the parent directory of all the log files
interactive : bool, default True
    If `True`, use plotly to draw the training/validation curve
paper : bool, default False
    If `True`, format the figure for a paper, using latext style
alpha : float, default 0.5
    Opacity of the traces
train_prefix : str, default 'train'
    Log name prefix shared between training logs
val_prefix : str, default 'inference'
    Log name prefix shared between validation logs
separator : str, default ':'
    Character used to separate the acceptable metric names in the
    metric parameter

---
### FunctionDef: `__init__`

Initialize the dropout block.

Parameters
----------
in_features : int
    Number of input features
out_features : int
    Number of output features
stride : int, default 1
    Convolution kernel stride
dilation : int, default 1
    Convolution kernel dilation
p : float, default 0.5
    Dropout probability
dimension : int, default 3
    Dimension of the input image
activation : union[str, dict], default 'relu'
    activation function configuration
normalization : union[str, dict], default 'batch_norm'
    normalization function configuration
bias : bool, default False
    Whether to add a bias term to the kernel

---
### FunctionDef: `__init__`

Initialize the embedding model.

Parameters
----------
uresnet : dict
    Backbone UResNet configuration
**base : dict, optional
    Basic parameters

---
### FunctionDef: `__init__`

Initialize the encoder.

Parameters
----------
cfg : dict
    Encoder configuration block

---
### FunctionDef: `__init__`

Initialize the evidential network.

Parameters
----------
in_channels : int
    Number of features from the upstream feature extractor
mlp : dict
    MLP configuration dictionary
eps : float, default 0.0
    Offset to apply to the softplus output
logspace : bool, default False
    Whether to take the sigmoid of gamma, or not

---
### FunctionDef: `__init__`

Initialize the fiducial conditions.

Parameters
----------
margin : Union[float, List[float], np.array]
    Minimum distance from a detector wall to be considered contained:
    - If float: distance buffer is shared between all 6 walls
    - If [x,y,z]: distance is shared between pairs of falls facing
      each other and perpendicular to a shared axis
    - If [[x_low,x_up], [y_low,y_up], [z_low,z_up]]: distance is
      specified individually of each wall.
cathode_margin : float, optional
    If specified, sets a different margin for the cathode boundaries
detector : str, default 'icarus'
    Detector to get the geometry from
geometry_file : str, optional
    Path to a `.yaml` geometry file to load the geometry from
mode : str, default 'module'
    Containement criterion (one of 'global', 'module', 'tpc'):
    - If 'tpc', makes sure it is contained within a single tpc
    - If 'module', makes sure it is contained within a single module
    - If 'detector', makes sure it is contained within the
      outermost walls
    - If 'meta', use the metadata range as a basis for containment.
      Note that this does not guarantee containment within the detector.
truth_vertex_mode : str, default 'truth_vertex'
     Vertex attribute to use to check containment of true interactions

---
### FunctionDef: `__init__`

Initialize the field calibrator.

Notes
-----
Placeholder until this module is implemented

---
### FunctionDef: `__init__`

Initialize the flash matching algorithm.

Parameters
----------
flash_key : str
    Flash data product name. In most cases, this is unambiguous, unless
    there are multiple types of segregated optical detectors
volume : str
    Physical volume corresponding to each flash ('module' or 'tpc')
ref_volume_id : str, optional
    If specified, the flash matching expects all interactions/flashes
    to live into a specific optical volume. Must shift everything.
method : str, default 'likelihood'
    Flash matching method (one of 'likelihood' or 'barycenter')
detector : str, optional
    Detector to get the geometry from
geometry_file : str, optional
    Path to a `.yaml` geometry file to load the geometry from
parent_path : str, optional
    Path to the parent directory of the main analysis configuration.
    This allows for the use of relative paths in the post-processors.
**kwargs : dict
    Keyword arguments to pass to specific flash matching algorithms

---
### FunctionDef: `__init__`

Initialize the full chain model.

Parameters
----------
chain : dict
    Dictionary of parameters used to configure the chain
uresnet_deghost : dict, optional
    Deghosting model configuration
uresnet_deghost_loss : dict, optional
    Deghosting loss configuration
uresnet : dict, optional
    Segmentation model configuration
uresnet_loss : dict, optional
    Segmentation loss configuration
uresnet_ppn: dict, optional
    Segmentation and point proposal model configuration
uresnet_ppn_loss : dict, optional
    Segmentation and point proposal loss configuration
graph_spice : dict, optional
    Supervised connected component clustering model configuration
graph_spice_loss : dict, optional
    Supervised connected component clustering loss configuration
grappa_shower : dict, optional
    Shower aggregation model configuration
grappa_track : dict, optional
    Track aggregation model configuration
grappa_particle : dict, optional
    Global particle aggregation configuration
grappa_inter : dict, optional
    Interaction aggregation model configuration

---
### FunctionDef: `__init__`

Initialize the full chain model.

Parameters
----------
chain : dict
    Dictionary of parameters used to configure the chain
uresnet_deghost : dict, optional
    Deghosting model configuration
uresnet_ppn : dict, optional
    Segmentation and point proposal model configuration
adapt_labels : dict, optional
    Parameters for the cluster label adaptation (if non-standard)
dbscan : dict, optional
    Connected component clustering configuration
graph_spice : dict, optional
    Supervised connected component clustering model configuration
grappa_shower : dict, optional
    Shower aggregation model configuration
grappa_track : dict, optional
    Track aggregation model configuration
grappa_particle : dict, optional
    Global particle aggregation configuration
grappa_inter : dict, optional
    Interaction aggregation model configuration
calibration : dict, optional
    Calibration manager configuration

---
### FunctionDef: `__init__`

Initialize the graph constructor.

This adds the possibility to set the `k` parameter of the kNN graph.

Parameters
----------
k : int
    Maximum number of nodes a node can be connected to
**kwargs : dict, optional
    Additional parameters to pass to the :class:`GraphBase`
    constructor.

---
### FunctionDef: `__init__`

Initialize the graph constructor.

This adds the possibility to set the directionality of the
bipartite graph explicitly.

Parameters
----------
directed_to : str, default 'secondary'
    Direction of the edge information flow ('primary' or 'secondary')
**kwargs : dict, optional
    Additional parameters to pass to the :class:`GraphBase` constructor.

---
### FunctionDef: `__init__`

Initialize the laoder.

Parameters
----------
stream : _io.TextIOWrapper
    Output of python's `open` function on a yaml file

---
### FunctionDef: `__init__`

Initialize the layer.

---
### FunctionDef: `__init__`

Initialize the likelihood-based flash matching algorithm.

Parameters
----------
cfg : str
    Flash matching configuration file path
detector : str, optional
    Detector to get the geometry from
parent_path : str, optional
    Path to the parent configuration file (allows for relative paths)
reflash_merging_window : float, optional
    Maximum time between successive flashes to be considered a reflash
scaling : Union[float, str], default 1.
    Global scaling factor for the depositions (can be an expression)
alpha : float, default 0.21
    Number of excitons (Ar*) divided by number of electron-ion pairs (e-,Ar+)
recombination_mip : float, default 0.65
    Recombination factor for MIP-like particles in LAr
legacy : bool, default False
    Use the legacy OpT0Finder function(s). TODO: remove when dropping legacy

---
### FunctionDef: `__init__`

Initialize the list and the default value.

Parameters
----------
object_list : List[object]
    Object list
default : object
    Default object class to use to type the list, if it is empty

---
### FunctionDef: `__init__`

Initialize the loss function parameters.

Parameters
----------
alpha : float, default 1
    Overall loss scaling factor
gamma : float, default 2
    Overall power to apply to the score prefactor
logits : bool, default False
    If `True`, the output of the network is considered to be logits
balance_loss : bool, default False
    If `True`, weights are applied to the loss to account for class imbalance
reduction : str, default 'none'
    Reduction function to apply to the output

---
### FunctionDef: `__init__`

Initialize the loss function parameters.

Parameters
----------
eps : float, default 1e-6
    Regularization constant for the ratio

---
### FunctionDef: `__init__`

Initialize the loss function parameters.

Parameters
----------
eps : float, default 1e-6
    Regularization constant for the ratio

---
### FunctionDef: `__init__`

Initialize the loss function parameters.

Parameters
----------
log_dice : dict, optional
    Parameters to pass to the :class:`BinaryLogDiceLoss`
bce : dict, optional
    Parameters to pass to the :class:`torch.nn.BCEWithLogitsLoss`
reduction : str, default 'mean'
    Reduction function to apply tot he BCE loss
w_dice : float, default 0.8
    Prefacor to be applied to the log Dice loss
w_ce : float, default 0.2
    Prefactor to be applied to the binary cross-entropy loss

---
### FunctionDef: `__init__`

Initialize the loss function parameters.

Parameters
----------
reduction : str, default 'none'
    Reduction function to apply to the output
eps : float, default 1e-7
    Offset to apply to the predictions/labels before passing them
    through the MSE loss function.

---
### FunctionDef: `__init__`

Initialize the loss function parameters.

Parameters
----------
threshold : float, default 0.2
    Fraction of the maximum loss value to use as a threshold
reduction : str, default 'none'
    Reduction function to apply to the output

---
### FunctionDef: `__init__`

Initialize the loss function parameters.

Parameters
----------
w_mincut : float, default 1.0
    Prefacor to be applied to the Mincut loss
mincut : dict, optional
    Parameters to pass to the :class:`Mincut`
**kwargs : dict, optional
    Parameters to pass to the :class:`BinaryLogDiceCELoss`

---
### FunctionDef: `__init__`

Initialize the loss function.

Parameters
----------
loss : str, default 'log_dice'
    Loss functional used to train edge scores
invert : bool, default True
    If `True`, on edges are labeled as 0 and off edges as 1
balance_loss : bool, default True
    Whether to weight the loss to account for class imbalance
equal_sampling : bool, default False
    If `True`, sample the same number of edges from each label class
min_sample_edges : int, default 1000
    If sampling evenly, minimum number of edges to sample with replacement

---
### FunctionDef: `__init__`

Initialize the manager.

Parameters
----------
geometry : dict
    Geometry configuration
gain_applied : bool, default False
    Weather the gain conversion was applied upstream or not
**cfg : dict, optional
    Calibrator configurations

---
### FunctionDef: `__init__`

Initialize the mask downsampler.

---
### FunctionDef: `__init__`

Initialize the mixed encoder.

Initializes the two underlying encoders:
- :class:`ClustGeoEdgeEncoder``
- :class:`ClustCNNEdgeEncoder`

Parameters
----------
geo_encoder : dict
    Geometric edge encoder configuration
cnn_encoder : dict,
    CNN edge encoder configuration

---
### FunctionDef: `__init__`

Initialize the mixed encoder.

Initializes the two underlying encoders:
- :class:`ClustGeoNodeEncoder`
- :class:`ClustCNNNodeEncoder`

Parameters
----------
geo_encoder : dict
    Geometric node encoder configuration
cnn_encoder : dict,
    CNN node encoder configuration

---
### FunctionDef: `__init__`

Initialize the node classifcation loss function.

Parameters
----------
target : str
    Column in the label tensor specifying the classification target
loss : str, default 'ce'
    Name of the loss function to apply
balance_loss : bool, default False
    Whether to weight the loss to account for class imbalance
weights : list, optional
    (C) One weight value per class
use_closest : bool, default False
    For each particle group, assign the label class to the node which
    is closest to the particle start point only
secondary_label : Union[int, List[int]], default -1
    When using `use_closest=True`, this label is assigned to nodes which
    are not the closest to a the start point of a particle group. These
    numbers can be different for each class if specified as a list

---
### FunctionDef: `__init__`

Initialize the node orientation loss function.

Parameters
----------
loss : str, default 'ce'
    Name of the loss function to apply

---
### FunctionDef: `__init__`

Initialize the node regression loss function.

Parameters
----------
target : str
    Column(s) in the label tensor specifying the regression target(s)
loss : str, default 'mse'
    Name of the loss function to apply

---
### FunctionDef: `__init__`

Initialize the normalization layer.

Parameters
----------
eps : float, default 1e-5
    Ensures non-divergent output features

---
### FunctionDef: `__init__`

Initialize the normalization layer.

Parameters
----------
eps : float, default 1e-8
    Ensures non-divergent output features

---
### FunctionDef: `__init__`

Initialize the orphan assigner.

Parameters
----------
mode : str
    Orphan assignment mode, one of 'knn' or 'radius'
iterate : bool, default True
    Iterate the process until no additional orphans can be assigned
assign_all : bool, default True
    If `True`, force assign all orphans to a cluster. In the 'knn' mode,
    this is guaranteed, provided there is at least one labeled point.
    In the 'radius' mode, this uses DBSCAN for outliers.
**kwargs : dict
    Arguments to pass to the underlying classifier function

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
aggr : str
    Aggregation function to apply ('sum', 'mean', 'max', etc.)

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
cluster_event : larcv.EventClusterPixel2D
    Event which contains the 2D clusters
projection_id : int
    Projection ID to get the 2D images from

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
collection_only : bool, default False
    If True, only uses the collection plane charge
collection_id : int, default 2
    Index of the collection plane
**kwargs : dict, optional
    Data product arguments to be passed to the `process` function

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
include_fragment_edges : bool, default False
    If `True`, includes edges which join particles in the same group
**kwargs : dict, optional
    Data product arguments to be passed to the `process` function

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
include_point_tagging : bool, default True
    If `True`, includes start vs end point tagging
**kwargs : dict, optional
    Data product arguments to be passed to the `process` function

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
particle_event : larcv.EventParticle, optional
    List of true particle information. If prodided, allows to fetch
    more information about each of the pixels in the image
add_particle_info : bool, default False
    If `True`, adds truth information from the true particle list
clean_data : bool, default False
    If `True`, removes duplicate voxels
type_include_mpr : bool, default False
    If `False`, sets all PID labels to -1 for MPR particles
type_include_secondary : bool, default False
    If `False`, sets all PID labels to -1 for secondary particles
primary_include_mpr : bool, default False
    If `False`, sets all primary labels to -1 for MPR particles
break_clusters : bool, default False
    If `True`, runs DBSCAN on each cluster, assigns different cluster
    IDs to different fragments of the broken-down cluster
break_eps : float, default 1.1
    Distance scale used in the break up procedure
break_metric : str, default 'chebyshev'
    Distance metric used in the break up produce
shape_precedence: list, default SHAPE_PREC
     Array of classes in the reference array, ordered by precedence
**kwargs : dict, optional
    Data product arguments to be passed to the `process` function

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
pixel_coordinates : bool, default True
    If set to `True`, the parser rescales the truth positions
    (start, end, etc.) to voxel coordinates
asis : bool, default False
    Load the objects as larcv objects, do not build local data class
**kwargs : dict, optional
    Data product arguments to be passed to the `process` function

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
pixel_coordinates : bool, default True
    If set to `True`, the parser rescales the truth positions
    (start, end, etc.) to voxel coordinates
post_process : bool, default True
    Processes particles to add/correct missing attributes
skip_empty : bool, default False
    Do not read the truth information corresponding to empty particles.
    This saves considerable read time when there are a lot of irrelevant
    particle stored in the LArCV file. It puts an empty `Particle`
    object in place of empty particles, to preserve list size and typing.
asis : bool, default False
    Load the objects as larcv objects, do not build local data class
**kwargs : dict, optional
    Data product arguments to be passed to the `process` function

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
projection_id : int
    Projection ID to get the 2D images from
sparse_event: larcv.EventSparseTensor2D, optional
    Sparse tensor to get the voxel/features from
sparse_event_list: List[larcv.EventSparseTensor2D], optional
    List of sparse tensors to get the voxel/features from

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
projection_id : int, optional
    Projection ID to get the 2D image from (if fetching from 2D)
**kwargs : dict, optional
    Data product arguments to be passed to the `process` function

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
sparse_event: larcv.EventSparseTensor3D, optional
    Sparse tensor to get the voxel/features from
sparse_event_list: List[larcv.EventSparseTensor3D], optional
    List of sparse tensors to get the voxel/features from
num_features : int, optional
    If a positive integer is specified, the sparse_event_list will be
    split in equal lists of length `features`. Each list will be
    concatenated along the feature dimension separately. Then all
    lists are concatenated along the first dimension (voxels). For
    example, this lets you work with distinct detector volumes whose
    input data is stored in separate TTrees. `num_features` is required
    to be a divider of the `sparse_event_list` length.
hit_keys : list of int, optional
    Indices among the input features of the `_hit_key_` TTrees that can
    be used to infer the `nhits` quantity (doublet vs triplet point).
nhits_idx : int, optional
    Index among the input features where the `nhits` feature
    (doublet vs triplet) should be inserted.
feature_only : bool, default False
    If `True`, only return the feature vector without the coordinates

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
sparse_value_event_list : List[larcv.EventSparseTensor3D]
    (7) List of sparse tensors used to compute the rescaled charge
    - Charge value of each of the contributing planes (3)
    - Index of the plane hit contributing to the space point (3)
    - Semantic labels (1)
collection_only : bool, default False
    If True, only uses the collection plane charge
collection_id : int, default 2
    Index of the collection plane
**kwargs : dict, optional
    Data product arguments to be passed to the `process` function

---
### FunctionDef: `__init__`

Initialize the parser.

Parameters
----------
sparse_value_event_list : List[larcv.EventSparseTensor3D]
    List of sparse tensors used to compute the aggregated charge
value_aggr : str
    Value aggregation function to apply ('sum', 'mean', 'max', etc.)
**kwargs : dict, optional
    Data product arguments to be passed to the `process` function

---
### FunctionDef: `__init__`

Initialize the particle image classifier.

Parameters
----------
classifier : dict
    Image classifier configuration
classifier_loss : dict, optional
    Image classifier loss configuration

---
### FunctionDef: `__init__`

Initialize the particle point-enhanced clustering algorithm.

Parameters
----------
method : str, default 'masked_dbscan'
    Clustering method
eps : float, default 1.8
    The maximum distance between two samples for one to be considered
    as in the neighborhood of the other.
min_samples : int, default 1
    The number of samples (or total weight) in a neighborhood for a
    point to be considered as a core point.
metric : str, default 'euclidean'
    Metric used to compute the pair-wise distances between space points
mask_radius : float, default 5.0
    Radius to mask around each particle point

---
### FunctionDef: `__init__`

Initialize the post-processing manager.

Parameters
----------
cfg : dict
    Post-processor configurations
parent_path : str, optional
    Path to the analysis tools configuration file

---
### FunctionDef: `__init__`

Initialize the post-processor.

Parameters
----------
arg0 : type
    Description of arg0
arg1 : type
    Description of arg1
obj_type : Union[str, List[str]]
    Types of objects needed in this post-processor (fragments,
    particles and/or interactions). This argument is shared between
    all post-processors. If None, does not load these objects.
run_mode : str
    One of 'reco', 'truth' or 'both'. Determines what kind of object
    the post-processor has to run on.

---
### FunctionDef: `__init__`

Initialize the primary identification loss function.

Parameters
----------
target : str
    Column name in the label tensor specifying the aggregation target
mode : str, default 'group'
    Loss mode, one of 'group', 'forest' or 'particle_forest'
    - 'group' turns every edge that connect two nodes that belong to
      the same group (same target value) on
    - 'forest' ensures that at least one path in the graph connects two
      nodes, if they belong to the same group
    - 'particle_forest' only turns on edges that join two particles
      have a parentage relationship in the true particle tree
loss : Union[str, dict], default 'ce'
    Name of the loss function to apply
balance_loss : bool, default False
    Whether to weight the loss to account for class imbalance
high_purity : bool, default False
    Only apply loss to nodes which belong to a sensible group, i.e.
    one with exactly one shower primary in it (not 0, not > 1)

---
### FunctionDef: `__init__`

Initialize the recombination model and its constants.

Parameters
----------
efield : float
    Electric field in kV/cm
drift_dir : np.ndarray
    (3) three-vector indicating the direction of the drift field
model : str, default 'mbox'
    Recombination model name (one of 'birks', 'mbox' or 'mbox_ell')
birks_a : float, default 0.800 (ICARUS CNGS fit)
    Birks model A parameter
birks_k : float, default 0.0486 (ICARUS CNGS fit)
    Birks model k parameter in (kV/cm)(gm/cm^2)/MeV
mbox_alpha : float, default 0.906 (ICARUS fit)
    Modified box model alpha parameter
mbox_beta : float, default 0.203 (ICARUS fit)
    Modified box model beta parameter in (kV/cm)(g/cm^2)/MeV
mbox_ell_r : float, default 1.25 (ICARUS fit)
    Modified box model ellipsoid correction R parameter
mip_dedx : float, default 2.105168
    Mean dE/dx value of a MIP in LAr. Used to apply a flat recombination
    correction if the local dE/dx is not evaluated through tracking.
track_mode : float, default 'bin_pca'
    If tracking is done to produce local dQ/dx values along tracks,
    defines the track chunking method to be used.
**kwargs : dict, optional
    Additional arguments to pass to the tracking algorithm

---
### FunctionDef: `__init__`

Initialize the recombination model and its constants.

Parameters
----------
gain : Union[list, float]
    Conversion factor from ADC to electrons (unique or per tpc)
num_tpcs : int
    Number of TPCs in the detector

---
### FunctionDef: `__init__`

Initialize the template-based particle identifier.

Parameters
----------
use_table : bool, default True
    If `True`, use tabulated values of dE/dx vs residual range. The
    dE/dx is evaluated using the theoretical value otherwise.
use_mpv : bool, default False
    If `True`, use the most-probable dE/dx value instead of the mean 
include_pids : list, default [2, 3, 4, 5]
    Particle species to consider as a viable PID candidate
optimize_rr : bool, default False
    If `True`, vary RR to minimize the chi2 agreement. If `False`, the
    track is assumed to range out (no hard scattering, no exiting)
max_rr : float
    Maximum allowed residual range offset
optimize_orient : bool, default True
    If `True`, compute the chi2 w.r.t. to the start and end points of
    the track, in case the travel direction was mireconstructed
tracking_mode : str, default 'step_next'
    Method used to chunk the track and compute the dE/dx vs RR (one of
    'step', 'step_next' or 'bin_pca')
**tracker : dict, optional
    Arguments to pass to the tracking algorithm (track chunking)

---
### FunctionDef: `__init__`

Initialize the track end point assignment parameters.

Parameters
----------
method : str, default 'local'
    Algorithm to correct track startpoint/endpoint misplacement. The
    following methods are available:
    - local: computes local energy deposition density only at
    the extrema and chooses the higher one as the endpoint.
    - gradient: computes local energy deposition density throughout
    the track, computes the overall slope (linear fit) of the energy
    density variation to estimate the direction.
    - ppn: uses ppn candidate predictions (classify_endpoints) to
    assign start and endpoints.
kwargs : dict
    Extra arguments to pass to the `check_track_orientation` or the
    `check_track_orientation_ppn' functions

---
### FunctionDef: `__init__`

Initialize the track validity post-processor.

Parameters
----------
threshold : float, default 3.0
    Vertex distance above which a track is not considered a primary
ke_theshold : float, default 50.0
    Kinetic energy threshold below which a track close to the vertex
    is deemed not primary/not valid
check_small_track : bool, default False
    Whether or not to apply the small track KE cut

---
### FunctionDef: `__init__`

Initialize the translater..

This defines a way to move the image around within a volume greater
than that define by the image metadata. The box must be larger than
the image itself.

Parameters
----------
lower : np.ndarray
    Lower bounds of the box in which to move the image around
upper : np.ndarray
    Upper bounds of the box in which to move the image around

---
### FunctionDef: `__init__`

Initialize the trigger information parser.

Parameters
----------
file_path : str
    Path to the csv file which contains the trigger information
correct_flash_times : bool, default True
    If True, corrects the flash times using w.r.t. the trigger times
flash_keys : List[str], optional
    When correcting flash times, provide the list of flash products
    to correct times for
flash_time_corr_us : float, default 4
    Systematic correction between the trigger time and the flash time
    in us

---
### FunctionDef: `__init__`

Initialize the unwrapper.

Parameters
----------
geometry : Geometry
     Detector geometry (needed if the input was split in
     different volumes)
remove_batch_col : bool
     Remove column which specifies batch ID from the unwrapped tensors

---
### FunctionDef: `__init__`

Initialize the vertex finder properties.

Parameters
----------
include_shapes : List[int], default [0, 1]
    List of semantic classes to consider for vertex reconstruction
use_primaries : bool, default True
    If true, only considers primary particles to reconstruct the vertex
update_primaries : bool, default False
    Use the reconstructed vertex to update primaries
anchor_vertex : bool, default True
    If true, anchor the candidate vertex to particle objects,
    with the expection of interactions only composed of showers
touching_threshold : float, default 2 cm
    Maximum distance for two track points to be considered touching
angle_threshold : float, default 0.3 radians
    Maximum angle between the vertex-to-start-point vector and a shower
    direction to consider that a shower originated from the vertex

---
### FunctionDef: `__init__`

Initialize the vertex regression loss function.

Parameters
----------
balance_primary_loss : bool, default `False`
    Whether to weight the primary loss to account for class imbalance
primary_loss : str, default `'ce'`
    Name of the loss function used to predict interaction primaries
regression_loss : str, default `'mse'`
    Name of the loss function used to predict the vertex position
only_contained : bool, default `True`
    Only considers label vertices contained in the active volume
normalize_positions : bool, default `False`
    Normalize the target position between 0 and 1
use_anchor_points : bool, default `False`
    Predict positions w.r.t. to the particle end points
return_vertex_labels : bool, default `False`
    If `True`, return the list vertex labels (one per particle)
detector : str, optional
    Name of a recognized detector to the geometry from
geometry_file : str, optional
    Path to a `.yaml` geometry file to load the geometry from

---
### FunctionDef: `__init__`

Initializes a detector geometry object.

The geometry configuration file is a YAML file which contains all the
necessary information to construct the physical boundaries of the
a detector (TPC size, positions, etc.) and (optionally) the set
of optical detectors and CRTs.

If the detector is already supported, the name is sufficient.
Supported: 'icarus', 'sbnd', '2x2', '2x2_single', 'ndlar'

Parameters
----------
detector : str, optional
    Name of a recognized detector to the geometry from
file_path : str, optional
    Path to a `.yaml` geometry configuration

---
### FunctionDef: `__init__`

Initializes attributes shared accross all graph constructors.

Parameters
----------
directed : bool, default False
    If `True`, direct the edges from lower to higher rank only
max_length : Union[float, List[float]], optional
    Length limitation to be applied to the edges. Can be:
    - Sclar: Constant threshold
    - Array: N*(N-1)/2 elements which correspond to the upper triangle
             of an adjacency matrix providing cuts for each class pairs
classes : Union[int, List[int]], optional
    List of classes that are involved in the graph
max_count : int, optional
    Maximum number of edges that can be produced (memory limitation)
dist_method : str, default 'voxel'
    Method used to compute inter-node distance ('voxel' or 'centroid')
dist_algorithm : str, default 'brute'
    Algorithm used to comppute inter-node distance
    ('brute' or 'recursive')

---
### FunctionDef: `__init__`

Initializes the CNN-based edge encoder.

Simply passes the configuration along to the underlying sparse residual
CNN encoder defined in :class:`SparseResidualEncoder`.

Parameters
----------
**cfg : dict, optional
    Configuration to pass along to the sparse residual encoder

---
### FunctionDef: `__init__`

Initializes the CNN-based global encoder.

Simply passes the configuration along to the underlying sparse residual
CNN encoder defined in :class:`SparseResidualEncoder`.

Parameters
----------
**cfg : dict, optional
    Configuration to pass along to the sparse residual encoder

---
### FunctionDef: `__init__`

Initializes the CNN-based node encoder.

Simply passes the configuration along to the underlying sparse residual
CNN encoder defined in :class:`SparseResidualEncoder`.

Parameters
----------
**cfg : dict, optional
    Configuration to pass along to the sparse residual encoder

---
### FunctionDef: `__init__`

Initializes the basics of the output file.

Parameters
----------
file_name : str, optional
    Name of the output HDF5 file
keys : List[str], optional
    List of data product keys to store. If not specified, store everything
skip_keys: List[str], optionl
    List of data product keys to skip
dummy_ds: Dict[str, str], optional
    Keys for which to create placeholder datasets. For each key, specify
    the object type it is supposed to represent as a string.
overwrite : bool, default False
    If `True`, overwrite the output file if it already exists
append : bool, default False
    If `True`, add new values to the end of an existing file
prefix : str, optional
    Input file prefix. It will be use to form the output file name,
    provided that no file_name is explicitely provided
split : bool, default False
    If `True`, split the output to produce one file per input file
lite : bool, default False
    If `True`, the lite version of objects is stored (drop point indexes)

---
### FunctionDef: `__init__`

Initializes the build manager.

Parameters
----------
fragments : bool
    Build/load RecoFragment/TruthFragment objects
particles : bool
    Build/load RecoParticle/TruthParticle objects
interactions : bool
    Build/load RecoInteraction/TruthInteraction objects
mode : str, default 'both'
    Whether to construct reconstructed objects, true objects or both
sources : Dict[str, str], optional
    Dictionary which maps the necessary data products onto a name
    in the input/output dictionary of the reconstruction chain.

---
### FunctionDef: `__init__`

Initializes the builder.

Parameters
----------
mode : str, default 'both'
    Whether to construct reconstructed objects, true objects or both
    (one of 'reco', 'truth', 'both' or 'all')
units : str, default 'cm'
    Units in which the position arguments of the constructed objects
    should be expressed (one of 'cm' or 'px')

---
### FunctionDef: `__init__`

Initializes the class attributes.

Parameters
----------
cfg : dict
    Global configuration dictionary
rank : int, optional
    Rank of the GPU. If not specified, the model will be run on CPU if
    `world_size` is 0 and GPU is `world_size` is > 0.

---
### FunctionDef: `__init__`

Initializes the geometric-based node encoder.

Parameters
----------
use_numpy : bool, default True
    Generate the features on CPU

---
### FunctionDef: `__init__`

Initializes the geometric-based node encoder.

Parameters
----------
use_numpy : bool, default True
    Generate the features on CPU
add_value : bool, default False
    Add mean and RMS value of pixels in the cluster
add_shape : bool, default False
    Add the particle semantic type
add_points : bool, default False
    Add the start/end points of the particles
add_local_dirs : bool, default False
    Add the local direction estimates at the start and end points
dir_max_dist : float, default 5.
    Radius around the end points included to estimate the directions
add_local_dedxs : boo, default False
    Add the local dE/dx estimates at the start and end points
dedx_max_dist : float, default 5.
    Readius around the end points incldued to estimate the dE/dx

---
### FunctionDef: `__init__`

Initializes the kernel.

Parameters
----------
num_features : int
    Number of dimensions in feature embedding space
bias : bool, default False
    If `True`, allows for an overall bias in the bilinear layer

---
### FunctionDef: `__init__`

Initializes the kernel.

Parameters
----------
num_features : int
    Number of dimensions in feature embedding space
bias : bool, default False
    If `True`, allows for an overall bias in the bilinear layer
mlp : dict, optional
    MLP architecture configuration, see :class:`MLP`

---
### FunctionDef: `__init__`

Initializes the kernel.

Parameters
----------
num_features : int
    Number of dimensions in feature embedding space
eps : float
    Features regularization factor

---
### FunctionDef: `__init__`

Initializes the kernel.

Parameters
----------
num_features : int
    Number of dimensions in feature embedding space
eps : float
    Features regularization factor

---
### FunctionDef: `__init__`

Initializes the linear layer.

Parameters
----------
in_channels : int
    Number of features coming from the upstream feature extractor
out_channels : int
    Number of logits to output

---
### FunctionDef: `__init__`

Initializes the linear layer.

Parameters
----------
in_channels : int
    Number of features coming from the upstream feature extractor
out_channels : int
    Number of logits to output
positive_out : bool, default False
    If `True`, pass the output through a Softplus layer
**mlp : dict
    MLP configuration

---
### FunctionDef: `__init__`

Initializes the linear layer.

Parameters
----------
in_channels : int
    Number of features coming from the upstream feature extractor
out_channels : int
    Number of logits to output (always 4, ignores this argument)
**evidential : dict
    Evidential configuration

---
### FunctionDef: `__init__`

Initializes the matching post-processor.

Parameters
----------
fragment: Union[bool, dict], optional
    Matching flag or configuration for fragments
particle: Union[bool, dict], optional
    Matching flag or configuration for particles
interaction: Union[bool, dict], optional
    Matching flag or configuration for interactions
truth_point_mode : str, default 'points'
    Type of truth points to use to do the matching
**kwargs : dict, optional
    Matching parameters shared between all matching processes

---
### FunctionDef: `__init__`

Initializes the message passing network.

Parameters
----------
node_feats : int, default 0
    Number of node features
node_layer : dict, optional
    Configuration of the node features update layer
edge_feats : int, default 0
    Number of edge features
edge_layer : dict, optional
    Configuration of the edge features update layer
global_feats : int, default 0
    Number of global features
global_layer : dict, optional
    Configuration of the global features update layer
num_mp : int, default 3
    Number of message passing steps (node/edge/global feature updates)
input_normalization : union[str, dict], default 'batch_norm'
    Input node/edge/global feature ormalization function configuration

---
### FunctionDef: `__init__`

Initializes the segmentation loss

Parameters
----------
uresnet : dict
    Model configuration
uresnet_loss : dict
    Loss configuration

---
### FunctionDef: `__init__`

Initializes the sparse residual CNN encoder.

Passes most of the configuration along to the underlying sparse
residual CNN encoder defined in :class:`UResNetEncoder`.

Parameters
----------
coord_conv : bool, default False
    Whether to include normalized coordinates in the input features
pool_mode : str, default 'avg'
    Final pooling operation mode ('avg', 'max' or 'conv'
feature_size : int, default 512
    Number of features produced after the final pooling
**cfg : dict, optional
    Configuration to pass along to the sparse residual encoder

---
### FunctionDef: `__init__`

Initializes the standalone PPN loss.

Parameters
----------
uresnet : dict
    Dictionary of the backbone uresnet configuration
ppn : dict
    Model configuration
uresnet_loss : dict, optional
    UResNet loss configuration
ppn_loss : dict, optional
    PPN loss configuration

---
### FunctionDef: `__init__`

Initializes the standalone PPN network.

Parameters
----------
uresnet : dict
    Dictionary of the backbone uresnet configuration
ppn : dict
    Model configuration
uresnet_loss : dict, optional
    UResNet loss configuration
ppn_loss : dict, optional
    PPN loss configuration

---
### FunctionDef: `__init__`

Initializes the standalone UResNet model.

Parameters
----------
uresnet : dict
    Model configuration
uresnet_loss : dict, optional
    Loss configuration

---
### FunctionDef: `__init__`

Initializes the underlying detector :class:`Geometry` object.

Parameters
----------
detector : str, optional
    Name of a recognized detector to the geometry from
file_path : str, optional
    Path to a `.yaml` geometry configuration
detector_coords : bool, default False
    If False, the coordinates are converted to pixel indices

---
### FunctionDef: `__init__`

Instantiates the LArCVDataset.

Parameters
----------
schema : dict
    A dictionary of (string, dictionary) pairs. The key is a unique
    name of a data chunk in a batch and the associated dictionary
    must include:
      - parser: name of the parser
      - args: (key, value) pairs that correspond to parser argument
        names and their values
dtype : str
    Data type to cast the input data to (to match the downstream model)
augment : dict, optional
    Augmentation strategy configuration
**kwargs : dict, optional
    Additional arguments to pass to the LArCVReader class

---
### FunctionDef: `__init__`

Intialize the Graph-SPICE loss.

Parameters
----------
graph_spice : dict
    Graph-SPICE configuration dictionary
graph_spice_loss : dict
    Graph-SPICE loss configuration dictionary

---
### FunctionDef: `__init__`

Intialize the TPC module.

Parameters
----------
positions : np.ndarray
    (N_t) List of TPC center positions, one per TPC
dimensions : np.ndarray
    (3) Dimensions of one TPC
drift_dirs : np.ndarray, optional
    (N_t, 3) List of drift directions. If this is not provided, it is
    inferred from the module configuration, provided that the module
    is composed of two TPCs with a shared cathode.

---
### FunctionDef: `__init__`

Intialize the image classification loss.

Parameters
----------
classifier : dict
    Image classifier configuration
classifier_loss : dict, optional
    Image classifier loss configuration

---
### FunctionDef: `__init__`

Load the calibration maps.

Parameters
----------
lifetime_db : str
    Path to a SQLite db file which maps [run, cryo, tpc] sets onto
    a specific transparency calibration map.
num_tpcs : int
    Number of TPCs in the detector
value_key: str, default 'scale'
    Database key which provides the calibration factor

---
### FunctionDef: `__init__`

Load the information needed to make a lifetime correction.

Parameters
----------
num_tpcs : int
    Number of TPCs in the detector
lifetime : Union[float, list], optional
    Specifies the electron lifetime in microseconds. If `list`, it
    should map a tpc ID onto a specific value.
driftv : Union[float, list], optional
    Specifies the electron drift velocity in cm/us. If `dict`, it
    should map a tpc ID onto a specific value.
lifetime_db : str, optional
    Path to a SQLite db file which maps [run, cryo, tpc] sets onto
    a specific lifetime value in microseconds.
driftv_db : str, optional
    Path to a SQLite db file which maps [run, cryo, tpc] sets onto
    a specific electron drift velocity value in cm/us.

---
### FunctionDef: `__init__`

Loops over data product names, stores them.

Parameters
----------
dtype : str
    Data type to cast the input data to
**kwargs : dict, optional
    Keyword arguments passed to the parser function

Notes
-----
All parser argument which correspond to the name of a tree in the
LArCV file must be contain either the `_event` or `_event_list` suffix.

---
### FunctionDef: `__init__`

Parse the CRT detector configuration.

The assumption here is that the CRT detectors collectively cover the
entire detector, regardless of TPC/optical modularization.

Parameters
----------
dimensions : List[List[float]]
    Dimensions of each of the CRT plane
positions : List[List[float]]
    Positions of each of the CRT plane
norms : List[int]
    Axis along which each of the CRT plane norm is pointing
logical_ids : List[int], optional
    Logical index corresponding to each CRT channel. If not specified,
    it is assumed that there is a one-to-one correspondance between
    physical and logical CRT planes.

---
### FunctionDef: `__init__`

Parse the detector boundary configuration.

Parameters
----------
dimensions : List[float]
    (3) Dimensions of one TPC
positions : List[List[float]]
    (N_t) List of TPC center positions, one per TPC
module_ids : List[int]
    (N_t) List of the module IDs each TPC belongs to
det_ids : List[int], optional
    (N_c) Index of the physical detector which corresponds to each
    logical ID. This is needed if a TPC is divided into multiple logical
    IDs. If this is not specified, it assumed that there is a one-to-one
    correspondance between logical and physical.
drift_dirs : List[List[float]], optional
    (N_t) List of drift direction vectors. If this is not provided, it
    is inferred from the module configuration, provided that modules
    are composed of two TPCs (with a shared cathode)

---
### FunctionDef: `__init__`

Parse the optical detector configuration.

Parameters
----------
volume : str
    Optical decteor segmentation (per 'tpc' or per 'module')
volume_offsets : np.ndarray
    Offsets of the optical volumes w.r.t. to the origin
shape : Union[str, List[str]]
    Optical detector geomtry (combination of 'ellipsoid' and/or 'box')
dimensions : Union[List[float], List[List[float]]]]
    (N_o, 3) List of optical detector dimensions along each axis
    (either the ellipsoid axis lenghts or the box edge lengths)
positions : List[List[float]]
    (N_o, 3) Positions of each of the optical detectors
shape_ids : List[int], optional
    (N_o) If there is different types of optical detectors, specify
    which type each of the index corresponds to
det_ids : List[int], optional
    (N_c) If there are multiple readout channels which contribute to each
    physical optical detector, map each channel onto a physical detector
global_index : bool, default False
    If `True`, the flash objects have a `pe_per_ch` attribute which refers
    to the entire index of optical detectors, rather than one volume
mirror : bool, default False
    If True, mirror the z positons of the optical modules in the second
    TPC of each module

---
### FunctionDef: `__init__`

Post-processor to merge tracks into showers.

Parameters
----------
angle_threshold : float, default 0.95
    Check if track and shower cosine similarity is greater than this value.
adjacency_threshold : float, default 0.5
    Check if track and shower is within this threshold distance.
dedx_limit : int, default -1
    Check if the track dedx is below this value,
    to avoid merging protons.
track_length_limit : int, default 40
    Check if track length is below this value,
    to avoid merging long tracks.

---
### FunctionDef: `__init__`

Process the model configuration.

Parameters
----------
name : str
    Name of the model as specified under spine.model.factories
modules : dict
    Dictionary of modules that make up the model
network_input : List[str]
    List of keys of parsed objects to input into the model forward
loss_input : List[str], optional
    List of keys of parsed objects to input into the loss forward
weight_path : str, optional
    Path to global model weights to load
calibration : dict, optional
    Model score calibration configuration
to_numpy : int, default False
    Cast model output to numpy ndarray
time_dependant_loss : bool, default False
    Handles time-dependant loss, such as KL divergence annealing
train : dict, default None
    Training regimen configuration
dtype : str, default 'float32'
    Data type of the model parameters and input data 
distributed : bool, default False
    Whether the model is part of a distributed training process
rank : int, optional
    Process rank in a torch distributed process
detect_anomaly : bool, default False
    Whether to attempt to detect a torch anomaly
find_unused_parameters : bool, default False
    Attempts to detect unused model parameters in the forward pass

---
### FunctionDef: `__init__`

Shared initializations across all types of batched data.

Parameters
----------
data : Union[np.ndarray, torch.Tensor]
    Batched data
is_sparse : bool, default False
    If initializing from an ME sparse data, flip to True
is_list : bool, default False
    Whether the underlying data is a list of tensors

---
### FunctionDef: `__init__`

Specify the EM shower conversion distance threshold and
the type of vertex to use for the distance calculation.

Parameters
----------
threshold : float, default -1.0
    If EM shower has a conversion distance greater than this,
    its PID will be changed to PHOT_PID.

---
### FunctionDef: `__init__`

Specify the EM shower conversion distance threshold and
the type of vertex to use for the distance calculation.

Parameters
----------
threshold : float, default -1.0
    If EM shower has a conversion distance greater than this,
    its PID will be changed to PHOT_PID.
vertex_mode : str, default 'vertex'
    The type of vertex to use for the distance calculation.
    'protons': Distance between the shower startpoint and the
    closest proton/pion point.
    'vertex_points': Distance between the vertex and all shower points.
    'vertex_startpoint': Distance between the vertex and the predicted
    shower startpoint.

---
### FunctionDef: `__init__`

Specify the threshold for the number of arms of showers.

Parameters
----------
threshold : float, default 70 (deg)
    If the electron shower's leading and subleading angle are
    separated by more than this, the shower is considered to be
    invalid and its PID will be changed to PHOT_PID.
min_samples : int, default 20
    The number of samples (or total weight) in a neighborhood 
    for a point to be considered as a core point (DBSCAN).
eps : float, default 0.02
    Maximum distance between two samples for one to be considered
    as in the neighborhood of the other (DBSCAN).

---
### FunctionDef: `__init__`

Store information about how to enforce neutrino logic.

Parameters
----------
method : str, default 'size'
    Method used to select the lepton: select the largest MIP
    ('size') or the MIP with the highest lepton score ('score')
cc_only : bool, default `True`
    If there are no leptons but MIPs are present, ensure that one
    of the MIPs is labeled as a lepton (CC-like)

---
### FunctionDef: `__init__`

Store information about which particle properties should
or should not be updated.

Parameters
----------
enforce_pid : bool, default True
    Enforce the PID prediction based on the semantic type
enforce_primary : bool, default True
    Enforce the primary prediction based on the semantic type

---
### FunctionDef: `__init__`

Store the `get_ppn_predictions` keyword arguments.

Parameters
----------
assign_to_particles: bool, default False
    If `True`, will assign PPN candidates to particle objects
restrict_shape : bool, default False
    If `True`, only associate PPN candidates with compatible shape
match_threshold : float, default 2.
    Maximum distance required to assign ppn point to particle
**ppn_pred_cfg : dict, optional
    Keyword arguments to pass to the `PPNPredictor` class

Returns
-------
dict
    Update result dictionary containing 'ppn_candidates' key

---
### FunctionDef: `__init__`

Store the necessary attributes to do CSDA range-based estimation.

Parameters
----------
tracking_mode : str, default 'step_next'
    Method used to compute the track length (one of 'displacement',
    'step', 'step_next', 'bin_pca' or 'spline')
include_pids : list, default [2, 3, 4, 5]
    Particle species to compute the kinetic energy for
fill_per_pid : bool, default False
    If `True`, compute the CSDA KE estimate under all PID assumptions
**kwargs : dict, optional
    Additional arguments to pass to the tracking algorithm

---
### FunctionDef: `__init__`

Store the necessary attributes to do MCS-based estimations.

Parameters
----------
tracking_mode : str, default 'bin_pca'
    Method used to compute the segment angles (one of 'step',
    'step_next' or 'bin_pca')
segment_length : float, default 5.0 cm
    Segment length in the units that specify the coordinates
split_angle : bool, default False
    Whether or not to project the 3D angle onto two 2D planes
res_a : float, default 0.25 rad*cm^res_b
    Parameter a in the a/dx^b which models the angular uncertainty
res_b : float, default 1.25
    Parameter b in the a/dx^b which models the angular uncertainty
include_pids : list, default [2, 3, 4, 5]
    Particle species to compute the kinetic energy for
fill_per_pid : bool, default False
    If `True`, compute the MCS KE estimate under all PID assumptions
only_uncontained : bool, default False
    Only run the algorithm on particles that are not contained
**kwargs : dict, optiona
    Additional arguments to pass to the tracking algorithm

---
### FunctionDef: `__init__`

Store the necessary attributes to do template-based PID prediction.

Parameters
----------
fill_per_pid : bool, default False
    If `True`, stores the scores associated with each PID candidate
**identifier : dict, optional
    Particle template identifier configuration parameters

---
### FunctionDef: `__init__`

Store the new thresholds to be used to update interaction topologies.

Parameters
----------
ke_thresholds : Union[float, dict]
    If a scalr, it specifies a blanket KE cut to apply to all
    particles. If it is a dictionary, it maps an PID to a KE threshold.
    If a 'default' key is provided, it is used for all particles,
    unless a number is provided for a specific PID.
reco_ke_mode : str, default 'ke'
    Which `Particle` attribute to use to apply the KE thresholds
truth_ke_mode : str, default 'energy_deposit'
    Which `TruthParticle` attribute to use to apply the KE thresholds

---
### FunctionDef: `__init__`

Store the new thresholds to be used to update the PID and primary
information of particles.

Parameters
----------
shower_pid_thresholds : dict, optional
    Dictionary which maps an EM PID output to a threshold value,
    in order
track_pid_thresholds : dict, optional
    Dictionary which maps a track PID output to a threshold value,
    in order
primary_treshold : float, optional
    Primary score above which a particle is considered a primary

---
### FunctionDef: `__init__`

Store the particle direction recosntruction parameters.

Parameters
----------
neighborhood_radius : float, default 5
    Max distance between start voxel and other voxels
optimize : bool, default True
    Optimizes the number of points involved in the estimate

---
### FunctionDef: `__init__`

Stores the ADC to MeV conversion factor.

Parameters
----------
scaling : Union[float, str], default 1.
    Global scaling factor for the depositions (can be an expression)
shower_fudge : Union[float, str], default 1.
    Shower energy fudge factor (accounts for missing cluster energy)

---
### FunctionDef: `__iter__`

Iterates over bootstrapped batches of data randomly picked
from the dataset.

---
### FunctionDef: `__iter__`

Iterates over sequential batches of data randomly located
in the dataset.

---
### FunctionDef: `__iter__`

Iterates over sequential batches of data.

---
### FunctionDef: `__iter__`

Overrides the basic iterator with one that takes into account
the number of replicas and the rank of the sampler.

---
### FunctionDef: `__iter__`

Placeholder to be overridden by children classes.

---
### FunctionDef: `__iter__`

Resets an iterator counter, return self.

Returns
-------
Module
    The module itself

---
### FunctionDef: `__iter__`

Resets an iterator counter, return self.

Returns
-------
TPCDetector
    The module itself

---
### FunctionDef: `__iter__`

Resets the counter and returns itself.

Returns
-------
object
    The Driver itself

---
### FunctionDef: `__len__`

Provides the full length of the sampler.

The length of the sampler can differ from the number of elements in
the underlying dataset, if the last batch is smaller than the requested
size and is dropped.

Returns
-------
int
    Total number of entries to sample

---
### FunctionDef: `__len__`

Provides the number of elements of the dataset.

Returns
-------
int
    Number of elements in the dataset

---
### FunctionDef: `__len__`

Returns the lenght of the dataset (in number of batches).

Returns
-------
int
    Number of entries in the dataset

---
### FunctionDef: `__len__`

Returns the number of TPCs in the module.

Returns
-------
int
    Number of TPCs in the module

---
### FunctionDef: `__len__`

Returns the number of entries in the file(s).

Returns
-------
int
    Number of entries in the file

---
### FunctionDef: `__len__`

Returns the number of entries that make up the batch.

---
### FunctionDef: `__len__`

Returns the number of events in the underlying reader object.

Returns
-------
int
    Number of elements in the underlying loader/reader.

---
### FunctionDef: `__len__`

Returns the number of modules in the detector.

Returns
-------
int
    Number of modules in the detector

---
### FunctionDef: `__next__`

Defines how to process the next Module in the detector.

Returns
-------
Module
    Next Module instance in the list

---
### FunctionDef: `__next__`

Defines how to process the next TPC in the module.

Returns
-------
Chamber
    Next Chamber instance in the list

---
### FunctionDef: `__next__`

Defines how to process the next entry in the iterator.

Returns
-------
Union[dict, List[dict]]
    Either one combined data dictionary, or one per entry in the batch

---
### FunctionDef: `__post_init__`

Check that the values provided are valid.

---
### FunctionDef: `__post_init__`

Immediately called after building the class attributes.

Makes sure the units are not binary and that they are recognized.

---
### FunctionDef: `__post_init__`

Immediately called after building the class attributes.

Provides two functions:
- Gives default values to array-like attributes. If a default value was
  provided in the attribute definition, all instances of this class
  would point to the same memory location.
- Casts strings when they are provided as binary objects, which is the
  format one gets when loading string from HDF5 files.

---
### FunctionDef: `__repr__`

Representation of the noamlization layer.

This includes the parameters of the layer.

---
### FunctionDef: `__setstate__`

Load optimizer state.

Parameters
----------
state : object
    Optimizer state dictionary

---
### FunctionDef: `__str__`

Human-readable string representation of the fragment object.

Results
-------
str
    Basic information about the fragment properties

---
### FunctionDef: `__str__`

Human-readable string representation of the fragment object.

Results
-------
str
    Basic information about the fragment properties

---
### FunctionDef: `__str__`

Human-readable string representation of the fragment object.

Results
-------
str
    Basic information about the fragment properties

---
### FunctionDef: `__str__`

Human-readable string representation of the interaction object.

Results
-------
str
    Basic information about the interaction properties

---
### FunctionDef: `__str__`

Human-readable string representation of the interaction object.

Results
-------
str
    Basic information about the interaction properties

---
### FunctionDef: `__str__`

Human-readable string representation of the interaction object.

Results
-------
str
    Basic information about the interaction properties

---
### FunctionDef: `__str__`

Human-readable string representation of the particle object.

Results
-------
str
    Basic information about the particle properties

---
### FunctionDef: `__str__`

Human-readable string representation of the particle object.

Results
-------
str
    Basic information about the particle properties

---
### FunctionDef: `__str__`

Human-readable string representation of the particle object.

Results
-------
str
    Basic information about the particle properties

---
### FunctionDef: `__sub__`

Overload the substraction operator.

Parameters
----------
time : Time
    Other Time object

Returns
-------
Time
   Substracted times

---
### FunctionDef: `_build_reco`

Builds :class:`RecoFragment` objects from the full chain output.

Parameters
----------
points : np.ndarray
    (N, 3) Set of deposition coordinates in the image
depositions : np.ndarray
    (N) Set of deposition values
fragment_clusts : List[np.ndarray]
    (P) List of indexes, each corresponding to a fragment instance
fragment_shapes : np.ndarray
    (P) List of fragment shapes (shower, track, etc.)
fragment_start_points : np.ndarray, optional
    (P, 3) List of fragment start point coordinates
fragment_end_points : np.ndarray, optional
    (P, 3) List of fragment end point coordinates
fragment_group_pred : np.ndarray, optional
    (P) Interaction group each fragment belongs to
sources : np.ndarray, optional
    (N, 2) Tensor which contains the module/tpc information

Returns
-------
List[RecoFragment]
    List of constructed reconstructed fragment instances

---
### FunctionDef: `_build_reco`

Builds :class:`RecoInteraction` objects from the full chain output.

This class builds an interaction by assembling particles together.

Parameters
----------
reco_particles : List[RecoParticle]
    List of reconstructed particle objects

Returns
-------
List[RecoInteraction]
    List of constructed reconstructed interaction instances

---
### FunctionDef: `_build_reco`

Builds :class:`RecoParticle` objects from the full chain output.

Parameters
----------
points : np.ndarray
    (N, 3) Set of deposition coordinates in the image
depositions : np.ndarray
    (N) Set of deposition values
particle_clusts : List[np.ndarray]
    (P) List of indexes, each corresponding to a particle instance
particle_shapes : np.ndarray
    (P) List of particle shapes (shower, track, etc.)
particle_start_points : np.ndarray
    (P, 3) List of particle start point coordinates
particle_end_points : np.ndarray
    (P, 3) List of particle end point coordinates
particle_group_pred : np.ndarray
    (P) Interaction group each particle belongs to
particle_node_type_pred : np.ndarray
    (P, N_c) Particle identification logits
particle_node_primary_pred : np.ndarray
    (P, 2) Particle primary classification logits
particle_node_orient_pred : np.ndarray, optional
    (P, 2) Particle orientation classification logits
sources : np.ndarray, optional
    (N, 2) Tensor which contains the module/tpc information
reco_fragments : List[RecoFragment], optional
    (F) List of reconstructed fragments

Returns
-------
List[RecoParticle]
    List of constructed reconstructed particle instances

---
### FunctionDef: `_build_truth`

Builds :class:`TruthFragment` objects from the full chain output.

Parameters
----------
label_tensor : np.ndarray
    Tensor which contains the cluster labels of each deposition
points_label : np.ndarray
    (N', 3) Set of deposition coordinates in the label image (identical
    for pixel TPCs, different if deghosting is involved)
depositions_label : np.ndarray
    (N') Set of true deposition values in MeV
depositions_q_label : np.ndarray, optional
    (N') Set of true deposition values in ADC, if relevant
label_adapt_tensor : np.ndarray, optional
    Tensor which contains the cluster labels of each deposition,
    adapted to the semantic segmentation prediction.
points : np.ndarray, optional
    (N, 3) Set of deposition coordinates in the image
depositions : np.ndarray, optional
    (N) Set of deposition values
label_tensor_g4 : np.ndarray, optional
    Tensor which contains the cluster labels of each deposition
    in the Geant4 image (before the detector simulation)
points_g4 : np.ndarray, optional
    (N'', 3) Set of deposition coordinates in the Geant4 image
depositions_g4 : np.ndarray, optional
    (N'') Set of deposition values in the Geant4 image
sources_label : np.ndarray, optional
    (N', 2) Tensor which contains the label module/tpc information
sources : np.ndarray, optional
    (N, 2) Tensor which contains the module/tpc information
particles : List[Particle], optional
    List of true particles

Returns
-------
List[TruthFragment]
    List of constructed true fragment instances

---
### FunctionDef: `_build_truth`

Builds :class:`TruthInteraction` objects from the full chain output.

This class builds an interaction by assembling particles together.

Parameters
----------
truth_particles : List[TruthParticle]
    List of truth particle objects
neutrinos : List[Neutrino], optional
    List of true neutrino information from the generator

---
### FunctionDef: `_build_truth`

Builds :class:`TruthParticle` objects from the full chain output.

Parameters
----------
particles : List[Particle]
    List of true particles
label_tensor : np.ndarray
    Tensor which contains the cluster labels of each deposition
points_label : np.ndarray
    (N', 3) Set of deposition coordinates in the label image (identical
    for pixel TPCs, different if deghosting is involved)
depositions_label : np.ndarray
    (N') Set of true deposition values in MeV
depositions_q_label : np.ndarray, optional
    (N') Set of true deposition values in ADC, if relevant
label_adapt_tensor : np.ndarray, optional
    Tensor which contains the cluster labels of each deposition,
    adapted to the semantic segmentation prediction.
points : np.ndarray, optional
    (N, 3) Set of deposition coordinates in the image
depositions : np.ndarray, optional
    (N) Set of deposition values
label_tensor_g4 : np.ndarray, optional
    Tensor which contains the cluster labels of each deposition
    in the Geant4 image (before the detector simulation)
points_g4 : np.ndarray, optional
    (N'', 3) Set of deposition coordinates in the Geant4 image
depositions_g4 : np.ndarray, optional
    (N'') Set of deposition values in the Geant4 image
sources_label : np.ndarray, optional
    (N', 2) Tensor which contains the label module/tpc information
sources : np.ndarray, optional
    (N, 2) Tensor which contains the module/tpc information
graph_label : np.ndarray, optional
    (E, 2) Parentage relations in the set of particles
truth_fragments : List[TruthFragment], optional
    (F) List of true fragments

Returns
-------
List[TruthParticle]
    List of restored true particle instances

---
### FunctionDef: `_end_point_trace`

Scatters the end points of the requested object type.

Parameters
----------
obj_name : str
    Name of the object to draw
color : Union[str, np.ndarray], optional
    Color of markers/lines or (N) list of color of markers/lines
markersize : float, default 5
    Marker size
marker_symbol : float, default 'circle-open'
    Marker style
**kwargs : dict, optional
    Additional parameters to pass

Returns
-------
list
    List of end point traces

---
### FunctionDef: `_flash_trace`

Draw the cumlative PEs of flashes that have been matched to
interactions specified by `obj_name`.

Parameters
----------
obj_name : str
    Name of the object to draw
matched_only : bool
    If `True`, only flashes matched to interactions are drawn
**kwargs : dict, optional
    List of additional arguments to pass to :func:`optical_traces`

Returns
-------
list
    List of optical detector traces

---
### FunctionDef: `_get_activation_fn`

Return an activation function given a string

---
### FunctionDef: `_is_contained`

Parameters
----------
points: np.ndarray
    Shape (N, 3). Coordinates in voxel units.
threshold: float or np.ndarray
    Distance (in voxels) from boundaries beyond which
    an object is contained. Can be an array if different
    threshold must be applied in x, y and z (shape (3,)).

Returns
-------
bool

---
### FunctionDef: `_load_reco`

Construct :class:`RecoParticle` objects from their stored versions.

Parameters
----------
reco_particles : List[RecoParticle]
    (P) List of partial reconstructed particles
points : np.ndarray
    (N, 3) Set of deposition coordinates in the image
depositions : np.ndarray
    (N) Set of deposition values
sources : np.ndarray, optional
    (N, 2) Tensor which contains the module/tpc information

Returns
-------
List[RecoParticle]
    List of restored reconstructed particle instances

---
### FunctionDef: `_load_reco`

Load :class:`RecoFragment` objects from their stored versions.

Parameters
----------
reco_fragments : List[RecoFragment]
    (F) List of partial reconstructed fragments
points : np.ndarray
    (N, 3) Set of deposition coordinates in the image
depositions : np.ndarray
    (N) Set of deposition values
sources : np.ndarray, optional
    (N, 2) Tensor which contains the module/tpc information

Returns
-------
List[RecoFragment]
    List of restored reconstructed fragment instances

---
### FunctionDef: `_load_reco`

Load :class:`RecoInteraction` objects from their stored versions.

Parameters
----------
reco_interactions : List[RecoInteraction]
    List of partial reconstructed interaction objects
reco_particles : List[RecoParticle]
    List of reconstructed particle objects

Returns
-------
List[RecoInteraction]
    List of restored reconstructed interaction instances

---
### FunctionDef: `_load_truth`

Construct :class:`TruthParticle` objects from their stored versions.

Parameters
----------
truth_particles : List[TruthParticle]
    (P) List of partial truth particles
points_label : np.ndarray
    (N', 3) Set of deposition coordinates in the label image (identical
    for pixel TPCs, different if deghosting is involved)
depositions_label : np.ndarray
    (N') Set of true deposition values in MeV
depositions_q_label : np.ndarray, optional
    (N') Set of true deposition values in ADC, if relevant
points : np.ndarray, optional
    (N, 3) Set of deposition coordinates in the image
depositions : np.ndarray, optional
    (N) Set of deposition values
points_g4 : np.ndarray, optional
    (N'', 3) Set of deposition coordinates in the Geant4 image
depositions_g4 : np.ndarray, optional
    (N'') Set of deposition values in the Geant4 image
sources_label : np.ndarray, optional
    (N', 2) Tensor which contains the label module/tpc information
sources : np.ndarray, optional
    (N, 2) Tensor which contains the module/tpc information

Returns
-------
List[TruthParticle]
    List of restored true particle instances

---
### FunctionDef: `_load_truth`

Load :class:`TruthFragment` objects from their stored versions.

Parameters
----------
truth_fragments : List[TruthFragment]
    (F) List of partial truth fragments
points_label : np.ndarray
    (N', 3) Set of deposition coordinates in the label image (identical
    for pixel TPCs, different if deghosting is involved)
depositions_label : np.ndarray
    (N') Set of true deposition values in MeV
depositions_q_label : np.ndarray, optional
    (N') Set of true deposition values in ADC, if relevant
points : np.ndarray, optional
    (N, 3) Set of deposition coordinates in the image
depositions : np.ndarray, optional
    (N) Set of deposition values
points_g4 : np.ndarray, optional
    (N'', 3) Set of deposition coordinates in the Geant4 image
depositions_g4 : np.ndarray, optional
    (N'') Set of deposition values in the Geant4 image
sources : np.ndarray, optional
    (N, 2) Tensor which contains the module/tpc information
sources_label : np.ndarray, optional
    (N', 2) Tensor which contains the label module/tpc information

Returns
-------
List[TruthFragment]
    List of restored true fragment instances

---
### FunctionDef: `_load_truth`

Load :class:`TruthInteraction` objects from their stored versions.

Parameters
----------
data : dict
    Dictionary of data products

Parameters
----------
truth_interactions : List[TruthInteraction]
    List of partial truth interaction objects
truth_particles : List[TruthParticle]
    List of truth particle objects

Returns
-------
List[TruthInteraction]
    List of restored truth interaction instances

---
### FunctionDef: `_object_colors`

Provides an appropriate colorscale and range for a given attribute.

Parameters
----------
obj_name : str
    Name of the object to draw
attr : Union[str, List[str]]
    Attribute name(s) used to set the color/hovertext
color_attr : str
    Name of the attribute to use to determine the color
split_traces : bool
    If `True`, one trace is produced for each object

Returns
-------
dict
    Dictionary of color parameters (colorscale, cmin, cmax)

---
### FunctionDef: `_object_traces`

Draw a specific object.

Parameters
----------
obj_name : str
    Name of the objects to be represented
attr : Union[str, List[str]]
    Attribute name(s) used to set the color/hovertext
color_attr : str
    Name of the attribute to use to determine the color
split_traces : bool
    If `True`, one trace is produced for each object

Returns
-------
List[plotly.graph_objs.Scatter3d]
    List of traces, one per object being drawn up

---
### FunctionDef: `_point_trace`

Scatters a set of discrete points per object instance.

Parameters
----------
obj_name : str
    Name of the object to draw
point_attr : str
    Name of the attribute specifying end point to draw
**kwargs : dict, optional
    List of additional arguments to pass to :func:`scatter_points`

Returns
-------
list
    List of point traces

---
### FunctionDef: `_raw_trace`

Draws the raw input image (pre-reconstruction).

Returns
-------
List[plotly.graph_objs.Scatter3d]
    List of one trace containing the input to the reconstruction

---
### FunctionDef: `_start_point_trace`

Scatters the start points of the requested object type.

Parameters
----------
obj_name : str
    Name of the object to draw
color : Union[str, np.ndarray], optional
    Color of markers/lines or (N) list of color of markers/lines
markersize : float, default 5
    Marker size
marker_symbol : float, default 'circle'
    Marker style
**kwargs : dict, optional
    Additional parameters to pass

Returns
-------
list
    List of start point traces

---
### FunctionDef: `_unwrap`

Routes set of data to the appropriate unwrapping scheme.

Parameters
----------
key : str
    Name of the data product to unwrap
data : list
    Data product

---
### FunctionDef: `_unwrap_index`

Unwrap an index list into its constituents.

Parameters
----------
data : IndexBatch
    Index batch product

---
### FunctionDef: `_unwrap_tensor`

Unwrap a batch of tensors into its constituents.

Parameters
----------
data : TensorBatch
    Tensor batch product

---
### FunctionDef: `_vertex_trace`

Scatters the vertex of the requested object type.

Parameters
----------
obj_name : str
    Name of the object to draw
color : Union[str, np.ndarray], optional
    Color of markers/lines or (N) list of color of markers/lines
markersize : float, default 10
    Marker size
marker_symbol : float, default 'circle-open'
    Marker style
**kwargs : dict, optional
    Additional parameters to pass

Returns
-------
list
    List of vertex point traces

---
### ClassDef: `AbstractBatchSampler`

Abstract sampler class.

Samplers that inherit from this class should work out of the box.
Just define the __len__ and __iter__ functions. __init__ defines
self.num_samples and self.batch_size as well as a self._random
RNG, if needed.

---
### FunctionDef: `act_dict`

Dictionary of recognized activation functions.

---
### FunctionDef: `act_dict`

Dictionary of valid activation functions.

---
### FunctionDef: `act_factory`

Instantiates an activation layer.

Parameters
----------
cfg : dict
    Activation layer configuration

Return
------
object
    Instantiated activation layer

---
### FunctionDef: `act_factory`

Instantiates an activation layer.

Parameters
----------
cfg : dict
    Activation layer configuration

Return
------
object
    Instantiated activation layer

---
### ClassDef: `AdaBound`

Implements AdaBound algorithm.

It has been proposed in `Adaptive Gradient Methods with Dynamic Bound of
Learning Rate`.

.. Adaptive Gradient Methods with Dynamic Bound of Learning Rate:
    https://openreview.net/forum?id=Bkg3g2R9FX

---
### ClassDef: `AdaBoundW`

Implements AdaBound algorithm with Decoupled Weight Decay (arxiv.org/abs/1711.05101)
It has been proposed in `Adaptive Gradient Methods with Dynamic Bound of Learning Rate`_.
Arguments:
    params (iterable): iterable of parameters to optimize or dicts defining
        parameter groups
    lr (float, optional): Adam learning rate (default: 1e-3)
    betas (Tuple[float, float], optional): coefficients used for computing
        running averages of gradient and its square (default: (0.9, 0.999))
    final_lr (float, optional): final (SGD) learning rate (default: 0.1)
    gamma (float, optional): convergence speed of the bound functions (default: 1e-3)
    eps (float, optional): term added to the denominator to improve
        numerical stability (default: 1e-8)
    weight_decay (float, optional): weight decay (L2 penalty) (default: 0)
    amsbound (boolean, optional): whether to use the AMSBound variant of this algorithm
.. Adaptive Gradient Methods with Dynamic Bound of Learning Rate:
    https://openreview.net/forum?id=Bkg3g2R9FX

---
### FunctionDef: `adapt_labels`

Adapts the cluster labels to account for the predicted semantics.

Points wrongly predicted get the cluster label of the closest touching
cluster, if there is one. Points that are predicted as ghosts get invalid
(-1) cluster labels everywhere.

Instances that have been broken up by the deghosting process get assigned
distinct cluster labels for each effective fragment.

Notes
-----
This function should work on Numpy arrays or Torch tensors.

Uses GPU version from `torch_cluster.knn` to speed up the label adaptation
computation.

Parameters
----------
clust_label : Union[np.ndarray, torch.Tensor]
    (N, N_l) Cluster label tensor
seg_label : List[Union[np.ndarray, torch.Tensor]]
    (M, 5) Segmentation label tensor
seg_pred : Union[np.ndarray, torch.Tensor]
    (M/N_deghost) Segmentation predictions for each voxel
ghost_pred : Union[np.ndarray, torch.Tensor], optional
    (M) Ghost predictions for each voxel
break_classes : List[int], default 
                [SHOWR_SHP, TRACK_SHP, MICHL_SHP, DELTA_SHP]
    Classes to run DBSCAN on to break up
break_eps : float, default 1.1
    Distance scale used in the break up procedure
break_metric : str, default 'chebyshev'
    Distance metric used in the break up produce

Returns
-------
Union[np.ndarray, torch.Tensor]
    (N_deghost, N_l) Adapted cluster label tensor

---
### FunctionDef: `adapt_labels_batch`

Batched version of :func:`adapt_labels`.

Parameters
----------
clust_label : TensorBatch
    (N, N_l) Cluster label tensor
seg_label : TensorBatch
    (M, 5) Segmentation label tensor
seg_pred : TensorBatch
    (M/N_deghost) Segmentation predictions for each voxel
ghost_pred : TensorBatch, optional
    (M) Ghost predictions for each voxel
break_classes : List[int], default 
                [SHOWR_SHP, TRACK_SHP, MICHL_SHP, DELTA_SHP]
    Classes to run DBSCAN on to break up
break_eps : float, default 1.1
    Distance scale used in the break up procedure
break_metric : str, default 'chebyshev'
    Distance metric used in the break up produce

Returns
-------
TensorBatch
    (N_deghost, N_l) Adapted cluster label tensor

---
### FunctionDef: `adapt_volume`

Apply margins from a given volume. Takes care of subtleties
associated with the cathode, if needed.

Parameters
----------
ref_volume : np.ndarray
    (3, 2) Array of volume boundaries
margin : np.ndarray
    Minimum distance from a detector wall to be considered contained as
    [[x_low,x_up], [y_low,y_up], [z_low,z_up]], i.e. distance is
    specified individually of each wall.
cathode_margin : float, optional
    If specified, sets a different margin for the cathode boundaries
module_id : int, optional
    ID of the module
tpc_id : int, optional
    ID of the TPC within the module

Returns
-------
np.ndarray
    (3, 2) Updated array of volume boundaries

---
### FunctionDef: `adjacency_matrix`

Creates a dense adjacency matrix from a list of connected edges in a
graph, i.e. densify the graph incidence matrix.

Parameters
----------
edge_index : np.ndarray
    (2, E) Sparse incidence matrix
num_nodes : int
    Number of nodes in the graph, C

Returns
-------
np.ndarray
    (C, C) Adjacency matrix

---
### FunctionDef: `adjust_positions`

Given a cathode crosser (either in one or two pieces), apply the
necessary position offsets to match it at the cathode.

Parameters
----------
data : dict
    Dictionary of data products
idx_i : int
    Index of a cathode crosser (or a cathode crosser fragment)
idx_j : int, optional
    Index of a matched cathode crosser fragment
truth : bool, default False
    If True, adjust truth object positions

Results
-------
np.ndarray
   (N, 3) Point coordinates

---
### ClassDef: `AGNNConvNodeLayer`

AGNNConv module for extracting graph node features.

This model simply takes a simple attention-based convolution of a node
with all of its neighbors to update the initial node feature vector (N_c),
preserving the original size and returning an updated (N_c) vector.

Source: https://arxiv.org/abs/1803.03735

---
### FunctionDef: `all`

Numba implementation of `np.all(x, axis)`.

Parameters
----------
x : np.ndarray
    (N, M) Array of values
axis : int
    Array axis ID

Returns
-------
np.ndarray
    (N) or (M) array of `all` outputs

---
### FunctionDef: `amax`

Numba implementation of `np.amax(x, axis)`.

Parameters
----------
x : np.ndarray
    (N,M) array of values
axis : int
    Array axis ID

Returns
-------
np.ndarray
    (N) or (M) array of `max` values

---
### FunctionDef: `ami`

Computes the Adjusted Mutual Information (AMI) between two sets of labels.

Parameters
----------
truth : np.ndarray
    (N) Set of true labels
pred : np.ndarray
    (N) Set of predicted labels
batch_ids : np.ndarray, optional
    (N) Batch IDs

Returns
-------
float
    Adjusted Mutual Information (AMI) value

---
### FunctionDef: `amin`

Numba implementation of `np.amin(x, axis)`.

Parameters
----------
x : np.ndarray
    (N,M) array of values
axis : int
    Array axis ID

Returns
-------
np.ndarray
    (N) or (M) array of `min` values

---
### FunctionDef: `ana_script_factory`

Instantiates an analyzer module from a configuration dictionary.

Parameters
----------
name : str
    Name of the analyzer module
cfg : dict
    Analysis script module configuration
parent_path : str
    Path to the parent directory of the main analysis configuration. This
    allows for the use of relative paths in the analyzers.
overwrite : bool, optional
    If `True`, overwrite the CSV logs if they already exist
log_dir : str, optional
    Output CSV file directory (shared with driver log)
prefix : str, optional
    Input file prefix. If requested, it will be used to prefix
    all the output CSV files.

Returns
-------
object
     Initialized analyzer object

---
### ClassDef: `AnaBase`

Parent class of all analysis scripts.

This base class performs the following functions:
- Ensures that the necessary methods exist
- Checks that the script is provided the necessary information
- Writes the output of the analysis to CSV

Attributes
----------
name : str
    Name of the analysis script (to call it from a configuration file)
req_keys : List[str]
    Data products needed to run the analysis script
opt_keys : List[str]
    Optional data products which will be used only if they are provided
units : str
    Units in which the coordinates are expressed

---
### ClassDef: `AnaManager`

Manager class to initialize and execute analysis scripts.

Analysis scripts use the output of the reconstruction chain and the
post-processors and produce simple CSV files.

It loads all the analysis scripts and feeds them data. It initializes
CSV writers needed to store the output of the analysis scripts.

---
### FunctionDef: `angular_loss`

Computes the angular/cosine distance between vectors that join candidate
points to the start points of particles and their respective direction
estimates. Values are normalized between 0 (perfect fit) and 1
(complete disagreement).

Parameters
----------
candidates : np.ndarray
    (C, 3) Vertex coordinates
points : np.ndarray
    (P, 3) Particle start points
directions : np.ndarray
    (P, 3) Particle directions
use_cos : bool
    Whether or not to use the cosine as a metric

Returns
-------
np.ndarray
    (C) Loss for each of the candidates

---
### FunctionDef: `annotate_heatmap`

A function to annotate a heatmap.

Parameters
----------
im
    The AxesImage to be labeled.
data
    Data used to annotate.  If None, the image's data is used.  Optional.
valfmt
    The format of the annotations inside the heatmap.  This should either
    use the string format method, e.g. "$ {x:.2f}", or be a
    `matplotlib.ticker.Formatter`.  Optional.
textcolors
    A pair of colors.  The first is used for values below a threshold,
    the second for those above.  Optional.
threshold
    Value in data units according to which the colors from textcolors are
    applied.  If None (the default) uses the middle of the colormap as
    separation.  Optional.
**kwargs
    All other arguments are forwarded to each call to `text` used to create
    the text labels.

---
### FunctionDef: `anode_pos`

Position of the anode along the drift direction.

Returns
-------
float
    Anode position along the drift direction

---
### FunctionDef: `anode_side`

Returns whether the anode is on the lower or upper boundary of
the TPC along the drift axis (0 for lower, 1 for upper).

Returns
-------
int
    Anode side of the TPC

---
### FunctionDef: `append`

Append the CSV file with the output.

Parameters
----------
result_blob : dict
    Dictionary containing the output of the reconstruction chain

---
### FunctionDef: `append`

Apppend a CSV log file with a set of values.

Parameters
----------
name : str
    Name of the writer
**kwargs : dict
    Dictionary of information to save to the writer

---
### FunctionDef: `append_entry`

Stores one entry.

Parameters
----------
out_file : h5py.File
    HDF5 file instance
data : dict
    Dictionary of data products
batch_id : int
    Batch ID to be stored

---
### FunctionDef: `append_key`

Stores data key in a specific dataset of an HDF5 file.

Parameters
----------
out_file : h5py.File
    HDF5 file instance
event : dict
    Dictionary of objects that make up one event
data : dict
    Dictionary of data products
key : string
    Dictionary key name
batch_id : int
    Batch ID to be stored

---
### FunctionDef: `apply_filter`

Restrict the list of entries.

Parameters
----------
n_entry : int, optional
    Maximum number of entries to load
n_skip : int, optional
    Number of entries to skip at the beginning
entry_list : list, optional
    List of integer entry IDs to add to the index
skip_entry_list : list, optional
    List of integer entry IDs to skip from the index
run_event_list: list((int, int, int)), optional
    List of (run, subrun, event) triplets to add to the index
skip_run_event_list: list((int, int, int)), optional
    List of (run, subrun, event) triplets to skip from the index

---
### FunctionDef: `apply_latex_style`

Sets the necessary :mod:`matplotlib` and :mod:`seaborn` parameters
to draw a plot using latex style.

---
### FunctionDef: `apply_mask`

Apply a global mask to the underlying tensor, update batching.

Parameters
----------
mask : Union[np.ndarray, torch.Tensor]
    (N) Boolean mask to apply to the underlying tensor

---
### FunctionDef: `argmax`

Numba implementation of `np.argmax(x, axis)`.

Parameters
----------
x : np.ndarray
    (N,M) array of values
axis : int
    Array axis ID

Returns
-------
np.ndarray
    (N) or (M) array of `argmax` values

---
### FunctionDef: `argmin`

Numba implementation of `np.argmin(x, axis)`.

Parameters
----------
x : np.ndarray
    (N,M) array of values
axis : int
    Array axis ID

Returns
-------
np.ndarray
    (N) or (M) array of `argmin` values

---
### FunctionDef: `ari`

Computes the Adjusted Rand Index (ARI) between two sets of labels.

Parameters
----------
truth : np.ndarray
    (N) Set of true labels
pred : np.ndarray
    (N) Set of predicted labels
batch_ids : np.ndarray, optional
    (N) Batch IDs

Returns
-------
float
    Adjusted Rand Index (ARI) value

---
### FunctionDef: `array_diff`

Compare the content of two arrays.

This functions returns the elemnts of the first array that
do not appear in the second array.

Parameters
----------
array_x : List[str]
    First array of strings
array_y : List[str]
    Second array of strings

Returns
-------
Set[str]
    Set of keys that appear in `array_x` but not in `array_y`.

---
### FunctionDef: `as_dict`

Returns the data class as dictionary of (key, value) pairs.

Parameters
----------
lite : bool, default False
    If `True`, the `_lite_skip_attrs` are dropped

Returns
-------
dict
    Dictionary of attribute names and their values

---
### ClassDef: `ASPP`

Atrous Spatial Pyramid Pooling.

---
### ClassDef: `AtrousIIBlock`

ResNet-type block with atrous convolutions.

Developed for the ACNN paper: "ACNN: a Full Resolution DCNN for Medical
Image Segmentation"

Original paper: https://arxiv.org/pdf/1901.09203.pdf

---
### FunctionDef: `attach_neutrino`

Attach neutrino generator information to this interaction.

Parameters
----------
neutrino : Neutrino
    Neutrino to fetch the attributes from

---
### ClassDef: `Attention`

Sparse Attention Module where the feature map is multiplied
by a soft masking score tensor (sigmoid activated)

---
### ClassDef: `AttentionMask`

Returns a masked tensor of x according to mask, where the number of
coordinates between x and mask differ.

---
### ClassDef: `Augmenter`

Generic class to handle data augmentation in SPINE.

---
### FunctionDef: `backbone_dict`

Returns dictionary of backbone classes using name keys.

Returns
-------
dict
    Dictionary of available backbones

---
### FunctionDef: `backbone_factory`

Instantiates a backbone model from a configuration dictionary.

Parameters
----------
cfg : dict
    Backbone configuration

Returns
-------
object
    Instantiated backbone function

---
### FunctionDef: `backward`

Run the backward step on the model.

Parameters
----------
loss : torch.tensor
    Scalar loss value to step the model weights

---
### ClassDef: `BarycenterFlashMatcher`

Matches interactions and flashes by matching the charge barycenter of
TPC interactions with the light barycenter of optical flashes.

---
### FunctionDef: `batch_dice_loss`

Compute the DICE loss, similar to generalized IOU for masks
Args:
    inputs: (num_masks, num_points) Tensor
    targets: (num_masks, num_points) Tensor

---
### FunctionDef: `batch_ids`

Returns the batch ID of each element in the full index list.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (N) Complete batch ID array, one per element

---
### FunctionDef: `batch_ids`

Returns the batch ID of each index in the list.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (I) Batch ID array, one per index in the list

---
### FunctionDef: `batch_ids`

Returns the batch ID of each of the elements in the tensor.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (N) Batch ID of each element in the tensor

---
### FunctionDef: `batch_log_dice_loss`

Compute the DICE loss, similar to generalized IOU for masks
Args:
    inputs: (num_masks, num_points) Tensor
    targets: (num_masks, num_points) Tensor

---
### FunctionDef: `batch_sigmoid_ce_loss`

Args:
    inputs: A float tensor of arbitrary shape.
            The predictions for each example.
    targets: A float tensor with the same shape as inputs. Stores the binary
             classification label for each element in inputs
            (0 for the negative class and 1 for the positive class).
Returns:
    Loss tensor

---
### ClassDef: `BatchBase`

Base class for all types of batched data.

Attributes
----------
data : Union[list, np.ndarray, torch.Tensor]
    Batched data
counts : Union[np.ndarray, torch.Tensor]
    (B) Number of data elements in each entry of the batch
edges : Union[np.ndarray, torch.Tensor]
    (B+1) Edges separating the entries in the batch
batch_size : int
    Number of entries that make up the batched data

---
### ClassDef: `BayesianUResNet`

UResNet with Uncertainty Quantification

The backbone model consists of UResNet Encoder-Decoder format with
standard residual layers for the shallow half and dropout residual layers
for the deep half of the network.

Configuration
-------------
mode: str
    string indicator for slight changes in network
    behavior/architecture. Supports three options:

        - standard: standard dropout segmentation network. This also
        includes MCDropout segnet, since training behavior is identical
        for both standard and mcdropout networks.
        - evd: Changes network into evidential segmentation network

num_samples: int
    if used as MCDropout Segnet, the number of stochastic
    forward samples to be taken.

num_classes: int
    number of segmentation classes (default: 5)

---
### FunctionDef: `bd`

Computes the Best Dice (BD) between two sets of labels.

Parameters
----------
truth : np.ndarray
    (N) Set of true labels
truth_unique : np.ndarray
    (K) Set of unique true labels
truth_counts : np.ndarray
    (K) Number of realization of each unique true label
pred : np.ndarray
    (N) Set of predicted labels
pred_unique : np.ndarray
    (L) Set of unique predicted labels
pred_counts : np.ndarray
    (L) Number of realization of each unique predicted label

---
### ClassDef: `BerHuLoss`

Applies the BerHu loss.

---
### FunctionDef: `bethe_bloch_lar`

Bethe-Bloch energy loss function for liquid argon.

Reference:

https://pdg.lbl.gov/2019/reviews/rpp2018-rev-passage-particles-matter.pdf

Corrections taken from:

https://pdg.lbl.gov/2023/AtomicNuclearProperties/adndt.pdf

Parameters
----------
T : float
   Kinetic energy in MeV
M : float
   Impinging particle mass in MeV/c^2
z : int, default 1
   Impinging partile charge in multiples of electron charge

Returns
-------
float
   Value of the energy loss rate in liquid argon in MeV/cm

---
### FunctionDef: `bethe_bloch_mpv_lar`

Most-probable value of energy loss through a thin layer of liquid argon.

https://pdg.lbl.gov/2019/reviews/rpp2018-rev-passage-particles-matter.pdf

Parameters
----------
T : float
   Kinetic energy in MeV
M : float
   Impinging particle mass in MeV/c^2
x : float
   Material thickness in cm
z : int, default 1
   Impinging partile charge in multiples of electron charge

Returns
-------
float
   Value of the energy loss in liquid argon in MeV

---
### FunctionDef: `bias`

Bias parameter of the AdaIN layer.

Note that in AdaptIS, the parameters to the AdaIN layer
are trainable outputs from the controller network.

---
### ClassDef: `BilinearKernel`

Kernel producing edges scores based on a learnable bilinear layer.

---
### FunctionDef: `binary_xloss`

Binary Cross entropy loss
  logits: [B, H, W] Variable, logits at each pixel (between -\infty and +\infty)
  labels: [B, H, W] Tensor, binary ground truth masks (0 or 1)
  ignore: void class id

---
### ClassDef: `BinaryDiceLoss`

Applies the binary Dice Loss.

The Dice loss is derived from the Dice Similarity Coefficient, also known
as the Sorensen–Dice coefficient, which is a statistical measure used to
compare the similarity of two samples.

---
### ClassDef: `BinaryFocalLoss`

Applies the focal loss.

Original Paper: https://arxiv.org/abs/1708.02002

---
### ClassDef: `BinaryLogDiceCELoss`

Applies the binary log Dice loss and the cross-entropy loss.

This class inherits from the :class:`BinaryLogDiceLoss` and adds
a cross-entropy loss on top of it, with some configurable weights.

---
### ClassDef: `BinaryLogDiceCEMincutLoss`

Applies the binary log Dice loss, cross-entropy loss and mincut loss.

This class inherits from the :class:`BinaryLogDiceCELoss` and adds
a mincut loss on top of it, with some configurable weights.

---
### ClassDef: `BinaryLogDiceLoss`

Applies the binary log Dice loss.

This class inherits from the standard :class:`BinaryDiceLoss` and simply
passes it through a logarithm.

---
### ClassDef: `BinaryMincutLoss`

Applies the min-cut loss.

This is a very basic loss of 1. - interesection between the output
probabilities and the target domain.

---
### ClassDef: `BipartiteGraph`

Generates graphs that connect primary nodes to secondary nodes.

See :class:`GraphBase` for attributes/methods shared
across all graph constructors.

---
### FunctionDef: `birks`

Birks equation to calculate electron quenching (higher local energy
deposition are prone to more electron-ion recombination).

Parameters
----------
dedx : Union[float, np.ndarray]
    Value or array of values of dE/dx in MeV/cm

Returns
-------
Union[float, np.ndarray]
   Quenching factors in electrons/MeV

---
### ClassDef: `BootstrapBatchSampler`

Sampler used for bootstrap sampling of the entire dataset.

This is particularly useful for training an ensemble of networks
(bagging).

---
### ClassDef: `Box`

Class which holds all methods associated with a box-shapes component.

Attributes
----------
boundaries : np.ndarray
    (3, 2) Box boundaries
    - 3 is the number of dimensions
    - 2 corresponds to the lower/upper boundaries along each axis

---
### FunctionDef: `box_trace`

Function which produces a plotly trace of a box given its lower bounds
and upper bounds in x, y and z.

Parameters
----------
lower : np.ndarray
    (3) Vector of lower boundaries in x, z and z
upper : np.ndarray
    (3) Vector of upper boundaries in x, z and z
draw_faces : bool, default False
    Weather or not to draw the box faces, or only the edges
line : dict, optional
    Dictionary which specifies box line properties
linewidth : int, optional
    Width of the box edge lines
color : Union[str, np.ndarray], optional
    Color of box
cmin : float, optional
    Minimum value of the color range
cmax : float, optional
    Maximum value of the color range
colorscale : Union[str, dict]
    Colorscale
intensity : Union[int, float], optional
    Color intensity of the box along the colorscale axis
hovertext : Union[int, str, np.ndarray], optional
    Text associated with the box
showscale : bool, default False
    If True, show the colorscale of the :class:`plotly.graph_objs.Mesh3d`
**kwargs : dict, optional
    List of additional arguments to pass to
    :class:`plotly.graph_objs.Scatter3D` or
    :class:`plotly.graph_objs.Mesh3D`, depending on what the `draw_faces`
    parameter is set to.

Returns
-------
Union[plotly.graph_objs.Scatter3D, plotly.graph_objs.Mesh3D]
    Box trace

---
### FunctionDef: `box_traces`

Function which produces a list of plotly traces of boxes given a list of
lower bounds and upper bounds in x, y and z.

Parameters
----------
lowers : np.ndarray
    (N, 3) List of vector of lower boundaries in x, z and z
uppers : np.ndarray
    (N, 3) List of vector of upper boundaries in x, z and z
draw_faces : bool, default False
    Weather or not to draw the box faces, or only the edges
color : Union[str, np.ndarray], optional
    Color of boxes or list of color of boxes
linewidth : int, default 2
    Width of the box edge lines
hovertext : Union[int, str, np.ndarray], optional
    Text associated with every box or each box
cmin : float, optional
    Minimum value along the color scale
cmax : float, optional
    Maximum value along the color scale
shared_legend : bool, default True
    If True, the plotly legend of all boxes is shared as one
legendgroup : str, optional
    Legend group to be shared between all boxes
showlegend : bool, default `True`
    Whether to show legends on not
name : str, optional
    Name of the trace(s)
**kwargs : dict, optional
    List of additional arguments to pass to
    :class:`plotly.graph_objs.Scatter3D` or
    :class:`plotly.graph_objs.Mesh3D`, depending on what the `draw_faces`
    parameter is set to.

Returns
-------
Union[List[plotly.graph_objs.Scatter3D], List[plotly.graph_objs.Mesh3D]]
    Box traces

---
### FunctionDef: `build_graph`

Construct a graph for a single batch id and semantic class that
will be used for connected components clustering.

Parameters
----------
coords : torch.Tensor
    (N, 3) Tensor of point coordinates
features : torch.Tensor
    (N, N_f) Graph embedding features to be used for edge prediction
seg_clusts : List[List[int]]
    (S) One pixel index per semantic type
seg_label : torch.Tensor
    (N, 1 + D + 1) Tensor of segmentation labels
    - 1 is the segmentation label
clust_label : torch.Tensor, optional
    (N, 1 + D + N_c) Tensor of cluster labels
    - N_c is is the number of cluster labels

Returns
-------
Dict[str, torch.Tensor]
    Dictionary of graph properties

---
### FunctionDef: `build_groups`

Use groups predictions from GrapPA to build superstructures.

Parameters
----------
clusts : IndexBatch
    List of clusters to aggregate using GrapPA
clust_shapes : TensorBatch
    Semantic type of each of the clusters
group_pred : TensorBatch
    Group ID of each node in the GraPA output
primary_mask : TensorBatch
    Binary mask as to whether a node is a group primary or not
aggregate_shapes : bool, default False
    Combine shapes to give a shape to the aggregated object
shape_use_primary : bool, default False
    Use primary shape as the group shape
retain_primaries : bool, default False
    Retain the primary cluster in the aggregated group

Returns
-------
groups : IndexBatch
    List of cluster groups aggregated using GrapPA
group_shapes : TensorBatch
    Semantic type of each of the cluster groups
group_primaries : IndexBatch
    List of primary clusters for each group

---
### FunctionDef: `build_matrix`

Builds a confusion matrix from a pixel-wise storage file.

Parameters
----------
data : pd.Dataframe
    Dataframe which contains the pixel label/predictions
num_classes : int, optional
    Number of classes to represent
mapping : dict, optional
    Mapping between the stored class and a redefined set of classes

---
### FunctionDef: `build_reco`

Builds :class:`RecoFragment` objects from the full chain output.

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
List[RecoFragment]
    List of constructed reconstructed fragment instances

---
### FunctionDef: `build_reco`

Builds :class:`RecoInteraction` objects from the full chain output.

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
List[RecoInteraction]
    List of constructed reconstructed interaction instances

---
### FunctionDef: `build_reco`

Builds :class:`RecoParticle` objects from the full chain output.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `build_reco`

Place-holder for a method used to build reconstructed objects.

Parameters
----------
data : dict
    Dictionary which contains the necessary data products

---
### FunctionDef: `build_sources`

Construct the reference coordinate and value tensors used by
all the representations built by the module.

These objects should be stored along with the constructed objects
if the objects are to be loaded later on.

Parameters
----------
data : dict
    Dictionary of input data and model outputs
entry : int, optional
    Entry number

---
### FunctionDef: `build_truth`

Builds :class:`TruthFragment` objects from the full chain output.

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
List[TruthFragment]
    List of constructed true fragment instances

---
### FunctionDef: `build_truth`

Builds :class:`TruthInteraction` objects from the full chain output.

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
List[TruthInteraction]
    List of constructed truth interaction instances

---
### FunctionDef: `build_truth`

Builds :class:`TruthParticle` objects from the full chain output.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `build_truth`

Place-holder for a method used to build truth objects.

Parameters
----------
data : dict
    Dictionary which contains the necessary data products

---
### ClassDef: `BuilderBase`

Abstract base class for building all data structures

A Builder class takes input data and full chain result dictionaries
and processes them into human-readable data structures.

---
### ClassDef: `BuildManager`

Manager which constructs data representations based on the chain output.

Takes care of two scenarios:
  - Interpret the raw output of the reconstruction chain
  - Load up existing objects stored as dictionaries

---
### FunctionDef: `calc_gradient_penalty`

Code From the DUQ main Github Repository:
https://github.com/y0ast/deterministic-uncertainty-quantification

Author: Joost van Amersfoort

---
### FunctionDef: `calc_gradient_penalty`

Code From the DUQ main Github Repository:
https://github.com/y0ast/deterministic-uncertainty-quantification

Author: Joost van Amersfoort

---
### ClassDef: `CalibrationDatabase`

Wraps basic SQLite loading/querying functions to provide a more
user-friendly API to the calibration classes.

Notes
-----
This class assumes that the structure of the SQLite libraries used
is that of ICARUS calibration databases, for now.

---
### ClassDef: `CalibrationLUT`

Look-up table for calibration values. Given a set of coordinates,
returns a calibration value.

---
### ClassDef: `CalibrationManager`

Manager in charge of applying all calibration-related corrections onto
a set of 3D space points and their associated measured charge depositions.

---
### ClassDef: `CalibrationProcessor`

Apply calibrations to the reconstructed objects.

---
### FunctionDef: `calibrator_factory`

Instantiates a calibrator from a configuration dictionary.

Parameters
----------
cfg : dict
    Calibrator configuration

Returns
-------
object
    Instantiated calibrator

---
### FunctionDef: `calibrator_factory`

Instantiates a calibrator module from a configuration dictionary.

Parameters
----------
name : str
    Name of the calibration module
cfg : dict
    Calibration module configuration

Returns
-------
object
     Initialized calibration module

---
### FunctionDef: `calibrator_loss_factory`

Instantiates a calibrator loss from a configuration dictionary.

Parameters
----------
cfg : dict
    Calibrator loss configuration

Returns
-------
object
    Instantiated calibrator loss

---
### ClassDef: `CalorimetricEnergyProcessor`

Compute calorimetric energy by summing the charge depositions and
scaling by the ADC to MeV conversion factor, if needed.

---
### ClassDef: `CascadeDilationBlock`

Cascaded Atrous Convolution Block.

---
### FunctionDef: `cast_to_numpy`

Casts the model output data products to numpy object in place.

Parameters
----------
result : dict
    Dictionary of model and loss outputs

---
### FunctionDef: `cathode_pos`

Location of the cathode plane along the drift axis.

Returns
-------
float
    Location of the cathode plane along the drift axis

---
### FunctionDef: `cathode_pos`

Position of the cathode along the drift direction.

Returns
-------
float
    Cathode position along the drift direction

---
### FunctionDef: `cathode_side`

Returns whether the cathode is on the lower or upper boundary of
the TPC along the drift axis (0 for lower, 1 for upper).

Returns
-------
int
    Cathode side of the TPC

---
### ClassDef: `CathodeCrosserProcessor`

Find particles that cross the cathode of a LArTPC module that is divided
into two TPCs. It might manifest itself into two forms:
- If the particle is ~in-time, it will be a single particle, with
  potentially a small break/offset in the center
- If the particle is sigificantly out-of-time, a cathode crosser will
  be composed of two distinct reconstructed particle objects

---
### FunctionDef: `cdist`

Numba implementation of Euclidean
`scipy.spatial.distance.cdist(x, p=2)` in 1D, 2D or 3D.

Parameters
----------
x1 : np.ndarray
    (N,d) array of point coordinates in the first set
x2 : np.ndarray
    (M,d) array of point coordinates in the second set

Returns
-------
np.ndarray
    (N,M) array of pair-wise Euclidean distances

---
### FunctionDef: `center`

Center of the box.

Returns
-------
np.ndarray
    Center of the box

---
### ClassDef: `Chamber`

Class which holds all properties of an individual time-projection
chamber (TPC).

Attributes
----------
drift_dir : np.ndarray
    (3) TPC drift direction vector (normalized)
drift_axis : int
    Axis along which the electrons drift (0, 1 or 2)

---
### FunctionDef: `check_containment`

Check whether a point cloud comes within some distance of the
boundaries of a certain subset of detector volumes, depending on the
mode.

Parameters
----------
points : np.ndarray
    (N, 3) Set of point coordinates
sources : np.ndarray, optional
    (S, 2) : List of [module ID, tpc ID] pairs that created the
    point cloud
allow_multi_module : bool, default `False`
    Whether to allow particles/interactions to span multiple modules
summarize : bool, default `True`
    If `True`, only returns a single flag for the whole cloud.
    Otherwise, returns a boolean array corresponding to each point.

Returns
-------
Union[bool, np.ndarray]
    `True` if the particle is contained, `False` if not

---
### FunctionDef: `check_merge`

Check if a track and a shower can be merged.

Parameters
----------
p_track : RecoParticle
    Track particle that will be merged into the shower.
p_shower : RecoParticle
    Shower particle to merge the track into.
angle_threshold : float, default 0.95
    Check if track and shower cosine distance is greater than this value.
adjacency_threshold : float, default 0.5
    Check if track and shower is within threshold distance.
dedx_limit : int, default -1
    Check if the track dedx is below this value,
    to avoid merging protons.
track_length_limit : int, default 40
    Check if track length is below this value,
    to avoid merging long tracks.

Returns
-------
result : bool
    True if the track and shower can be merged, False otherwise.

---
### FunctionDef: `check_track_orientation`

Given a set of track point coordinates and the track end points, checks
which end point is most likely to be the correct start, based on the
rate of energy deposition in the track.

Parameters
----------
coordinates : np.ndarray
    (N, 3) Coordinates of the points that make up the track
values : np.ndarray
    (N) Values associated with each point
start_point : np.ndarray
    (3) Start point of the track
end_point : np.ndarray
    (3) End point of the track
method : str, default 'local'
    Method used to orient the track (one of 'local', 'gradient')
local_radius : float, default 5
    Radius around the end points to used to evaluate the local dE/dx
anchor_points : bool, default True
    Weather or not to collapse end point onto the closest track point
segment_method : str, default 'step_next'
    Method used to segment the track when using the 'gradient' method
segment_length : float, default 5
    Segment length when using the 'gradient' method
segment_min_count : int, default 10
    Minimum number of points in a segment when using the 'gradient' method

Returns
-------
bool
   Returns `True` if the start point provided is correct, `False`
   if the end point is more likely to be the start point.

---
### FunctionDef: `check_track_orientation_ppn`

Use PPN end point predictions to predict track orientation.

Use the PPN point assignments as a basis to orient a track. Match
the end points of a track to the closest PPN candidate and pick the
candidate with the highest start score as the start point

Parameters
----------
start_point : np.ndarray
    (3) Start point of the track
end_point : np.ndarray
    (3) End point of the track
ppn_candidates : np.ndarray
    (N, 10)  PPN point candidates and their associated scores

Returns
-------
bool
   Returns `True` if the start point provided is correct, `False`
   if the end point is more likely to be the start point.

---
### FunctionDef: `check_units`

Check that the point coordinates of an object are as expected.

Parameters
----------
obj : Union[FragmentBase, ParticleBase, InteractionBase]
    Particle or interaction object

Results
-------
np.ndarray
    (N, 3) Point coordinates

---
### FunctionDef: `check_units`

Checks that the objects in the list are expressed in the
appropriate units. Convert them otherwise.

Parameters
----------
data : dict
    Dictionary of data products
key : str
    Dictionary key corresponding to the objects to convert
entry : int, optional
    Entry to process

---
### FunctionDef: `chi2`

Computes a chi2 score given a set of observed/expected dE/dx values.

Parameters
----------
dedxs : np.ndarray
    (S) Measured values of dedxs at a set of known residual ranges
rrs : np.ndarray
    (S) Residual range values (one per track segment)
pid : int
    Particle species enumerator

Returns
-------
float
    Chi2 agreement value

---
### ClassDef: `ChildrenProcessor`

Count the number of children of a given particle, using the particle
hierarchy information from :class:`ParticleGraphParser`.

---
### FunctionDef: `class_mask`

Filter classes according to segmentation label.

---
### FunctionDef: `clean_config`

Remove model loading/freezing keys from all level of a dictionary.

This is used to remove the weight loading/freezing from the input
configuration before it is fed to the model/loss classes.

Parameters
----------
config : dict
    Dictionary to remove the keys from

---
### FunctionDef: `clean_sparse_data`

Helper that factorizes common cleaning operations required when trying
to match cluster3d data products to sparse3d data products.

This function does the following:
1. Lexicographically sort group data (images are lexicographically sorted)
2. Remove voxels from group data that are not in image
3. Choose only one group per voxel (by lexicographic order)

The set of sparse voxels must be a subset of the set of cluster voxels and
it must not contain any duplicates.

Parameters
----------
cluster_voxels : np.ndarray
    (N, 3) Matrix of voxel coordinates in the cluster3d tensor
cluster_data : np.ndarray
    (N, F) Matrix of voxel values corresponding to each voxel
    in the cluster3d tensor
sparse_voxels : np.ndarray
    (M, 3) Matrix of voxel coordinates in the reference sparse tensor
precedence: list, default SHAPE_PREC
    (C) Array of classes in the reference array, ordered by precedence

Returns
-------
cluster_voxels: np.ndarray
    (M, 3) Ordered and filtered set of voxel coordinates
cluster_data: np.ndarray
    (M, F) Ordered and filtered set of voxel values

---
### FunctionDef: `closest_pair`

Algorithm which finds the two points which are closest to each other
from two separate sets.

Two algorithms:
- `brute`: compute cdist, use argmin
- `recursive`: Start with one point in one set, find the closest
               point in the other set, move to theat point, repeat. This
               algorithm is *not* exact, but a good and very quick proxy.

Parameters
----------
x1 : np.ndarray
    (Nx3) array of point coordinates in the first set
x1 : np.ndarray
    (Nx3) array of point coordinates in the second set
algorithm : str
    Name of the algorithm to use: `brute` or `recursive`
seed : bool
    Whether or not to use the two farthest points in one set to seed the recursion

Returns
-------
int
    ID of the first point that makes up the pair
int
    ID of the second point that makes up the pair
float
    Distance between the two points

---
### ClassDef: `ClustCNNEdgeEncoder`

Produces cluster edge features using a sparse residual CNN encoder.

Considers an edge as an image containing both ojbects connected by
the edge in a single image.

---
### ClassDef: `ClustCNNGlobalEncoder`

Produces graph-wide features using a sparse residual CNN encoder.

Considers the whole graph as an image containing all objects in it.

---
### ClassDef: `ClustCNNNodeEncoder`

Produces cluster node features using a sparse residual CNN encoder.

---
### ClassDef: `Cluster2DParser`

Class that retrieves and parses a 2D cluster list.

.. code-block. yaml

    schema:
      cluster_label:
        parser: cluster2d
        cluster_event: cluster2d_pcluster

---
### FunctionDef: `cluster3d_to_sparse3d`

Merge all clusters in a cluster3d object into a single sparse object.

Parameters
----------
larcv.EventClusterVoxel3D
    Cluster of 3D sparse tensor
segmentation : bool, default True
    If `True`, create dummy segmentation labels for the output tensor
ghost : bool, default True
    If `True`, include ghost labels in the dummy segmentation labels

Returns
-------
larcv.EventSparseTensor3D
    Event containing one 3D larcv sparse tensor

---
### ClassDef: `Cluster3DAggregateParser`

Identical to :class:`Cluster3DParser`, but aggregates charge information
from multiple value sources.

---
### ClassDef: `Cluster3DChargeRescaledParser`

Identical to :class:`Cluster3DParser`, but computes rescaled charges
on the fly.

---
### ClassDef: `Cluster3DParser`

Class that retrieves and parses a 3D cluster list.

.. code-block. yaml

    schema:
      cluster_label:
        parser: cluster3d
        cluster_event: cluster3d_pcluster
        particle_event: particle_pcluster
        particle_mpv_event: particle_mpv
        neutrino_event: neutrino_mpv
        sparse_semantics_event: sparse3d_semantics
        sparse_value_event: sparse3d_pcluster
        add_particle_info: true
        clean_data: true
        type_include_mpr: false
        type_include_secondary: false
        primary_include_mpr: true
        break_clusters: false

---
### FunctionDef: `cluster_dedx`

Computes the initial local dE/dx of a cluster.

Parameters
----------
voxels : np.ndarray
    (N, 3) Voxel coordinates
values : np.ndarray
    (N) Voxel values
starts : np.ndarray
    (3) Start point w.r.t. which to compute the local dE/dx
max_dist : float, default 5.0
    Neighborhood radius around the point used to compute the dE/dx

Returns
-------
float
    Local dE/dx value around the start point

---
### FunctionDef: `cluster_direction`

Estimates the orientation of a cluster.

It follows the following procedure:
- By default, it takes the normalized mean direction from the cluster
  start point to the cluster voxels
- If `max_dist` is specified, it restricts the cluster voxels
  to those within a `max_dist` radius from the start point
- If `optimize` is True, it selects the neighborhood which
  minimizes the transverse spread w.r.t. the direction

Parameters
----------
voxels : np.ndarray
    (N, 3) Voxel coordinates
starts : np.ndarray
    (C, 3) Start points w.r.t. which to estimate the direction
clusts : List[np.ndarray]
    (C) List of cluster indexes
max_dist : float, default -1
    Neighborhood radius around the point used to estimate the direction
optimize : bool, default False
    If `True`, the neighborhood radius is optimized on the fly for
    each cluster.

Returns
-------
np.ndarray
    (3) Direction vector

---
### FunctionDef: `cluster_end_points`

Estimates the end points of a clusters using PCA and curvature.

It proceeds in the following fashion:
1. Find the principal axis a of the point cloud
2. Find the coordinate a_i of each point along this axis
3. Find the points with minimum and maximum coordinate
4. Find the point that has the largest umbrella curvature

Parameters
----------
voxels : np.ndarray
    (N, 3) Voxel coordinates

Returns
-------
int
    Index of the start voxel
int
    Index of the end voxel

---
### FunctionDef: `cluster_to_voxel_label`

Turns a list of labels on clusters to an array of labels on voxels.

Parameters
----------
clusts : List[np.ndarray]
    (C) List of cluster indexes
node_labels : np.ndarray
    (C) Node labels

Returns
-------
np.ndarray
    (N) Voxel labels

---
### FunctionDef: `cluster_track_chunks`

Find point where the track is broken, divide out the track
into self-contained chunks which are Linf connect (Moore neighbors).

Parameters
----------
points : np.ndarray
    (N, 3) List of track cluster point coordinates
start_point : np.ndarray
    (3) Start point of the track cluster
end_point : np.ndarray
    (3) End point of the track cluster
pixel_size : float
    Dimension of one pixel, used to identify what is big enough to
    constitute a break

Returns
-------
np.ndarray
    (N) Track chunk labels

---
### ClassDef: `ClusterAna`

Class which computes and stores the necessary data to evaluate
clustering metrics at different aggregation stages:
- fragments
- particles
- interactions

---
### ClassDef: `ClusterGraphConstructor`

Manager class for handling per-batch, per-semantic type graph
construction and node predictions in Graph-SPICE clustering.

---
### FunctionDef: `clustering_metrics`

Computes several clustering metrics for a set of clusters.

Parameters
----------
clusts : List[np.ndarray]
    (C) List of cluster indexes
node_assn : np.ndarray
    (C) True node groups labels
node_pred : np.ndarray
    (C) Predicted node group labels

Returns
-------
float
    Adjusted Rand Index (ARI)
float
    Adjusted Mutual information (AMI)
float
    Symetric Best Dice (SBD)
float
    Purity
float
    Efficiency

---
### ClassDef: `ClusterLabelEnum`

Enumerates all possible columns of the cluster label tensor.

---
### ClassDef: `ClustGeoCNNMixEdgeEncoder`

Produces cluster edge features using both geometric and CNN encoders.

---
### ClassDef: `ClustGeoCNNMixNodeEncoder`

Produces cluster node features using both geometric and CNN encoders.

---
### ClassDef: `ClustGeoEdgeEncoder`

Produces cluster edge features using hand-engineered quantities.

The basic 19 geometric features are composed of:
- Position of the voxel in the first cluster closest to the second (3)
- Position of the voxel in the second cluster closest to the first (3)
- Displacement vector from the first to the second point defined above (3)
- Length of the displacement vector (1)
- Outer product of the displacement vector (9)

---
### ClassDef: `ClustGeoNodeEncoder`

Produces cluster node features using hand-engineered quantities.

The basic 16 geometric features are composed of:
- Center (3)
- Covariance matrix (9)
- Principal axis (3)
- Voxel count (1)

The flag `add_value` adds the following 2 features:
- Mean energy (1)
- RMS energy (1)

The flag `add_shape` adds the particle shape information:
- Semantic type (1), i.e. most represented type in cluster

The flag `add_points` adds the particle end points information
- Start point (3)
- End point (3)

The flag `add_directions` adds the particle direction information
- Start direction (3)
- End direction (3)

The flag `add_local_dedxs` adds the local dEdx estimate at each endpoint
- Start dEdx (1)
- End dEdx (1)

---
### FunctionDef: `collate_factory`

Instantiates collate function based on type specified in configuration
under `io.collate.name`. The name must match the name of a class
under `spine.io.collates`.

Parameters
----------
collate_cfg : dict
    Collate function configuration dictionary

Returns
-------
function
    Initialized collate function

---
### ClassDef: `CollateAll`

General collate function for all data types coming from the parsers.

Provide it with a list of dictionaries, each of which maps keys to one of:
1. Tuple of (voxel tensor, feature tensor, metadata) which get merged
   into a single tensor with rows [batch_id, *coords, *features]
2. Simple feature tensor which gets merged into a single tensor with
   rows [batch_id, *features]
3. Scalars/list/objects which simply get put in a single list

---
### FunctionDef: `color_rgba`

Convert an RGB color array into an RGBA string.

Parameters
----------
color : List[int]
    (3) List of RGB values
alpha : float
    Alpha value in [0, 1]

Returns
-------
str
    RGBA string

---
### FunctionDef: `combine`

Wrapper function for combining different components of the loss function.
Inputs:
    features (torch.Tensor): pixel embeddings
    labels (torch.Tensor): ground-truth instance labels
Returns:
    loss: combined loss, in most cases over a given semantic class.

---
### FunctionDef: `combine_multiclass`

Wrapper function for combining different components of the loss,
in particular when clustering must be done PER SEMANTIC CLASS.

NOTE: When there are multiple semantic classes, we compute the DLoss
by first masking out by each semantic segmentation (ground-truth/prediction)
and then compute the clustering loss over each masked point cloud.

INPUTS:
    features (torch.Tensor): pixel embeddings
    slabels (torch.Tensor): semantic labels
    clabels (torch.Tensor): group/instance/cluster labels

OUTPUT:
    loss_segs (list): list of computed loss values for each semantic class.
    loss[i] = computed DLoss for semantic class <i>.
    acc_segs (list): list of computed clustering accuracy for each semantic class.

---
### FunctionDef: `combine_multiclass`

Wrapper function for combining different components of the loss,
in particular when clustering must be done PER SEMANTIC CLASS.

NOTE: When there are multiple semantic classes, we compute the DLoss
by first masking out by each semantic segmentation (ground-truth/prediction)
and then compute the clustering loss over each masked point cloud.

INPUTS:
    features (torch.Tensor): pixel embeddings
    slabels (torch.Tensor): semantic labels
    clabels (torch.Tensor): group/instance/cluster labels

OUTPUT:
    loss_segs (list): list of computed loss values for each semantic class.
    loss[i] = computed DLoss for semantic class <i>.
    acc_segs (list): list of computed clustering accuracy for each semantic class.

---
### FunctionDef: `combine_multiclass`

Wrapper function for combining different components of the loss,
in particular when clustering must be done PER SEMANTIC CLASS.

NOTE: When there are multiple semantic classes, we compute the DLoss
by first masking out by each semantic segmentation (ground-truth/prediction)
and then compute the clustering loss over each masked point cloud.

INPUTS:
    features (torch.Tensor): pixel embeddings
    slabels (torch.Tensor): semantic labels
    clabels (torch.Tensor): group/instance/cluster labels

OUTPUT:
    loss_segs (list): list of computed loss values for each semantic class.
    loss[i] = computed DLoss for semantic class <i>.
    acc_segs (list): list of computed clustering accuracy for each semantic class.

---
### FunctionDef: `combine_multiclass`

Wrapper function for combining different components of the loss,
in particular when clustering must be done PER SEMANTIC CLASS.

NOTE: When there are multiple semantic classes, we compute the DLoss
by first masking out by each semantic segmentation (ground-truth/prediction)
and then compute the clustering loss over each masked point cloud.

INPUTS:
    features (torch.Tensor): pixel embeddings
    slabels (torch.Tensor): semantic labels
    clabels (torch.Tensor): group/instance/cluster labels

OUTPUT:
    loss_segs (list): list of computed loss values for each semantic class.
    loss[i] = computed DLoss for semantic class <i>.
    acc_segs (list): list of computed clustering accuracy for each semantic class.

---
### FunctionDef: `combine_multiclass`

Wrapper function for combining different components of the loss,
in particular when clustering must be done PER SEMANTIC CLASS.

NOTE: When there are multiple semantic classes, we compute the DLoss
by first masking out by each semantic segmentation (ground-truth/prediction)
and then compute the clustering loss over each masked point cloud.

INPUTS:
    features (torch.Tensor): pixel embeddings
    slabels (torch.Tensor): semantic labels
    clabels (torch.Tensor): group/instance/cluster labels

OUTPUT:
    loss_segs (list): list of computed loss values for each semantic class.
    loss[i] = computed DLoss for semantic class <i>.
    acc_segs (list): list of computed clustering accuracy for each semantic class.

---
### FunctionDef: `combine_multiclass`

Wrapper function for combining different components of the loss,
in particular when clustering must be done PER SEMANTIC CLASS.

NOTE: When there are multiple semantic classes, we compute the DLoss
by first masking out by each semantic segmentation (ground-truth/prediction)
and then compute the clustering loss over each masked point cloud.

INPUTS:
    features (torch.Tensor): pixel embeddings
    slabels (torch.Tensor): semantic labels
    clabels (torch.Tensor): group/instance/cluster labels

OUTPUT:
    loss_segs (list): list of computed loss values for each semantic class.
    loss[i] = computed DLoss for semantic class <i>.
    acc_segs (list): list of computed clustering accuracy for each semantic class.

---
### FunctionDef: `combine_multiclass`

Wrapper function for combining different components of the loss,
in particular when clustering must be done PER SEMANTIC CLASS.

NOTE: When there are multiple semantic classes, we compute the DLoss
by first masking out by each semantic segmentation (ground-truth/prediction)
and then compute the clustering loss over each masked point cloud.

INPUTS:
    features (torch.Tensor): pixel embeddings
    slabels (torch.Tensor): semantic labels
    clabels (torch.Tensor): group/instance/cluster labels
OUTPUT:
    loss_segs (list): list of computed loss values for each semantic class.
    loss[i] = computed DLoss for semantic class <i>.
    acc_segs (list): list of computed clustering accuracy for each semantic class.

---
### FunctionDef: `combine_multiclass`

Wrapper function for combining different components of the loss,
in particular when clustering must be done PER SEMANTIC CLASS.

NOTE: When there are multiple semantic classes, we compute the DLoss
by first masking out by each semantic segmentation (ground-truth/prediction)
and then compute the clustering loss over each masked point cloud.

INPUTS:
    features (torch.Tensor): pixel embeddings
    slabels (torch.Tensor): semantic labels
    clabels (torch.Tensor): group/instance/cluster labels
OUTPUT:
    loss_segs (list): list of computed loss values for each semantic class.
    loss[i] = computed DLoss for semantic class <i>.
    acc_segs (list): list of computed clustering accuracy for each semantic class.

---
### FunctionDef: `combine_multiclass`

Wrapper function for combining different components of the loss,
in particular when clustering must be done PER SEMANTIC CLASS.

NOTE: When there are multiple semantic classes, we compute the DLoss
by first masking out by each semantic segmentation (ground-truth/prediction)
and then compute the clustering loss over each masked point cloud.

INPUTS:
    features (torch.Tensor): pixel embeddings
    slabels (torch.Tensor): semantic labels
    clabels (torch.Tensor): group/instance/cluster labels
OUTPUT:
    loss_segs (list): list of computed loss values for each semantic class.
    loss[i] = computed DLoss for semantic class <i>.
    acc_segs (list): list of computed clustering accuracy for each semantic class.

---
### FunctionDef: `complete_graph`

Creates a list of edges corresponding to a directed complete graph
in a batch of nodes (nodes from separate entries).

Parameters
----------
counts : np.ndarray, optional
    (B) Number of nodes in each entry of the batch

---
### ClassDef: `CompleteGraph`

Generates graphs that connect each node with every other node.

If two nodes belong to separate batches, they cannot be connected.

See :class:`GraphBase` for attributes/methods shared
across all graph constructors.

---
### FunctionDef: `compute_accuracy`

Compute accuracy score for a single datapoint (one trained model)

---
### FunctionDef: `compute_angular_criterion`

Compute the angular criterion for the given primary electron shower.

Parameters
----------
p : RecoParticle
    Primary electron shower to check for multi-arm.
vertex : np.ndarray
    Vertex of the interaction with shape (3, )
eps : float
    Maximum distance between two samples for one to be considered
    as in the neighborhood of the other (DBSCAN).
min_samples : int
    The number of samples (or total weight) in a neighborhood 
    for a point to be considered as a core point (DBSCAN).

Returns
-------
max_angle : float
    Maximum angle between the mean cluster direction vectors 
    of the shower points (degrees)

---
### FunctionDef: `compute_edge_weight`

Converts the output of the embedder into an edge score.

Parameters
----------
sp_emb1 : torch.Tensor
    (E, 3) Spatial embeddings of the source nodes
sp_emb2 : torch.Tensor
    (E, 3) Spatial embeddings of the target nodes
ft_emb1 : torch.Tensor
    (E, N_f) Feature embeddings of the source nodes
ft_emb2 : torch.Tensor
    (E, N_f) Feature embeddings of the target nodes
cov1 : torch.Tensor
    (E, 2) Spatial extent of the cluster the source nodes belongs to
cov2 : torch.Tensor
    (E, 2) Spatial extent of the cluster the target nodes belongs to
occ1 : torch.Tensor
    (E, 1) Multiplicity of the cluster the source nodes belongs to
occ2 : torch.Tensor
    (E, 1) Multiplicity of the cluster the target nodes belongs to

Returns
-------
torch.Tensor
    Scalar value of the edge weight

---
### FunctionDef: `compute_edge_weight_coord`

Converts the the spatial coordinates information into an edge score.

Parameters
----------
coord1 : torch.Tensor
    (E, 3) Coordinates of the source nodes
coord2 : torch.Tensor
    (E, 3) Coordinates of the target nodes
tan1 : torch.Tensor
    (E, N_f) Tangents of the source nodes
tan2 : torch.Tensor
    (E, N_f) Tangents of the target nodes
coord_cov1 : torch.Tensor
    (E, 3) Spatial extent of the cluster the source nodes belongs to
coord_cov2 : torch.Tensor
    (E, 3) Spatial extent of the cluster the target nodes belongs to
tan_cov1 : torch.Tensor
    (E, 1) Multiplicity of the cluster the source nodes belongs to
tan_cov2 : torch.Tensor
    (E, 1) Multiplicity of the cluster the target nodes belongs to

Returns
-------
torch.Tensor
    Scalar value of the edge weight

---
### FunctionDef: `compute_heuristic_accuracy`

Compute Adjusted Rand Index Score for given embedding coordinates,
where predicted cluster labels are obtained from distance to closest
centroid (computes heuristic accuracy).

Inputs:
    embedding (torch.Tensor): (N, d) Tensor where 'd' is the embedding dimension.
    truth (torch.Tensor): (N, ) Tensor for the ground truth clustering labels.
Returns:
    score (float): Computed ARI Score
    clustering (array): the predicted cluster labels.

---
### FunctionDef: `compute_rescaled_charge`

Computes rescaled charge after deghosting.

The last 6 columns of the input tensor *MUST* contain:
- charge in each of the projective planes (3)
- index of the hit in each 2D projection (3)

Notes
-----
This function should work on numpy arrays or Torch tensors.

Parameters
----------
data : Union[np.ndarray, torch.Tensor]
    (N, 1 + D + N_f + 6) tensor of voxel/value pairs
collection_only : bool, default False
    Only use the collection plane to estimate the rescaled charge
collection_id : int, default 2
    Index of the collection plane

Returns
-------
data : Union[np.ndarray, torch.Tensor]
    (N) Rescaled charge values

---
### FunctionDef: `compute_rescaled_charge_batch`

Batched version of :func:`compute_rescaled_charge`.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f + 6) tensor of voxel/value pairs
collection_only : bool, default False
    Only use the collection plane to estimate the rescaled charge
collection_id : int, default 2
    Index of the collection plane

Returns
-------
Union[np.ndarray, torch.Tensor]
    (N) Rescaled charge values

---
### FunctionDef: `cone_trace`

Converts a cloud of points into a 3D cone.

This function uses the PCA and the average angle w.r.t. to the point
of maximum curvature as a basis to construct a cone.

Parameters
----------
points : np.ndarray
    (N, 3) Array of point coordinates
fraction : float, default 0.5
    Fraction of the points contained in the cone (angle quantile)
num_samples : int, default 10
    Number of points sampled along h and phi in the conical coordinate
    system of the cone. A larger number increases the resolution.
showscale : bool, default False
    If True, show the colorscale of the :class:`plotly.graph_objs.Mesh3d`
color : Union[str, float], optional
    Color of the cone
hovertext : Union[int, str, np.ndarray], optional
    Text associated with the cone
**kwargs : dict, optional
    Additional parameters to pass to the 

---
### FunctionDef: `config_full`

Fixture to generate a basic configuration dictionary given a model name.

---
### FunctionDef: `config_simple`

Fixture to generate a basic configuration dictionary given a model name.
    

---
### ClassDef: `ConfigLoader`

Configuration loader class.

This class implements a more complex YAML loader than the standard loader in
order to support more advanced functions such as:
- Include YAML configuration files into another YAML configuration file;
- Edit an included YAML dictionary with one liners (to modify single
  configuration parameters without replicating a configuration block).

---
### ClassDef: `ConnectedComponentClusterer`

Finds connected components based on graph edge assignments.

---
### FunctionDef: `construct`

Prepares the input based on the required data and runs constructor.

Parameters
----------
func : str
    Build function name
data : dict
    Dictionary of data products
entry : int, optional
    Entry to process

Returns
-------
List[object]
    List of constructed objects

---
### ClassDef: `ContainmentProcessor`

Check whether a fragment, particle or interaction is contained.

This module checks whether the object comes within some distance of the
boundaries of the detector and assign the `is_contained` attribute
accordingly.

---
### FunctionDef: `contingency_table`

Build a contingency table for two sets of labels.

Parameters
----------
x : np.ndarray
    (N) Array of integrer values
y : np.ndarray
    (M) Array of integrer values
nx : int, optional
    Number of integer values allowed in `x`, N
ny : int, optional
    Number of integer values allowd in `y`, M

Returns
-------
np.ndarray
    (N, M) Contingency table

---
### FunctionDef: `convdist_protons`

Helper function to compute the distance between the shower
startpoint and the closest proton point.

Parameters
----------
ia : RecoInteraction
    Reco interaction to apply the conversion distance cut.
shower_p : RecoParticle
    Member particle of the interaction, assumed to be the primary
    electron/gamma shower.

Returns
-------
start_to_closest_proton : float
    Closest distance between the shower startpoint 
    and proton/pion points.

---
### FunctionDef: `convdist_vertex_points`

Helper function to compute the closest distance 
between the vertex and all shower points. 

Parameters
----------
ia : RecoInteraction
    Reco interaction to apply the conversion distance cut.
shower_p : RecoParticle
    Member particle of the interaction, assumed to be the primary
    electron/gamma shower.

Returns
-------
start_to_closest_proton : float
    Closest distance between the shower startpoint and proton points.

---
### FunctionDef: `convdist_vertex_startpoint`

Helper function to compute the closest distance 
between the vertex and predicted shower startpoint. 

Parameters
----------
ia : RecoInteraction
    Reco interaction to apply the conversion distance cut.
shower_p : RecoParticle
    Member particle of the interaction, assumed to be the primary
    electron/gamma shower.

Returns
-------
start_to_closest_proton : float
    Closest distance between the shower startpoint and proton points.

---
### ClassDef: `ConversionDistanceProcessor`

Enforce additional constraint on valid primary electron showers
using vertex-to-shower separation distance. 

NOTE: This processor can only change reco electron shower pid to
photon pid depending on the distance threshold. 

---
### ClassDef: `ConvolutionBlock`

Convolution block which operates a sequence of
two (convolution + nomalization + activation) steps.

---
### FunctionDef: `copy`

Returns an independant copy of the object.

Returns
-------
Time
    Copy of the object

---
### FunctionDef: `correct_shower_startpoint`

Function to correct the shower startpoint by finding the closest
point to the vertex.

Parameters
----------
shower_p : RecoParticle
    Primary EM shower to correct the startpoint.
ia : RecoInteraction
    Reco interaction to use as the vertex estimate.

Returns
-------
guess : np.ndarray
    (3, ) array of the corrected shower startpoint.

---
### FunctionDef: `create`

Create the output file structure based on the data dictionary.

Parameters
----------
data : dict
    Dictionary of data products
cfg : dict
    Dictionary containing the complete SPINE configuration

---
### FunctionDef: `create`

Initialize the header of the CSV file, record the keys to be stored.

Parameters
----------
result_blob : dict
    Dictionary containing the output of the reconstruction chain

---
### FunctionDef: `crt_traces`

Function which produces a list of traces which represent the optical
detectors in a 3D event display.

Parameters
----------
meta : Meta, optional
    Metadata information (only needed if pixel_coordinates is True)
detector_coords : bool, default False
    If False, the coordinates are converted to pixel indices
shared_legend : bool, default True
    If True, the legend entry in plotly is shared between all the
    detector volumes
name : Union[str, List[str]], default 'Detector'
    Name(s) of the detector volumes
color : Union[int, str, np.ndarray]
    Color of CRT detectors or list of color of CRT detectors
**kwargs : dict, optional
    List of additional arguments to pass to
    spine.vis.ellipsoid.ellipsoid_traces or spine.vis.box.box_traces

Returns
-------
List[plotly.graph_objs.Mesh3D]
    List of CRT detector traces (one per CRT element)

---
### ClassDef: `CRTDetector`

Handles all geometry queries for a set of cosmic-ray taggers.

Attributes
----------
positions : np.ndarray
    (N_c, 3) Location of the center of each of the CRT planes
    - N_c is the number of CRT planes
dimensions : np.ndarray
    (N_c, 3) Dimensions of each of the CRT planes
    - N_c is the number of CRT planes
norms : np.ndarray
    (N_c) Axis aligned with the norm of each of the CRT planes
    - N_c is the number of CRT planes
det_ids : Dict[int, int], optional
    Mapping between the CRT channel and its corresponding detector

---
### ClassDef: `CRTHit`

CRT hit information.

Attributes
----------
id : int
    Index of the CRT hit in the list
plane : int
    Index of the CRT tagger that registered the hit
tagger : str
    Name of the CRT tagger that registered the hit
feb_id : np.ndarray
    Address of the FEB board stored as a list of bytes (uint8)
ts0_s : int
    Absolute time from White Rabbit (seconds component)
ts0_ns : float
    Absolute time from White Rabbit (nanoseconds component)
ts0_s_corr : float
    Unclear in the documentation, placeholder at this point
ts0_ns_corr : float
    Unclear in the documentation, placeholder at this point
ts1_ns : float
    Time relative to the trigger (nanoseconds component)
total_pe : float
    Total number of PE in the CRT hit
pe_per_ch : np.ndarray
    Number of PEs per FEB channel
center : np.ndarray
    Barycenter of the CRT hit in detector coordinates
width : np.ndarray
    Uncertainty on the barycenter of the CRT hit in detector coordinates
units : str
    Units in which the position attributes are expressed

---
### ClassDef: `CRTHitParser`

Copy construct CRTHit and return an array of `CRTHit`.

.. code-block. yaml
    schema:
      crthits:
        parser: crthit
        crthit_event: crthit_crthit

---
### ClassDef: `CRTMatcher`

Adapter class between full chain outputs and matcha (Python package
for matching tracks to CRT hits)

---
### ClassDef: `CRTMatchProcessor`

Associates TPC particles with CRT hits.
    

---
### ClassDef: `CRTTPCManager`

Class that manages TPC track and CRT hit objects. Similar to the FlashManager
class, but does not inherit from it. Interfaces with matcha to perform CRT-TPC 
matching; see https://github.com/andrewmogan/matcha

Attributes
==========

Methods
=======

---
### FunctionDef: `csda_ke_lar`

Numerically optimizes the kinetic energy necessary to observe the
range of a particle that has been measured, under the CSDA.

Parameters
----------
R : float
    Range that the particle travelled through liquid argon in cm
M : float
    Particle mass in MeV/c^2
z : int, default 1
    Impinging partile charge in multiples of electron charge
T_max : float, default 1e6
    Maximum allowed kinetic energy
epsrel : float, default 1e-3
    Relative error tolerance
epsabs : float, default 1e-3
    Asbolute error tolerance

Returns
-------
float
    CSDA kinetic energy in MeV

---
### FunctionDef: `csda_range_lar`

Numerically integrates the inverse Bethe-Bloch formula to find the
CSDA range of a particle for a given initial kinetic energy.

Parameters
----------
T0 : float
    Initial kinetic energy in MeV
M : float
    Particle mass in MeV/c^2
z : int, default 1
    Impinging partile charge in multiples of electron charge
epsrel : float, default 1e-3
    Relative error tolerance
epsabs : float, default 1e-3
    Asbolute error tolerance

Returns
-------
float
    CSDA range in cm

---
### FunctionDef: `csda_table_spline`

Interpolates a CSDA table to form a spline which maps a range to a
kinematic energy estimate.

Parameters
----------
particle_type : int
    Particle type ID to construct splines. Maps are
    avaible for muons, pions, kaons and protons.
value : str, default 'T'
    Value to provide for each range value (one of 'T' or 'dE/dx')
table_dir : str, default 'csda_tables'
    Relative path to the CSDA range tables

Returns
-------
callable
    Function mapping range (cm) to Kinetic E (MeV) or dE/dx (MeV/cm)

---
### ClassDef: `CSDAEnergyProcessor`

Reconstruct the kinetic energy of tracks based on their range in liquid
argon using the continuous slowing down approximation (CSDA).

---
### ClassDef: `CSVWriter`

Writes data to a CSV file.

Builds a CSV file to store the output of the analysis tools. It can only be
used to store relatively basic quantities (scalars, strings, etc.).

Typical configuration should look like:

.. code-block:: yaml

    io:
      ...
      writer:
        name: csv
        file_name: output.csv

---
### FunctionDef: `current`

Simple function which returns the current time (wall and cpu).

Returns
-------
Time
   Current time

---
### FunctionDef: `data_keys`

Returns a list of data product names.

Returns
-------
List[str]
    List of data product names

---
### ClassDef: `DataBase`

Base class of all data structures.

Defines basic methods shared by all data structures.

---
### ClassDef: `DataFormat`

Data structure to hold writing parameters.

Attributes
----------
dtype : type, optional
    Data type
class_name : str, optional
    Name of the class the information comes from
width : int, defaul t0
    Width of the tensor to store, if it is a tensor
merge : bool, default False
    Whether to merge lists of arrays into a single dataset
scalar : bool, default False
    Whether the data is a scalar object or not

---
### FunctionDef: `dataset_factory`

Instantiates a Dataset based on a configuration.

The Dataset type is specified in configuration under `io.dataset.name`.
The name must match the name of a class under `spine.io.datasets`.

Parameters
----------
dataset_cfg : dict
    Dataset configuration dictionary
entry_list: list, optional
    List of entry numbers to include in the dataset
dtype : str, optional
    Data type to cast the input data to (to match the downstream model)

Returns
-------
torch.utils.data.Dataset
    Initialized dataset

Note
----
Currently the choice is limited to `LArCVDataset` only.

---
### ClassDef: `DBSCAN`

Uses DBSCAN to find locally-dense particle fragments.

It uses sklearn's DBSCAN implementation to fragment each of the particle
shapes into dense instances. Runs DBSCAN on each requested semantic class
separately, in one of three ways:
- Run pure DBSCAN on all the voxels in that class
- Runs DBSCAN on PPN point-masked voxels and then associates the 
  leftovers based on proximity to existing instances.
- Use a graph-based method to cluster tracks based on PPN vertices. This
  technique can only be used on tracks.

---
### FunctionDef: `dbscan`

Runs DBSCAN on 3D points and returns the group assignments.

Notes
-----
The traditional 'min_samples' is always set to 1 here.

Parameters
----------
x : np.ndarray
    (N, 3) array of point coordinates
eps : float
    Distance below which two points are considered neighbors
metric : str, default 'euclidean'
    Distance metric used to compute pdist

Returns
-------
np.ndarray
    (N) Group assignments

---
### FunctionDef: `dbscan_points`

Runs DBSCAN on an input point cloud.

Returns the clusters as a list of indexes.

Parameters
----------
coordinates : np.ndarray
    Set of point coordinates
eps : float, default 1.999
    Distance parameter of DBSCAN
min_samples : int, default 1
    Minimum number of points in a cluster to be valid
metric : str, default 'euclidean'
    Metric used to compute distances

Returns
-------
List[np.ndarray]
    List of cluster indexes

---
### FunctionDef: `decoder`

UResNeXt Decoder

INPUTS:
    - encoderTensors (list of SparseTensor): output of encoder.
RETURNS:
    - decoderTensors (list of SparseTensor):
    list of feature tensors in decoding path at each spatial resolution.

---
### FunctionDef: `decoder`

UResNeXt Decoder

INPUTS:
    - encoderTensors (list of SparseTensor): output of encoder.
RETURNS:
    - decoderTensors (list of SparseTensor):
    list of feature tensors in decoding path at each spatial resolution.

---
### FunctionDef: `decoder`

Vanilla FPN Decoder

INPUTS:
    - encoderTensors (list of SparseTensor): output of encoder.
RETURNS:
    - decoderTensors (list of SparseTensor):
    list of feature tensors in decoding path at each spatial resolution.

---
### FunctionDef: `decoder`

Vanilla UResNet Decoder
INPUTS:
    - encoderTensors (list of SparseTensor): output of encoder.
RETURNS:
    - decoderTensors (list of SparseTensor):
    list of feature tensors in decoding path at each spatial resolution.

---
### ClassDef: `DefaultKernel`

Kernel producing edge score based on feature L2 similarity.

This Kernel assumes that the upstream embedder produces a set of spatial
and embedding coordinates and computes the L2 similarity between the two
node feature vectors. It scales the L2 distance by the covariance and
penalizes for cluster size dissimilarity.

---
### FunctionDef: `define_containment_volumes`

This function defines a list of volumes to check containment against.

If the containment is checked against a constant volume, it is more
efficient to call this function once and call `check_containment`
reapitedly after.

Parameters
----------
margin : Union[float, List[float], np.array]
    Minimum distance from a detector wall to be considered contained:
    - If float: distance buffer is shared between all 6 walls
    - If [x,y,z]: distance is shared between pairs of walls facing
      each other and perpendicular to a shared axis
    - If [[x_low,x_up], [y_low,y_up], [z_low,z_up]]: distance is
      specified individually of each wall.
cathode_margin : float, optional
    If specified, sets a different margin for the cathode boundaries
mode : str, default 'module'
    Containement criterion (one of 'global', 'module', 'tpc'):
    - If 'tpc', makes sure it is contained within a single TPC
    - If 'module', makes sure it is contained within a single module
    - If 'detector', makes sure it is contained within in the detector
    - If 'source', use the origin of voxels to determine which TPC(s)
      contributed to them, and define volumes accordingly

---
### ClassDef: `DelaunayGraph`

Generates graphs based on the Delaunay triangulation of the input
node locations.

Triangulates the input, converts the triangles into a list of valid edges.

See :class:`GraphBase` for attributes/methods shared
across all graph constructors.

---
### FunctionDef: `delta_lar`

Density correction

Parameters
----------
bg : float
    Product of Lorentz beta and gamma (beta/sqrt(1-beta**2))

Returns
-------
float
    Density correction to the Bethe-Bloch function

---
### FunctionDef: `dep_modes`

Dictionary which makes the correspondance between the name of a true
object deposition attribute with the underlying deposition array it points to.

Returns
-------
Dict[str, str]
    Dictionary of (attribute, key) mapping for point depositions

---
### FunctionDef: `dep_modes`

Dictionary which makes the correspondance between the name of a true
object deposition attribute with the underlying deposition array it points to.

Returns
-------
Dict[str, str]
    Dictionary of (attribute, key) mapping for point depositions

---
### FunctionDef: `depositions_adapt_q_sum`

Total deposition value for the entire object in the adapted tensor
and in the original units.

Returns
-------
float
    Sum of all depositions that make up the object

---
### FunctionDef: `depositions_adapt_sum`

Total deposition value for the entire object in the adapted tensor.

Returns
-------
float
    Sum of all depositions that make up the object

---
### FunctionDef: `depositions_g4_sum`

Total deposition value for the entire object in the Geant4 tensor.

Returns
-------
float
    Sum of all depositions that make up the object

---
### FunctionDef: `depositions_q_sum`

Total deposition value for the entire object in the original units.

Returns
-------
float
    Sum of all depositions that make up the object

---
### FunctionDef: `depositions_sum`

Total deposition value for the entire object.

Returns
-------
float
    Sum of all depositions that make up the object

---
### FunctionDef: `dice_loss`

Parameters
----------
logits: (N x num_queries)
targets: (N x num_queries)

---
### FunctionDef: `dice_loss_flat`

Parameters
----------
logits: (N x num_queries)
targets: (N x num_queries)

---
### FunctionDef: `digamma_evd_loss`

Bayes risk loss for Dirichlet prior Evidential Learning

INPUTS:
    - alpha (FloatTensor): N x C concentration parameters, 
    where C is the number of class labels.
    - y (FloatTensor): N x C one-hot encoded class labels

RETURNS:
    - loss (FloatTensor): N x 1 non-reduced loss for each example. 

---
### FunctionDef: `dimension`

Number of dimensions in the image.

Returns
-------
int
    Number of dimensions in the image

---
### FunctionDef: `dimensions`

Dimensions of the box.

Returns
-------
np.ndarray
    Box dimensions

---
### FunctionDef: `directed_batch_ids`

Returns the batch ID of each element in the directed index.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (N) Complete batch ID array, one per element

---
### FunctionDef: `directed_counts`

Returns the number of edges per entry, counting edges once even
if they are bidirectional.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (B) Complete batch ID array, one per element

---
### FunctionDef: `directed_index`

Index of the directed graph. If a graph is undirected, it only
returns one of the two edges corresponding to a connection.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (2, E//2) Underlying batch of edge indexes

---
### FunctionDef: `directed_index_t`

Index of the directed graph, transposed. If the graph is undirected,
it only returns one of the two edges corresponding to a connection.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (E//2, 2) Underlying batch of edge indexes, transposed

---
### ClassDef: `DirectionProcessor`

Reconstructs the direction of fragments and/or particles w.r.t. to
their start (and end for tracks) points.

This modules assign the `start_dir` and `end_dir` attributes.

---
### ClassDef: `DiscriminativeLoss`

Implementation of the Discriminative Loss Function in Pytorch.
https://arxiv.org/pdf/1708.02551.pdf
Note that there are many other implementations in Github, yet here
we tailor it for use in conjuction with Sparse UResNet.

---
### ClassDef: `DistributedProxySampler`

Sampler that restricts data loading to a subset of input sampler indices.

It is especially useful in conjunction with
:class:`torch.nn.parallel.DistributedDataParallel`. In such case, each
process can pass a DistributedSampler instance as a DataLoader sampler,
and load a subset of the original dataset that is exclusive to it.

---
### FunctionDef: `draw`

Finds all training and validation log files inside the specified
directory and draws an evolution plot of the requested quantities.

Parameters
----------
model : Union[str, List[str]]
    Model (folder) / list of models names under the main directory
metric : Union[str, List[str]]
    Metric / list of metrics to draw
limits : Union[List[float], Dict[str, List[float]]], optional
    List of y boundaries for the plot. If specified as a dictionary,
    can be used to specify different boundaries for each metric.
model_name : Union[str, Dict[str, str]], optional
    Name of the model as displayed in the legend. If there are multiple
    models, provide a dictionary which maps each model onto a name
metric_name : Union[str, Dict[str, str]], optional
    Name of the metric as displayed in the legend. If there are multiple
    metrics, provide a dictionary which maps each metric onto a name
max_iter : int, optional
    Maximum number of iterations to include in the plot
step : int, optional
    Step between two consecutive iterations that are represented
smoothing : int, optional
    Number of iteration over which to average the metric values
iter_per_epoch : float, optional
    Number of iterations to complete an dataset epoch
same_plot : bool, default True
    If `True`, draw all metrics on the same plot
leg_ncols : int, default 1
    Number of columns in the legend
figure_name : str, optional
    Name of the figure. If specified, figure is saved

---
### FunctionDef: `draw_confusion_matrix`

Draws the confusion matrix from a file produced by the analysis
script used to evaluate the classification accuracy.

Parameters
----------
file_path : str
    Path to the file which contains the classification metrics
num_classes : int, optional
    Number of classes to represent
mapping : dict, optional
    Mapping between the stored class and a redefined set of classes
show_counts : bool, default False
    Show the number of entries in the contingency matrix
class_names : list, optional
    Labels for each class
figsize : tuple, default (9, 6)
    Figure size
norm_axis : int, default 0
    Normalization axis (0: recall, 1: precision)

---
### ClassDef: `Drawer`

Handles drawing the true/reconstructed output.

This class is given the entire input/output dictionary from one entry and
provides functions to represent the output.

---
### FunctionDef: `drift_axis`

Drift axis for the module (shared between chambers).

Returns
-------
int
    Axis along which electrons drift in this module (0, 1 or 2)

---
### FunctionDef: `drift_sign`

Sign of drift w.r.t. to the drift axis orientation.

Returns
-------
int
    Returns the sign of the drift vector w.r.t. to the drift axis

---
### ClassDef: `Driver`

Central SPINE driver.

Processes global configuration and runs the appropriate modules:
  1. Load data
  2. Run the model forward (including loss) and backward (if training)
  3. Unwrap batched data
  4. Build representations
  5. Run post-processing
  6. Run analysis scripts
  7. Write to file

It takes a configuration dictionary of the form:

.. code-block:: yaml

    base:
      <Base driver configuration>
    io:
      <Input/output configuration>
    model:
      <Model architecture>
    build:
      <Rules as to how to build reconstructed object representations>
    post:
      <Post-processors>
    ana:
      <Analysis scripts>

---
### ClassDef: `DropoutBlock`

Convolution block which operates a sequence of
two (convolution + dropout + nomalization + activation) steps.

---
### FunctionDef: `dual_figure3d`

Function which returns a plotly.graph_objs.Figure with two set of traces
side-by-side in separate subplots.

Parameters
----------
traces_left : List[object]
    List of plotly traces to draw in the left subplot
traces_right : List[object]
    List of plotly traces to draw in the right subplot
layout : plotly.Layout, optional
    Plotly layout
titles : List[str], optional
    Titles of the two subplots
width : int, default 1000
    Width of the layout in pixels
height : int, default 500
    Height of the layout in pixels
synchronize : bool, default False
    If True, matches the camera position/angle of one plot to the other
margin : dict, optional
    Specifies the margin in each subplot
**kwargs : dict, optional
    List of additional arguments to pass to plotly.graph_objs.Layout

Returns
-------
plotly.graph_objs.Figure
    Plotly figure with the two subplots

---
### ClassDef: `DummyDataset`

Dataset with the basic attributes needed to tes the samplers.

---
### ClassDef: `DUQParticleClassifier`

Uncertainty Estimation Using a Single Deep Deterministic Neural Network
https://arxiv.org/pdf/2003.02037.pdf
Joost van Amersfoort, Lewis Smith, Yee Whye Teh, Yarin Gal.

Pytorch Implementation for SparseConvNets with MinkowskiEngine backend.

---
### ClassDef: `DUQUResNet`

Single Pass Deep Uncertainty Quantification Network
Original Paper: https://arxiv.org/abs/2003.02037

Implementation adapted from the DUQ main Github Repository:
https://github.com/y0ast/deterministic-uncertainty-quantification

Author: Joost van Amersfoort

---
### ClassDef: `EConvNodeLayer`

EdgeConv module for extracting graph node features.

This model first aggregates the feature vector (N_c) of the node being
updated with a summary statistic of the difference between the features
of the node and those of other connected nodes to form a (2*N_c) feature
vector. This feature vector is then passed through a multi-layer
perceptron (MLP) and outputs a (C, N_o) vector, with N_o the width
of the unedrlying MLP (feature size of the hidden representation).

Source: https://arxiv.org/abs/1801.07829

---
### FunctionDef: `edge_assignment`

Determines which edges are turned on based on the group ID of the 
clusters they are connecting. 

Parameters
----------
edge_index: np.ndarray
    (E, 2) Sparse incidence matrix
group_ids : np.ndarray
    (C) Cluster group IDs

Returns
-------
np.ndarray:
    (E) Array specifying on/off edges

---
### FunctionDef: `edge_assignment_batch`

Batched version of :func:`edge_assignment`.

Parameters
----------
edge_index: EdgeIndexBatch
    (2, E) Sparse incidence matrix
group_ids : TensorBatch
    (C) Cluster group IDs

Returns
-------
TensorBatch
    (E) Array specifying on/off edges

---
### FunctionDef: `edge_assignment_forest`

Determines which edges must be turned on based on to form a
minimum-spanning tree (MST) for each node group. 

For each group, find the most likely spanning tree, label the edges in the
tree as 1. For all other edges, apply loss only if in separate groups. If
undirected, also assign symmetric path. This method enforces that the
network minmally forms a forest graph on the input nodes, with each tree
in the forest spanning a target node group.

Parameters
----------
edge_index : np.ndarray
    (E, 2) Input sparse incidence matrix (on clusters)
edge_pred : np.ndarray
    (E, 2) Logits associated with each edge
group_ids : np.ndarray
    (C) Cluster group IDs

Returns
-------
np.ndarray:
    (E) Array specifying on/off edges
np.ndarray
    (E) Valid edge mask (edges to apply the loss to)

---
### FunctionDef: `edge_assignment_forest_batch`

Batched version of :func:`edge_assignment_forest`.

Parameters
----------
edge_index : EdgeIndexBatch
    (2, E) Input sparse incidence matrix (on clusters)
edge_pred : TensorBatch
    (E, 2) Logits associated with each edge
group_ids : TensorBatch
    (C) Cluster group IDs

Returns
-------
TensorBatch
    (E) Array specifying on/off edges
TensorBatch
    (E) Array specifying edges to apply the loss to

---
### FunctionDef: `edge_assignment_from_graph`

Determines which edges are turned on based on whether they appear in
a reference list of true edges or not.

Parameters
----------
edge_index : EdgeIndexBatch
    (E, 2) Input sparse incidence matrix (on clusters)
truth_edge_index : TensorBatch
    (E', 2) Label sparse incidence matrix (on particles)
part_ids : np.ndarray
    (C) Particle IDs of the clusters

Returns
-------
np.ndarray:
    (E) Array specifying on/off edges

---
### FunctionDef: `edge_assignment_from_graph_batch`

Batched version of :func:`edge_assignment_from_graph`.

Parameters
----------
edge_index : EdgeIndexBatch
    (2, E) Input sparse incidence matrix (on clusters)
truth_edge_index : TensorBatch
    (2, E') Label sparse incidence matrix (on particles)
part_ids : TensorBatch
    (C) Particle IDs of the clusters

Returns
-------
TensorBatch
    (E) Array specifying on/off edges

---
### FunctionDef: `edge_assignment_score`

Finds the graph that produces the lowest grouping score by iteratively
adding the next most likely edge, if it improves the the score. This method
effectively builds a spanning tree.

Parameters
----------
edge_index : np.ndarray
    (2, E) Sparse incidence matrix
edge_pred : np.ndarray
    (E, 2) Logits associated with each edge
num_nodes : int
    Number of nodes in the graph, C
track_node : np.ndarray, optional
    (C) Whether a node is a track fragment/particle or not

Returns
-------
np.ndarray
    (E', 2) Optimal incidence matrix
np.ndarray
    (C) Optimal group ID for each node
float
    Score of the optimal incidence matrix

---
### FunctionDef: `edge_assignment_score_batch`

Batched version of :func:`edge_assignment_score`.

Parameters
----------
edge_index : EdgeIndexBatch
    (2, E) Sparse incidence matrix
edge_pred : TensorBatch
    (E, 2) Logits associated with each edge
clusts : IndexBatch
    (C) List of cluster indexes
track_node : TensorBatch, optional
    (C) Whether a node is a track fragment/particle or not

Returns
-------
np.ndarray
    (E', 2) Optimal incidence matrix
np.ndarray
    (C) Optimal group ID for each node
float
    Score of the optimal incidence matrix

---
### FunctionDef: `edge_encoder_factory`

Instantiates an edge encoder from a configuration dictionary.

Parameters
----------
cfg : dict
    Edge encoder configuration

Returns
-------
object
    Instantiated edge encoder

---
### FunctionDef: `edge_layer_factory`

Instantiates a GNN edge update layer from a configuration dictionary.

Parameters
----------
cfg : dict
    GNN edge update layer configuration
node_in : int
    Number of input node features
edge_in : int
    Number of input edge features
glob_in : int
    Number of input global graph features

Returns
-------
object
    Instantiated GNN edge update layer

---
### FunctionDef: `edge_loss_factory`

Instantiates an edge loss from a configuration dictionary.

Parameters
----------
cfg : dict
    Edge loss configuration

Returns
-------
object
    Instantiated edge loss

---
### FunctionDef: `edge_purity_mask`

Creates a mask that is `True` only for edges which connect two nodes
that both belong to a common group which has a single clear primary. 

This is useful for shower clustering only, for which there can be no or
multiple primaries in the group, making the the edge classification
ill-defined (no primary typically indicates a shower which originates
outside of the active volume).

Note: It is possible that the single true primary has been broken into
several nodes; that is acceptable.

Parameters
----------
edge_index : np.ndarray
    (2, E) Sparse incidence matrix
part_ids : np.ndarray
    (C) Array of cluster particle IDs
group_ids : np.ndarray
    (C) Array of cluster group IDs
primary_ids : np.ndarray
    (C) Array of cluster primary IDs

Returns
-------
np.ndarray
    (E) High purity edge mask

---
### FunctionDef: `edge_purity_mask_batch`

Batched version of :func:`edge_purity_mask`.

Parameters
----------
edge_index : EdgeIndexBatch
    (2, E) Sparse incidence matrix
part_ids : TensorBatch
    (C) Array of cluster particle IDs
group_ids : TensorBatch
    (C) Array of cluster group IDs
primary_ids : TensorBatch
    (C) Array of cluster primary IDs

Returns
-------
np.ndarray
    (E) High purity edge mask

---
### ClassDef: `EdgeChannelLoss`

Takes the two-channel edge output of the GNN and optimizes edge-wise
scores such that edges that connect nodes that belong to common instance
are given a high score.

For use in config:

..  code-block:: yaml

    model:
      name: grappa
      modules:
        grappa_loss:
          edge_loss:
            name: channel
            <dictionary of arguments to pass to the loss>

See configuration files prefixed with `grappa_` under the `config`
directory for detailed examples of working configurations.

---
### ClassDef: `EdgeIndexBatch`

Batched edge index with the necessary methods to slice it.

Attributes
----------
offsets : Union[np.ndarray, torch.Tensor]
    (B) Offsets between successive indexes in the batch
directed : bool
    Whether the edge index is directed or undirected

---
### ClassDef: `EdgeLoss`

Loss applied to edge scores produced by a GraphSPICE.

This loss simply treats the edge score as logit predictions and compares
them to edge labels (simple classification task).

---
### FunctionDef: `edges`

Returns the bin edges in each axis.

Returns
-------
np.ndarray
    (D) List of (N_i + 1) edges per dimension, with N_i the number
    of bins in the the ith dimension

---
### FunctionDef: `eff`

Assignment efficiency, evaluated per true cluster and averaged.

Parameters
----------
truth : np.ndarray
    (N) Set of true labels
pred : np.ndarray
    (N) Set of predicted labels
batch_ids : np.ndarray, optional
    (N) Batch IDs
per_cluster : bool, default True
    If `True`, computes the efficiency per truth cluster, than averages it

Returns
-------
float
    Assignment efficiency

---
### FunctionDef: `ellipsoid_trace`

Converts a cloud of points or a covariance matrix into a 3D ellipsoid.

This function uses the centroid and the covariance matrix of a cloud of
points to define an ellipsoid which would encompass a user-defined fraction
`contour` of all the points, were the points distributed following
a 3D Gaussian.

Parameters
----------
points : np.ndarray, optional
    (N, 3) Array of point coordinates
centroid : np.ndarray, optional
    (3) Centroid
covmat : np.ndarray, optional
    (3, 3) Covariance matrix which defines the ellipsoid shape
contour : float, default 0.5
    Fraction of the points contained in the ellipsoid, under the
    Gaussian distribution assumption
num_samples : int, default 10
    Number of points sampled along theta and phi in the spherical coordinate
    system of the ellipsoid. A larger number increases the resolution.
color : Union[str, float], optional
    Color of ellipse
intensity : Union[int, float], optional
    Color intensity of the box along the colorscale axis
hovertext : Union[int, str, np.ndarray], optional
    Text associated with the box
showscale : bool, default False
    If True, show the colorscale of the :class:`plotly.graph_objs.Mesh3d`
**kwargs : dict, optional
    Additional parameters to pass to the underlying
    :class:`plotly.graph_objs.Mesh3d` object

---
### FunctionDef: `ellipsoid_traces`

Function which produces a list of plotly traces of ellipsoids given a
list of centroids and one covariance matrix in x, y and z.

Parameters
----------
centroids : np.ndarray
    (N, 3) Positions of each of the ellipsoid centroids
covmat : np.ndarray
    (3, 3) Covariance matrix which defines any of the base ellipsoid shape
color : Union[str, np.ndarray], optional
    Color of ellipsoids or list of color of ellispoids
hovertext : Union[int, str, np.ndarray], optional
    Text associated with every ellipsoid or each ellipsoid
cmin : float, optional
    Minimum value along the color scale
cmax : float, optional
    Maximum value along the color scale
shared_legend : bool, default True
    If True, the plotly legend of all ellipsoids is shared as one
legendgroup : str, optional
    Legend group to be shared between all boxes
showlegend : bool, default `True`
    Whether to show legends on not
name : str, optional
    Name of the trace(s)
**kwargs : dict, optional
    List of additional arguments to pass to the underlying list of
    :class:`plotly.graph_objs.Mesh3D`

Returns
-------
Union[List[plotly.graph_objs.Mesh3D]]
    Ellipsoid traces

---
### ClassDef: `EmptyClusterEdgeEncoder`

Produces empty cluster edge features.

---
### ClassDef: `EmptyClusterGlobalEncoder`

Produces empty global graph features.

---
### ClassDef: `EmptyClusterNodeEncoder`

Produces empty cluster node features.

---
### FunctionDef: `encoder`

UResNeXt Encoder.

INPUTS:
    - x (SparseTensor): MinkowskiEngine SparseTensor

RETURNS:
    - result (dict): dictionary of encoder output with
    intermediate feature planes:
      1) encoderTensors (list): list of intermediate SparseTensors
      2) finalTensor (SparseTensor): feature tensor at
      deepest layer.

---
### FunctionDef: `encoder`

UResNeXt Encoder.

INPUTS:
    - x (SparseTensor): MinkowskiEngine SparseTensor

RETURNS:
    - result (dict): dictionary of encoder output with
    intermediate feature planes:
      1) encoderTensors (list): list of intermediate SparseTensors
      2) finalTensor (SparseTensor): feature tensor at
      deepest layer.

---
### FunctionDef: `encoder`

Vanilla FPN Encoder.

INPUTS:
    - x (SparseTensor): MinkowskiEngine SparseTensor

RETURNS:
    - result (dict): dictionary of encoder output with
    intermediate feature planes:
      1) encoderTensors (list): list of intermediate SparseTensors
      2) finalTensor (SparseTensor): feature tensor at
      deepest layer.

---
### FunctionDef: `encoder`

Vanilla UResNet Encoder.

INPUTS:
    - x (SparseTensor): MinkowskiEngine SparseTensor

RETURNS:
    - result (dict): dictionary of encoder output with
    intermediate feature planes:
      1) encoderTensors (list): list of intermediate SparseTensors
      2) finalTensor (SparseTensor): feature tensor at
      deepest layer.

---
### FunctionDef: `encoder`

Vanilla UResNet Encoder.

INPUTS:
    - x (SparseTensor): MinkowskiEngine SparseTensor

RETURNS:
    - result (dict): dictionary of encoder output with
    intermediate feature planes:
      1) encoderTensors (list): list of intermediate SparseTensors
      2) finalTensor (SparseTensor): feature tensor at
      deepest layer.

---
### FunctionDef: `encoder`

Vanilla UResNet Encoder.

INPUTS:
    - x (SparseTensor): MinkowskiEngine SparseTensor

RETURNS:
    - result (dict): dictionary of encoder output with
    intermediate feature planes:
      1) encoderTensors (list): list of intermediate SparseTensors
      2) finalTensor (SparseTensor): feature tensor at
      deepest layer.

---
### FunctionDef: `encoder_factory`

Instantiates an image encoder from a configuration dictionary.

Parameters
----------
cfg : dict
    Encoder configuration

Returns
-------
object
    Instantiated encoder

---
### FunctionDef: `end_dir`

Converts the final momentum to a direction vector.

Note that if a particle stops, this is unreliable as an estimate of the
direction of the particle before it stops.

Returns
-------
np.ndarray
    (3) End direction vector

---
### FunctionDef: `end_dir`

Converts the final momentum to a direction vector.

Note that if a particle stops, this is unreliable as an estimate of the
direction of the particle before it stops.

Returns
-------
np.ndarray
    (3) End direction vector

---
### FunctionDef: `end_p`

Computes the magnitude of the final momentum.

Returns
-------
float
    Norm of the final momentum vector

---
### FunctionDef: `enum_attrs`

Fetches the list of enumerated attributes as a dictionary.

Returns
-------
Dict[int, Dict[int, str]]
    Dictionary which maps names onto enumerator descriptors

---
### FunctionDef: `enum_factory`

Parses an enumerated object from string name(s) to value(s).

Parameters
----------
enum : str
    Name of the enumerated type
value : Union[str, List[str]]
    Name or names of the enumerated objects (from config)

Returns
-------
Union[int, List[int]]
    Value or values of the enumerated objects

---
### FunctionDef: `evaluate`

Evaluate the clustering accuracy of a graph.

Parameters
----------
graph : dict
    Dictionary of graph attributes organized by batch and shape
mean : bool, default False
    If `True`, returns the batch-averaged metric values

Returns
-------
dict
    Dictionary of accuracy metrics

---
### FunctionDef: `evd_kl_divergence`

KL Divergence between Dir(p|alpha) and Dir(p|beta), where
alpha and beta are Dirichlet concentration parameters. 

INPUTS:
    - alpha (FloatTensor): N x C concentration parameters
    - beta (FloatTensor): N x C concentration parameters. In case of 
    truth labels, this is a one-hot encoded class label tensor. 
    If None, this will compute the KL Divergence between Dir(p|alpha)
    and Dir(p|1), which is the uniform distribution over C classes. 

RETURNS:
    - loss (FloatTensor): N x 1 non-reduced kl divergence loss. 

---
### ClassDef: `EVDLoss`

Base class for loss used in the paper:
Sensoy et. al., Evidential Deep Learning to Quantify 
Classification Uncertainty

---
### ClassDef: `EventAna`

Class which saves basic event information (and their matches).

---
### FunctionDef: `evidential_forward`

Forwarding operation for evidential segmentation network.

---
### ClassDef: `EvidentialModel`

Model which produces evidential predictions with an MLP backbone.

---
### ClassDef: `ExpandAs`

Expands a one dimensional feature tensor to a higher dimension.

Given a sparse tensor with one dimensional features, expand the
feature map to a given shape and return a newly constructed
ME.SparseTensor. This is used to expand a score array and apply
it to the entire feature tensor of the the input.

---
### ClassDef: `ExpandAs`

Given a sparse tensor with one dimensional features, expand the
feature map to given shape and return a newly constructed
ME.SparseTensor.

    - x (ME.SparseTensor): with x.F.shape[1] == 1
    - shape (tuple)

---
### FunctionDef: `expected_dedxs`

Computes the expected dE/dx values given a set of residual ranges.

Parameters
----------
rrs : np.ndarray
    (S) Residual range values (one per track segment)
pid : int
    Particle species enumerator

Returns
-------
np.ndarray
    Expected dE/dxs values from a table or the theory

---
### FunctionDef: `farthest_pair`

Algorithm which finds the two points which are
farthest from each other in a set.

Two algorithms:
- `brute`: compute pdist, use argmax
- `recursive`: Start with the first point in one set, find the farthest
               point in the other, move to that point, repeat. This
               algorithm is *not* exact, but a good and very quick proxy.

Parameters
----------
x : np.ndarray
    (N, 3) array of point coordinates
algorithm : str
    Name of the algorithm to use: `brute` or `recursive`

Returns
-------
int
    ID of the first point that makes up the pair
int
    ID of the second point that makes up the pair
float
    Distance between the two points

---
### FunctionDef: `feature_embedding_loss`

Compute discriminative feature embedding loss.

INPUTS:
    - ft_emb (N x F)
    - groups (N)
    - ft_centroids (N_c X F)

---
### ClassDef: `FiducialProcessor`

Check that an interaction vertex is in a user-defined fiducial volume.

The fiducial volume is defined as a margin distances from each of the
detector walls.

---
### ClassDef: `FieldCalibrator`

Applies position corrections to account for field non-uniformities
(space charge, cathode distrotions, etc.)

---
### FunctionDef: `filter_class`

Filter classes according to segmentation label.

---
### FunctionDef: `filter_class`

Filter classes according to segmentation label.

---
### FunctionDef: `filter_class`

Filter classes according to segmentation label.

---
### FunctionDef: `filter_class`

Filter the list of pixels to those in the list of requested shapes.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
    - N is the the total number of voxels in the image
    - 1 is the batch ID
    - D is the number of dimensions in the input image
    - N_f is the number of features per voxel
seg_label : TensorBatch
    (N, 1 + D + 1) Tensor of segmentation labels
    - 1 is the segmentation label
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels
    - N_c is is the number of cluster labels

Parameters
----------
data : TensorBatch
    (M, 1+ + D + Nf) restricted tensor of voxel/value pairs
seg_label : TensorBatch
    (M, 1 + D + 1) restricted tensor of segmentation labels
clust_label : TensorBatch
    (M, 1 + D + N_c) Restricted tnesor of cluster labels
index : torch.Tensor
    (M) Index to narrow down the original tensor
counts : torch.Tensor
    (B) Number of restricted points in each batch entry

---
### FunctionDef: `filter_class`

Filter the list of pixels to those in the list of requested shapes.

Parameters
----------
seg_label : TensorBatch
    (N, 1 + D + 1) Tensor of segmentation labels
    - 1 is the segmentation label
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels
    - N_c is is the number of cluster labels
filter_index : IndexBatch
    (M) Index to narrow down the original tensor

Parameters
----------
seg_label : TensorBatch
    (M, 1 + D + 1) restricted tensor of segmentation labels
clust_label : TensorBatch
    (M, 1 + D + N_c) Restricted tnesor of cluster labels

---
### FunctionDef: `filter_duplicate_voxels`

Returns an array with no duplicate voxel coordinates.

If there are multiple voxels with the same coordinates, this algorithm
simply picks the first one.

Parameters
----------
data: np.ndarray
    (N, 3) Lexicographically sorted matrix of voxel coordinates

Returns
-------
np.ndarray
    (N) Boolean mask which is False for pixels to remove

---
### FunctionDef: `filter_duplicate_voxels_ref`

Returns an array with no duplicate voxel coordinates.

If there are multiple voxels with the same coordinates, this algorithm
picks the voxel which has the shape label that comes first in order of
precedence. If multiple voxels with the same precedence index share voxel
coordinates, the first one is picked.

Parameters
----------
data: np.ndarray
    (N, 3) Lexicographically sorted matrix of voxel coordinates
reference: np.ndarray
    (N) Array of values which have to follow the precedence order
precedence: list
    (C) Array of classes in the reference array, ordered by precedence

Returns
-------
np.ndarray
    (N) Boolean mask which is False for pixels to remove

---
### FunctionDef: `filter_invalid_nodes`

Remove invalid node from a graph, bridge gaps formed by the filtering.

Each time a node is removed, the function proceeds as follows:
- If the node has no children, remove any edges that connect to it
- If the node has children:
  - If it does not have a parent, remove any edges from it
  - If it has a parent, connect the parent to its children

Parameters
----------
edge_index : np.ndarray
    (E, 2) Original graph incidence map
invalid_nodes : np.ndarray
    (N) List of nodes to remove from the original graph incidence map

Returns
-------
np.ndarray
    (E', 2) Filtered graph incidence map

---
### FunctionDef: `filter_voxels_ref`

Removes voxels thsat do not appear in a reference tensor.

Returns an array which does not contain any voxels which do not belong to
the reference array. The reference array must contain a subset of the
voxels in the array to be filtered.

Assumes both arrays are lexicographically sorted, the reference matrix
contains no duplicates and is a subset of the matrix to be filtered.

Parameters
----------
data: np.ndarray
    (N, 3) Lexicographically sorted matrix of voxel coordinates to filter
reference: np.ndarray
    (N, 3) Lexicographically sorted matrix of voxel coordinates to match

Returns
-------
np.ndarray
    (N) Boolean mask which is False for pixels to remove

---
### FunctionDef: `final_factory`

Instantiates a final layer from a configuration dictionary.

Parameters
----------
in_channels : int
    Number of features input into the final layer
**cfg : dict
    Final layer configuration

Returns
-------
object
    Instantiated final layer

---
### ClassDef: `FinalEvidential`

Simple wrapper class for a final Evidential model.

---
### ClassDef: `FinalLinear`

Simple wrapper class for a final linear layer operation.

---
### ClassDef: `FinalMLP`

Simple wrapper class for a final MLP model.

---
### FunctionDef: `find_cluster_means`

For a given image, compute the centroids \mu_c for each
cluster label in the embedding space.

INPUTS:
    features (torch.Tensor) - the pixel embeddings, shape=(N, d) where
    N is the number of pixels and d is the embedding space dimension.

    labels (torch.Tensor) - ground-truth group labels, shape=(N, )

OUTPUT:
    cluster_means (torch.Tensor) - (n_c, d) tensor where n_c is the number of
    distinct instances. Each row is a (1,d) vector corresponding to
    the coordinates of the i-th centroid.

---
### FunctionDef: `find_cluster_means`

For a given image, compute the centroids mu_c for each
cluster label in the embedding space.
Inputs:
    features (torch.Tensor): the pixel embeddings, shape=(N, d) where
    N is the number of pixels and d is the embedding space dimension.
    labels (torch.Tensor): ground-truth group labels, shape=(N, )
Returns:
    cluster_means (torch.Tensor): (n_c, d) tensor where n_c is the number of
    distinct instances. Each row is a (1,d) vector corresponding to
    the coordinates of the i-th centroid.

---
### FunctionDef: `find_cluster_means`

For a given image, compute the centroids mu_c for each
cluster label in the embedding space.
Inputs:
    features (torch.Tensor): the pixel embeddings, shape=(N, d) where
    N is the number of pixels and d is the embedding space dimension.
    labels (torch.Tensor): ground-truth group labels, shape=(N, )
Returns:
    cluster_means (torch.Tensor): (n_c, d) tensor where n_c is the number of
    distinct instances. Each row is a (1,d) vector corresponding to
    the coordinates of the i-th centroid.

---
### FunctionDef: `find_cluster_means`

For a given image, compute the centroids mu_c for each
cluster label in the embedding space.
Inputs:
    features (torch.Tensor): the pixel embeddings, shape=(N, d) where
    N is the number of pixels and d is the embedding space dimension.
    labels (torch.Tensor): ground-truth group labels, shape=(N, )
Returns:
    cluster_means (torch.Tensor): (n_c, d) tensor where n_c is the number of
    distinct instances. Each row is a (1,d) vector corresponding to
    the coordinates of the i-th centroid.

---
### FunctionDef: `find_cluster_means`

For a given image, compute the centroids mu_c for each
cluster label in the embedding space.
Inputs:
    features (torch.Tensor): the pixel embeddings, shape=(N, d) where
    N is the number of pixels and d is the embedding space dimension.
    labels (torch.Tensor): ground-truth group labels, shape=(N, )
Returns:
    cluster_means (torch.Tensor): (n_c, d) tensor where n_c is the number of
    distinct instances. Each row is a (1,d) vector corresponding to
    the coordinates of the i-th centroid.

---
### FunctionDef: `find_cluster_means_cuda`

For a given image, compute the centroids \mu_c for each
cluster label in the embedding space.

INPUTS:
    features (torch.Tensor) - the pixel embeddings, shape=(N, d) where
    N is the number of pixels and d is the embedding space dimension.

    labels (torch.Tensor) - ground-truth group labels, shape=(N, )

OUTPUT:
    cluster_means (torch.Tensor) - (n_c, d) tensor where n_c is the number of
    distinct instances. Each row is a (1,d) vector corresponding to
    the coordinates of the i-th centroid.

---
### FunctionDef: `find_key`

Checks if a :class:`pd.DataFrame` contains any of the keys listed
in a character-separated string.

If multiple keys match, pick the first one.

Parameters
----------
df : Union[pd.DataFrame, dict]
    Pandas dataframe or dictionary containing data
key_list : str
    Character-separated list of acceptable names for an attribute

Returns
-------
key : str
    First data key which matches one of the keys in the list
key_name : str
    First key in the list of acceptale names

---
### FunctionDef: `fit_predict`

Perform connected components clustering on a batch.

Parameters
----------
graph : dict
    Dictionary of graph attributes organized by batch and shape
edge_mode : str, default 'edge_pred'
    Attribute of the graph used to get the edge status
threshold : float, optional
    Override the edge score threshold set in the configuration
min_size : int, optional
    Override the minimum cluster size set in the configuration

Returns
-------
Union[np.ndarray, torch.Tensor]
    Node assignments

---
### FunctionDef: `fit_predict_entry`

Assign cluster labels to graph nodes based on edge assignments
in one entry.

Parameters
----------
node_coords : np.ndarray
    (N, 3) Set of point coordinates
edge_index : np.ndarray
    (E, 2) Set of edge source and target indices
edge_assn : np.ndarray
    (E) Boolean assignment for each edge (0 for off, 1 for on)
node_clusts : List[List[int]]
    (B, S) One list of node indices per (batch ID, shape) pair
edge_clusts : List[List[int]]
    (B, S) One list of edge indices per (batch ID, shape) pair
min_size : int, optional
    Override the minimum cluster size set in the configuration

Returns
-------
np.ndarry
    (N) Cluster assignments for each of the points in the input

---
### FunctionDef: `fit_predict_one`

Assign cluster labels to graph nodes based on edge assignments
in one graph, i.e. one (entry, shape) pair.

Parameters
----------
node_coords : np.ndarray
    (N, 3) Set of point coordinates
edge_index : np.ndarray
    (E, 2) Set of edge source and target indices
edge_assn : np.ndarray
    (E) Boolean assignment for each edge (0 for off, 1 for on)
offset : int
    Offset to apply to assigned nodes
min_size : int, optional
    Override the minimum cluster size set in the configuration

Returns
-------
np.ndarry
    (N) Cluster assignments for each of the points in the input

---
### FunctionDef: `fixed_length_attrs`

Fetches the dictionary of fixed-length array attributes as a dictionary.

Returns
-------
Dict[str, int]
    Dictionary which maps fixed-length attributes onto their length

---
### FunctionDef: `fixture_batch_edge_index`

Generate a batch of typical edge index data from the parsers.

Returns
-------
List[dict]
    One dictionary of data per entry in the batch

---
### FunctionDef: `fixture_batch_sparse`

Generate a batch of typical sparse data from the parsers.

Returns
-------
List[dict]
    One dictionary of data per entry in the batch

---
### FunctionDef: `fixture_cluster2d_event`

Generates one larcv.EventClusterPixel2D.

Returns
-------
larcv.EventClusterPixel2D
    Single dummy cluster of 2D sparse tensor

---
### FunctionDef: `fixture_cluster3d_event`

Generates one larcv.EventClusterVoxel3D.

Returns
-------
larcv.EventClusterVoxel3D
    Single dummy cluster of 3D sparse tensor

---
### FunctionDef: `fixture_crthit_event`

Generates one larcv.EventCRTHit.

Returns
-------
larcv.EventCRTHit
    Dummy list of larcv CRT hits

---
### FunctionDef: `fixture_dataset`

Generates a dummy dataset whith the necessary attributes and
methods to test the sampler classes.

---
### FunctionDef: `fixture_edge_index_list`

Generates a dummy list of unwrapped edge indexes.

---
### FunctionDef: `fixture_flash_event`

Generates one larcv.EventFlash.

Returns
-------
larcv.EventFlash
    Dummy list of larcv flashes

---
### FunctionDef: `fixture_flash_event_list`

Generates a list of larcv.EventFlash.

Returns
-------
larcv.EventFlash
    Dummy list of larcv flashes

---
### FunctionDef: `fixture_hdf5_data`

Download an HDF5 datafile here and cache it.

Parameters
----------
tmp_path : str
   Generic pytest fixture used to handle temporary test files
hdf5_datafile : str
   Name of the datafile to pull (default defined in pytest.ini)

---
### FunctionDef: `fixture_hdf5_output`

Create a dummy output path for an HDF5 file.

Parameters
----------
tmp_path : str
   Generic pytest fixture used to handle temporary test files

---
### FunctionDef: `fixture_index_batch`

Generates a dummy index batch.

---
### FunctionDef: `fixture_index_list`

Generates a dummy list of unwrapped index lists.

---
### FunctionDef: `fixture_larcv_data`

Download a LArCV ROOT datafile here and cache it.

Parameters
----------
tmp_path : str
   Generic pytest fixture used to handle temporary test files
larcv_datafile : str
   Name of the datafile to pull (default defined in pytest.ini)

---
### FunctionDef: `fixture_neutrino_event`

Generates one larcv.EventNeutrino.

Fills some of the attributes of the dummy neutrinos to be considered valid
in the parsers used to process them.

Returns
-------
larcv.EventNeutrino
    List of larcv.Neutrino objects

---
### FunctionDef: `fixture_particle_event`

Generates one larcv.EventParticle.

Fills some of the attributes of the dummy particles to be considered valid
in the parsers used to process them.

Returns
-------
larcv.EventParticle
    List of larcv.Particle objects

---
### FunctionDef: `fixture_sparse2d_event`

Generates one larcv.EventSparseTensor2D.

Returns
-------
larcv.EventSparseTensor2D
    Single dummy 2D sparse tensor

---
### FunctionDef: `fixture_sparse2d_event_list`

Generates one larcv.EventSparseTensor2D.

Returns
-------
List[larcv.EventSparseTensor2D]
    List of dummy 2D sparse tensor

---
### FunctionDef: `fixture_sparse3d_event`

Generates one larcv.EventSparseTensor3D.

Returns
-------
larcv.EventSparseTensor3D
    Single dummy 3D sparse tensor

---
### FunctionDef: `fixture_sparse3d_event_list`

Generates a list of larcv.EventSparseTensor3D.

Returns
-------
List[larcv.EventSparseTensor3D]
    List of dummy 3D sparse tensor

---
### FunctionDef: `fixture_sparse3d_seg_event`

Generates a single segmentation label larcv.EventSparseTensor3D.

Returns
-------
larcv.EventSparseTensor3D
    Single dummy segmentation label 3D sparse tensor

---
### FunctionDef: `fixture_tensor_batch`

Generates a dummy tensor batch.

---
### FunctionDef: `fixture_tensor_list`

Generates a dummy list of unwrapped tensors.

---
### FunctionDef: `fixture_trigger_event`

Generates one larcv.EventTrigger.

Returns
-------
larcv.EventTrigger
    Dummy trigger event

---
### ClassDef: `Flash`

Optical flash information.

Attributes
----------
id : int
    Index of the flash in the list
volume_id : int
    Index of the optical volume in which the flahs was recorded
time : float
    Time with respect to the trigger in microseconds
time_width : float
    Width of the flash in microseconds
time_abs : float
    Time in units of PMT readout clock
frame : int
    Frame number
in_beam_frame : bool
    Whether the flash is in the beam frame
on_beam_time : bool
    Whether the flash time is consistent with the beam window
total_pe : float
    Total number of PE in the flash
fast_to_total : float
    Fraction of the total PE contributed by the fast component
pe_per_optdet : np.ndarray
    (N) Fixed-length array of the number of PE per optical detector
center : np.ndarray
    Barycenter of the flash in detector coordinates
width : np.ndarray
    Spatial width of the flash in detector coordinates
units : str
    Units in which the position coordinates are expressed

---
### ClassDef: `FlashMatchingAna`

Class which computes and stores the necessary data to build a
semantic segmentation confusion matrix.

---
### ClassDef: `FlashMatchProcessor`

Associates TPC interactions with optical flashes.

---
### ClassDef: `FlashParser`

Copy construct Flash and return an array of `Flash`.

This parser also takes care of flashes that have been split between their
respective optical volumes, provided a `flash_event_list`. This parser
assumes that the trees are provided in order of the volume ID they
correspond to.

.. code-block. yaml
    schema:
      flashes:
        parser: flash
        flash_event_list:
          - flash_cryoE
          - flash_cryoW

---
### FunctionDef: `flatten_binary_scores`

Flattens predictions in the batch (binary case)
Remove labels equal to 'ignore'

---
### FunctionDef: `flatten_probas`

Flattens predictions in the batch

---
### FunctionDef: `form_clusters`

Builds a list of indexes corresponding to each cluster in the event.

The `data` tensor should only contain one entry.

Parameters
----------
data : Union[np.ndarray, torch.Tensor]
    Cluster label data tensor
min_size : int, default -1
    Minimum size of a cluster to be included in the list
column : int, default CLUST_COL
    Column of the label tensor to use to fetch the pixel cluster IDs
shapes : List[int], optional
    List of semantic classes to include in the list of cluster

Returns
-------
List[Union[np.ndarray, torch.Tensor]]
    (C) List of arrays of voxel indexes in each cluster
List[int]
    (C) Number of pixels in the mask for each cluster

---
### FunctionDef: `form_clusters_batch`

Batched version of :func:`form_clusters`.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
min_size : int, default -1
    Minimum size of a cluster to be included in the list
column : int, default CLUST_COL
    Column of the label tensor to use to fetch the pixel cluster IDs
shapes : List[int], optional
    List of semantic classes to include in the list of cluster

Returns
-------
IndexBatch
    Object used to index clusters within a batch of data

---
### FunctionDef: `forward`

        

---
### FunctionDef: `forward`

        

---
### FunctionDef: `forward`

        

---
### FunctionDef: `forward`

Applies mask and downsamples it for the next layer.

Parameters
----------
ghost_mask : ME.SparseTensor
    Current resolution ghost mask
premask_tensor : ME.SparseTensor
    Current resolution feature map to be pruned

Returns
-------
downsampled_mask : ME.SparseTensor)
    2x2 downsampled ghost mask
downsampled_tensor : ME.SparseTensor
    2x2 downsampled feature map

---
### FunctionDef: `forward`

Applies the edge channel loss to a batch of data.

Parameters
----------
clust_label : TensorBatch
    (N, 1 + D + N_f) Tensor of cluster labels for the batch
clusts : IndexBatch
    (C) Index which maps each cluster to a list of voxel IDs
edge_index : EdgeIndexBatch
    (2, E) Sparse ncidence matrix between clusters
edge_pred : TensorBatch
    (E, 2) Edge prediction logits (binary output)
true_edge_index : EdgeIndexBatch
    (2, E') True reference sparse incidence matrix
**kwargs : dict, optional
    Other labels/outputs of the model which are not relevant here

Returns
-------
loss : torch.Tensor
    Value of the loss
accuracy : float
    Value of the edge-wise classification accuracy
count : int
    Number of edges the loss was applied to

---
### FunctionDef: `forward`

Applies the edge loss to a batch of data.

Parameters
----------
clust_label : TensorBatch
    (N, 1 + D + N_c) Tensor of cluster labels
    - N_c is is the number of cluster labels
edge_attr : TensorBatch
    (E) Edge scores
edge_label : TensorBatch
    (E) Edge binary labels
**kwargs : dict, optional
    Additional upstream model outputs not used in this loss

Returns
-------
loss : torch.Tensor
    Value of the loss
accuracy : float
    Value of the edge-wise classification accuracy
iou : float
    IoU accuracy metric
count : int
    Number of edges the loss was applied to

---
### FunctionDef: `forward`

Applies the image classification loss to a batch of data.

Parameters
----------
labels : List[int]
    (B) List of image labels, one per entry in the batch
logits : TensorBatch
    (B, C) Tensor of predicted logits, one per entry in the batch
**kwargs : dict, optional
    Other labels/outputs of the model which are not relevant here

Returns
-------
loss : torch.Tensor
    Value of the loss
accuracy : float
    Value of the image-wise classification accuracy

---
### FunctionDef: `forward`

Applies the node classification loss to a batch of data.

Parameters
----------
clust_label : TensorBatch
    (N, 1 + D + N_f) Tensor of cluster labels for the batch
clusts : IndexBatch
    (C) Index which maps each cluster to a list of voxel IDs
node_pred : TensorBatch
    (C, 2) Node prediction logits (binary output)
coord_label : TensorBatch, optional
    (P, 1 + D + 8) Label start, end, time and shape for each point
**kwargs : dict, optional
    Other labels/outputs of the model which are not relevant here

Returns
-------
loss : torch.Tensor
    Value of the loss
accuracy : float
    Value of the node-wise classification accuracy
count : int
    Number of nodes the loss was applied to

---
### FunctionDef: `forward`

Applies the node orientation loss to a batch of data.

Parameters
----------
clust_label : TensorBatch
    (N, 1 + D + N_f) Tensor of cluster labels for the batch
coord_label : TensorBatch, optional
    (P, 1 + D + 8) Tensor of start/end point labels for each
    true particle in the image
clusts : IndexBatch
    (C) Index which maps each cluster to a list of voxel IDs
node_pred : TensorBatch
    (C, 2) Node prediction logits (binary output)
start_points : TensorBatch
    (C, 3) Start point features associated with each node
end_points : TensorBatch
    (C, 3) End point features associated with each node
**kwargs : dict, optional
    Other labels/outputs of the model which are not relevant here

Returns
-------
loss : torch.Tensor
    Value of the loss
accuracy : float
    Value of the node-wise orientation accuracy
count : int
    Number of nodes the loss was applied to

---
### FunctionDef: `forward`

Applies the node regression loss to a batch of data.

Parameters
----------
clust_label : TensorBatch
    (N, 1 + D + N_f) Tensor of cluster labels for the batch
clusts : IndexBatch
    (C) Index which maps each cluster to a list of voxel IDs
node_pred : TensorBatch
    (C, N_d) Node prediction
**kwargs : dict, optional
    Other labels/outputs of the model which are not relevant here

Returns
-------
loss : torch.Tensor
    Value of the loss
accuracy : float
    Value of the node-wise classification accuracy
count : int
    Number of nodes the loss was applied to

---
### FunctionDef: `forward`

Applies the node type loss to a batch of data.

Parameters
----------
clust_label : TensorBatch
    (N, 1 + D + N_f) Tensor of cluster labels for the batch
clusts : IndexBatch
    (C) Index which maps each cluster to a list of voxel IDs
node_pred : TensorBatch
    (C, 2) Node prediction logits (binary output)
meta : List[Meta], optional
    Image metadata information
start_points : TensorBatch, optional
    (C, 3) Node start positions
end_points : TensorBatch, optional
    (C, 3) Node end positions
**kwargs : dict, optional
    Other labels/outputs of the model which are not relevant here

Returns
-------
loss : torch.Tensor
    Value of the loss
accuracy : float
    Value of the node-wise classification accuracy
count : int
    Number of nodes the loss was applied to
primary_loss : torch.Tensor
    Value of the primary classification loss
primary_accuracy : float
    Value of the primary classification accuracy
reg_loss : torch.Tensor
    Value of the vertex regression loss
reg_accuracy : float
    Value of the vertex regression accuracy

---
### FunctionDef: `forward`

Applies the shower primary loss to a batch of data.

Parameters
----------
clust_label : TensorBatch
    (N, 1 + D + N_f) Tensor of cluster labels for the batch
clusts : IndexBatch
    (C) Index which maps each cluster to a list of voxel IDs
node_pred : TensorBatch
    (C, 2) Node prediction logits (binary output)
coord_label : TensorBatch, optional
    (P, 1 + D + 8) Label start, end, time and shape for each point
group_pred : TensorBatch, optional
    (C) Predicted group to which each node belongs to
**kwargs : dict, optional
    Other labels/outputs of the model which are not relevant here

Returns
-------
loss : torch.Tensor
    Value of the loss
accuracy : float
    Value of the node-wise classification accuracy
count : int
    Number of nodes the loss was applied to

---
### FunctionDef: `forward`

Apply the node/edge/global losses to the logits from GrapPA.

Parameters
----------
clust_label : TensorBatch
    (N, 1 + D + N_f) Tensor of voxel/value pairs
    - N is the the total number of voxels in the image
    - 1 is the batch ID
    - D is the number of dimensions in the input image
    - N_f is is the number of cluster labels
coord_label : TensorBatch, optional
    (P, 1 + D + 8) Tensor of start/end point labels for each
    true particle in the image
graph_label : EdgeIndexTensor, optional
    (2, E) Tensor of edges that correspond to physical
    connections between true particle in the image
iteration : int, optional
    Iteration index
**output : dict
    Output of the GrapPA model

---
### FunctionDef: `forward`

Compute the PPN loss for a batch of data.

The PPN loss comprises three components:
- Regression loss: position of the point of interest within a pixel
- Type: type of point of interest
- Mask: whether or not a pixel is within some distance of a point

Parameters
----------
final_tensor : TensorBatch
    Feature tensors at the deepest layer of the backbone UResNet
decoder_tensors : List[TensorBatch]
    Feature tensors of each of the decoding blocks
ghost : TensorBatch, optional
    Logits of the ghost predictions of the backbone UResNet
seg_label : TensorBatch, optional
    Segmentation label tensor

Returns
-------
dict
     Dictionary of outputs

---
### FunctionDef: `forward`

Compute the embeddings for one batch of data.

Inputs
------
data: TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
    - N is the the total number of voxels in the image
    - 1 is the batch ID
    - D is the number of dimensions in the input image
    - N_f is the number of features per voxel

Returns
-------
dict
    Dictionary of outputs

---
### FunctionDef: `forward`

Computes the cross-entropy loss of the semantic segmentation
predictions.

Parameters
----------
seg_label : TensorBatch
    (N, 1 + D + 1) Tensor of segmentation labels for the batch
segmentation : TensorBatch
    (N, N_c) Tensor of logits from the segmentation model
point_label : TensorBatch, optional
    (P, 1 + D + 1) Tensor of points of interests for the batch. This
    is used to upweight the loss near specific points.
ghost : TensorBatch, optional
    (N, 2) Tensor of ghost logits from the segmentation model
weights : TensorBatch, optional
    (N) Tensor of weights for each pixel in the batch
**kwargs : dict, optional
    Other outputs of the upstream model which are not relevant here

Returns
-------
dict
    Dictionary of accuracies and losses

---
### FunctionDef: `forward`

Computes the kernel edge score of all node pairs in the graph.

Parameters
----------
x1 : torch.Tensor
    (E, N_f) Features of the source nodes
x2 : torch.Tensor
    (E, N_f) Features of the targer nodes

---
### FunctionDef: `forward`

Computes the kernel edge score of all node pairs in the graph.

Parameters
----------
x1 : torch.Tensor
    (E, N_f) Features of the source nodes
x2 : torch.Tensor
    (E, N_f) Features of the targer nodes

---
### FunctionDef: `forward`

Computes the kernel edge score of all node pairs in the graph.

This kernel expectes a set of (3 + 3 + 3 + N_f + 2 + 3 + 1 + 1)
features per node:
- 3 coordinates
- 3 tangent components
- 3 spatial embedding features
- 16 feature embedding features
- 2 covariance features
- 3 coordinate covariance features
- 1 tangent coviarance feature
- 1 occupancy feature

Parameters
----------
x1 : torch.Tensor
    (E, 3 + 3 + 3 + N_f + 2 + 3 + 1 + 1) Features of the source nodes
x2 : torch.Tensor
    (E, 3 + 3 + 3 + N_f + 2 + 3 + 1 + 1) Features of the targer nodes

---
### FunctionDef: `forward`

Computes the kernel edge score of ll node pairs in the graph.

This kernel expectes a set of (3 + N_f + 2 + 1) features per node:
- 3 spatial embedding features
- N_f feature embedding features
- 2 covariance features
- 1 occupancy feature

Parameters
----------
x1 : torch.Tensor
    (E, 3 + N_f + 2 + 1) Features of the source nodes
x2 : torch.Tensor
    (E, 3 + N_f + 2 + 1) Features of the target nodes

---
### FunctionDef: `forward`

Computes the three PPN losses.

Parameters
----------
ppn_label : TensorBatch
    (N, 1 + D + N_l) Tensor of PPN labels for the batch
ppn_points : TensorBatch
    Complete PPN predictions at the last layer
ppn_masks : List[TensorBatch]
    Binary mask at each layer of the PPN
ppn_layers : List[TensorBatch]
    Output logits at each layer of the PPN
ppn_coords : List[TensorBatch]
    Set of coordinates at each layer of the PPN
ppn_output_coords : TensorBatch
    Set of coordinates at the very last layer of the PPN
ppn_classify_endpoins : TensorBatch, optional
    Set of logits associated with end point classification
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels
    - N_c is is the number of cluster labels
**kwargs : dict, optional
    Other outputs of the upstream model which are not relevant here

Returns
-------
dict
    Dictionary of accuracies and losses

---
### FunctionDef: `forward`

Evaluate the IoU score for a batch of label and predictions.

Parameters
----------
y_true : torch.Tensor
    Set of labels
y_pred : torch.Tensor
    Set of predictions

Returns
-------
float
    IoU score

---
### FunctionDef: `forward`

Expand a tensor to the appropriate shape

Parameters
----------
x : torch.Tensor
    (N, 2) Input tensor
shape : ntuple
    (N, X) Shape to expand the mask to
propagate_all : bool, default False
    If `True`, sets all features to 1.
use_binary_mask : bool, default False
    If `True`, sets all features to either 0 or 1
scrore_threshold : float, default 0.5
    If `use_binary_mask == True`, sets the threshold above which
    the feature is 1.0 and below which it is 0.0

---
### FunctionDef: `forward`

Forward function for the Discriminative Loss Module.

Inputs:
    out: output of UResNet; embedding-space coordinates.
    semantic_labels: ground-truth semantic labels
    group_labels: ground-truth instance labels
Returns:
    (dict): A dictionary containing key-value pairs for
    loss, accuracy, etc.

---
### FunctionDef: `forward`

Generate CNN cluster edge features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    Indexes that make up each cluster
edge_index : EdgeIndexBatch
    Incidence map between clusters
**kwargs : dict, optional
    Additional objects no used by this encoder

Returns
-------
TensorBatch
    (E, N_e) Set of N_e features per edge

---
### FunctionDef: `forward`

Generate CNN cluster node features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    Indexes that make up each cluster
**kwargs : dict, optional
    Additional objects no used by this encoder

Returns
-------
TensorBatch
    (C, N_c) Set of N_c features per cluster

---
### FunctionDef: `forward`

Generate CNN global graph features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    Indexes that make up each cluster
**kwargs : dict, optional
    Additional objects no used by this encoder

Returns
-------
TensorBatch
    (B, N_g) Set of N_g globale graph features per batch entry

---
### FunctionDef: `forward`

Generate empty edge features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    Indexes that make up each cluster
edge_index : EdgeIndexBatch
    Incidence map between clusters
**kwargs : dict, optional
    Additional objects no used by this encoder

Returns
-------
TensorBatch
    (E, 0) Empty set of features per edge

---
### FunctionDef: `forward`

Generate empty global graph features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    Indexes that make up each cluster
**kwargs : dict, optional
    Additional objects no used by this encoder

Returns
-------
TensorBatch
    (B, 0) Empty set of features per batch entry

---
### FunctionDef: `forward`

Generate empty node features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    Indexes that make up each cluster
**kwargs : dict, optional
    Additional objects no used by this encoder

Returns
-------
TensorBatch
    (C, 0) Empty set of features per cluster

---
### FunctionDef: `forward`

Generate geometric cluster edge features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    (C) Indexes that make up each cluster
edge_index : EdgeIndexBatch
    Incidence map between clusters
closest_index : Union[np.ndarray, torch.Tensor], optional
    (C, C) : Combined index of the closest pair of voxels per
    pair of clusters
**kwargs : dict, optional
    Additional objects no used by this encoder

Returns
-------
TensorBatch
   (C, N_e) Set of N_e features per edge

---
### FunctionDef: `forward`

Generate geometric cluster node features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    (C) Indexes that make up each cluster
coord_label : TensorBatch
    (P, 1 + D + 8) Label start, end, time and shape for each point
points : TensorBatch
    (C, 6) Set of start/end points for each input cluster
extra : TensorBatch
    (C, 1/2/3) Set of mean/rms values in the cluster and/or shape
**kwargs : dict, optional
    Additional objects no used by this encoder

Returns
-------
TensorBatch
   (C, N_c) Set of N_c features per cluster

---
### FunctionDef: `forward`

Generate mixed cluster edge features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    (C) List of list of indexes that make up each cluster
edge_index : EdgeIndexBatch
    Incidence map between clusters
**kwargs : dict, optional
    Additional objects no used by this encoder

Returns
-------
TensorBatch
    (C, N_e) Set of N_e features per edge

---
### FunctionDef: `forward`

Generate mixed cluster node features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    (C) List of list of indexes that make up each cluster
**kwargs : dict, optional
    Additional objects no used by this encoder

Returns
-------
TensorBatch
    (C, N_c) Set of N_c features per cluster

---
### FunctionDef: `forward`

Inputs
------
    x: Input ME.SparseTensor from UResNet output

---
### FunctionDef: `forward`

Inputs:
    - input (torch.Tensor): N x 6 (coords, edep, semantic_labels)
    - cnn_result: dict of List[torch.Tensor], containing:
        - segmentation
        - embeddings
        - seediness
        - margins

Returns:
    - fragments
    - frag_batch_ids
    - frag_seg

---
### FunctionDef: `forward`

Merge two sparse tensors

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor
other : ME.SparseTensor
    Other sparse tensor to merge

Returns
-------
ME.SparseTensor
    Concatenated sparse tensor

---
### FunctionDef: `forward`

Pass a batch of data through DBSCAN to form space clusters.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Tensor of voxel/value pairs
    - N is the the total number of voxels in the image
    - 1 is the batch ID
    - D is the number of dimensions in the input image
    - N_f is 1 (charge/energy) if the clusters (`clusts`) are provided,
      or it needs to contain cluster labels to build them on the fly
seg_pred : TensorBatch
    (N) Segmentation value for each data point
coord_label : TensorBatch, optional
    Location of the true particle points
**ppn_result : dict, optional
    Dictionary of outputs from the PPN model

---
### FunctionDef: `forward`

Pass a batch of node/edges through the edge update layer.

Parameters
----------
node_feats : torch.Tensor
    (C, N_c) Node features
edge_index : torch.Tensor
    (2, E) Incidence matrix
*args : list, optional
    Other parameters passed but not needed

Returns
-------
torch.Tensor
    (C, N_o) Updated node features

---
### FunctionDef: `forward`

Pass a batch of node/edges through the edge update layer.

Parameters
----------
node_feats : torch.Tensor
    (C, N_c) Node features
edge_index : torch.Tensor
    (2, E) Incidence matrix
*args : list, optional
    Other parameters passed but not needed

Returns
-------
torch.Tensor
    (C, N_o) Updated node features

---
### FunctionDef: `forward`

Pass a batch of node/edges through the edge update layer.

Parameters
----------
node_feats : torch.Tensor
    (C, N_c) Node features
edge_index : torch.Tensor
    (2, E) Incidence matrix
*args : list, optional
    Other parameters passed but not needed

Returns
-------
torch.Tensor
    (C, N_o) Updated node features

---
### FunctionDef: `forward`

Pass a batch of node/edges through the edge update layer.

Parameters
----------
node_feats : torch.Tensor
    (C, N_c) Node features
edge_index : torch.Tensor
    (2, E) Incidence matrix
edge_feats : torch.Tensor
    (E, N_e) Edge features
*args : list, optional
    Other parameters passed but not needed

Returns
-------
torch.Tensor
    (C, N_o) Updated node features

---
### FunctionDef: `forward`

Pass a batch of node/edges through the edge update layer.

Parameters
----------
node_feats : torch.Tensor
    (C, N_c) Node features
edge_index : torch.Tensor
    (2, E) Incidence matrix
edge_feats : torch.Tensor
    (E, N_e) Edge features
glob_feats : torch.Tensor
    (B, N_g) Global features
batch : torch.Tensor
    (C) ID of the entry of each of the nodes within the batch

Returns
-------
torch.Tensor
    (C, N_o') Updated node features

---
### FunctionDef: `forward`

Pass a batch of node/edges through the edge update layer.

Parameters
----------
src_feats : torch.Tensor
    (E, N_c) Source node features
dest_feats : torch.Tensor
    (E, N_c) Sink node features
edge_feats : torch.Tensor
    (E, N_e) Edge features
glob_feats : torch.Tensor
    (B, N_g) Global features
batch : torch.Tensor
    (E) ID of the entry of each of the edges within the batch

Returns
-------
torch.Tensor
    (C, N_o) Updated edge features

---
### FunctionDef: `forward`

Pass a batch of node/edges through the global update layer.

Parameters
----------
node_feats : torch.Tensor
    (C, N_c) Source node features
edge_index : torch.Tensor
    (2, E) Incidence matrix
edge_feats : torch.Tensor
    (E, N_e) Edge features
glob_feats : torch.Tensor
    (B, N_g) Global features
batch : torch.Tensor
    (C) ID of the entry of each of the nodes within the batch

Returns
-------
torch.Tensor
    (B, N_o) Updated global features

---
### FunctionDef: `forward`

Pass a tensor of features through the MLP.

Parameters
----------
x : torch.Tensor
    (N, F) Tensor of features

Paramters
---------
torch.Tensor
    (N, W) Updated tensor of features

---
### FunctionDef: `forward`

Pass a tensor through the ASPP block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the AtrousII block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the Cascaded Atrous Convolution block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the MBConv block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the MBResConv block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the ResNeXt block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the ResNet block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the SE block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the SEResNet block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the SEResNet block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the SPP block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the UResNet backbone.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
encoder_tensors : List[ME.SparseTensor]
    List of intermediate tensors (taken between encoding block and
    convolution) from the encoder half
decoder_tensors : List[ME.SparseTensor]
    List of feature tensors in decoding path at each spatial resolution
final_tensor : ME.SparseTensor
    Feature tensor at deepest layer

---
### FunctionDef: `forward`

Pass a tensor through the convolution block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the decoder.

Parameters
----------
final : ME.SparseTensor
    Output of the encoder
encoder_tensors : List[ME.SparseTensor]
    List of tensors from each depth of the encoder

Returns
-------
List[ME.SparseTensor]
    List of feature tensors in decoding path at each spatial resolution

---
### FunctionDef: `forward`

Pass a tensor through the dropout block.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
ME.SparseTensor
    Output sparse tensor

---
### FunctionDef: `forward`

Pass a tensor through the encoder.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor

Returns
-------
encoder_tensors : List[ME.SparseTensor]
    List of intermediate tensors (taken between encoding block and
    convolution) from the encoder half
final_tensor : ME.SparseTensor
    Feature tensor at deepest layer

---
### FunctionDef: `forward`

Pass one batch of data through the CNN encoder.

Parameters
----------
data : torch.Tensor
     (N, 1 + D + N_f) Batch of data

Returns
-------
torch.Tensor
    (B) Batch of features, one per batch ID

---
### FunctionDef: `forward`

Pass one minibatch of data through the network and the loss.

Load one minibatch of data. pass it through the network forward
function and the loss computation. Store the output.

Parameters
----------
data : dict
    Dictionary of input data product keys which each map to its
    associated batched data product
iteration : int, optional
    Iteration number (relevant for time-dependant losses)

Returns
-------
dict
    Dictionary of model and loss outputs

---
### FunctionDef: `forward`

Pass predictions/labels through the loss function.

Parameters
----------
inputs : torch.Tensor
    (N) Values predicted by the network
targets : torch.Tensor
    (N) Regression targets

Returns
-------
torch.Tensor
    Loss value

---
### FunctionDef: `forward`

Pass predictions/labels through the loss function.

Parameters
----------
inputs : torch.Tensor
    (N) Values predicted by the network
targets : torch.Tensor
    (N) Regression targets

Returns
-------
torch.Tensor
    Loss value or array of loss values (if no reduction)

---
### FunctionDef: `forward`

Pass predictions/labels through the loss function.

Parameters
----------
inputs : torch.Tensor
    (N) Values predicted by the network
targets : torch.Tensor
    (N) Regression targets

Returns
-------
torch.Tensor
    Loss value or array of loss values (if no reduction)

---
### FunctionDef: `forward`

Pass predictions/labels through the loss function.

Parameters
----------
logits : torch.Tensor
    (N) Values predicted by the network
targets : torch.Tensor
    (N) Regression targets

Returns
-------
torch.Tensor
    Loss value

---
### FunctionDef: `forward`

Pass predictions/labels through the loss function.

Parameters
----------
logits : torch.Tensor
    (N) Values predicted by the network
targets : torch.Tensor
    (N) Regression targets

Returns
-------
torch.Tensor
    Loss value

---
### FunctionDef: `forward`

Pass predictions/labels through the loss function.

Parameters
----------
logits : torch.Tensor
    (N) Values predicted by the network
targets : torch.Tensor
    (N) Regression targets

Returns
-------
torch.Tensor
    Loss value

---
### FunctionDef: `forward`

Pass predictions/labels through the loss function.

Parameters
----------
logits : torch.Tensor
    (N) Values predicted by the network
targets : torch.Tensor
    (N) Regression targets

Returns
-------
torch.Tensor
    Loss value

---
### FunctionDef: `forward`

Pass predictions/labels through the loss function.

Parameters
----------
logits : torch.Tensor
    (N) Values predicted by the network
targets : torch.Tensor
    (N) Regression targets

Returns
-------
torch.Tensor
    Loss value

---
### FunctionDef: `forward`

Pass tensor through the layer.

Parameters
----------
input_data : ME.SparseTensor
    Sparse input tensor

Return
------
ME.SparseTensor
    Sparse output tensor

---
### FunctionDef: `forward`

Pass tensor through the layer.

Parameters
----------
input_data : ME.SparseTensor
    Sparse input tensor

Return
------
ME.SparseTensor
    Sparse output tensor

---
### FunctionDef: `forward`

Pass tensor through the layer.

Parameters
----------
input_data : ME.SparseTensor
    Sparse input tensor

Return
------
ME.SparseTensor
    Sparse output tensor

---
### FunctionDef: `forward`

Passes a set of features through the evidential model.

Parameters
----------
input_feats : torch.Tesnor
    (N, F) Tensor of input features

Results
-------
torch.Tensor
    (N, F) Tensor of evidence

---
### FunctionDef: `forward`

Passes a set of features through the final linear layer.

Parameters
----------
input_feats : TensorBatch
    (N, F) Batched tensor of input features

Results
-------
TensorBatch
    (N, F) Batched tensor of logits

---
### FunctionDef: `forward`

Passes a set of features through the final linear layer.

Parameters
----------
input_feats : TensorBatch
    (N, F) Batched tensor of input features

Results
-------
TensorBatch
    (N, F) Batched tensor of logits

---
### FunctionDef: `forward`

Passes a set of features through the final linear layer.

Parameters
----------
input_feats : TensorBatch
    (N, F) Batched tensor of input features

Results
-------
TensorBatch
    (N, F) Batched tensor of logits

---
### FunctionDef: `forward`

Prepares particle clusters and feed them to the GNN model.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Tensor of voxel/value pairs
    - N is the the total number of voxels in the image
    - 1 is the batch ID
    - D is the number of dimensions in the input image
    - N_f is 1 (charge/energy) if the clusters (`clusts`) are provided,
      or it needs to contain cluster labels to build them on the fly
coord_label : TensorBatch, optional
    (P, 1 + 2*D + 2) Tensor of label points (start/end/time/shape)
clusts : IndexBatch, optional
    (C) List of indexes corresponding to each cluster
shapes : TensorBatch, optional
    (C) List of cluster semantic class used to define the max length
groups : TensorBatch, optional
    (C) List of node groups, one per cluster. If specified, will
        remove connections between nodes of a separate group.
points : TensorBatch, optional
    (C, 3/6) Tensor of start (and end) points
extra : TensorBatch, optional
    (C, N_f) Batch of features to append to the existing node features

Returns
-------
clusts : IndexBatch
    (C, N_c, N_{c,i}) Cluster indexes
edge_index : TensorBatch
    (E, 2) Incidence matrix
node_features : TensorBatch
    (C, N_c,f) Node features
edge_features : TensorBatch
    (C, N_e,f) Node features
global_features : TensorBatch
    (C, N_g,f) Global features
node_pred : TensorBatch
    (C, N_n) Node predictions (logits)
edge_pred : TensorBatch
    (C, N_e) Edge predictions (logits)
global_pred : TensorBatch
    (C, N_e) Global predictions (logits)

---
### FunctionDef: `forward`

Prune the input data.

Parameters
----------
x : ME.SparseTensor
    Input sparse tensor
mask : ME.SparseTensor
    Mask to apply

---
### FunctionDef: `forward`

Run a batch of data through the forward function.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
    - N is the the total number of voxels in the image
    - 1 is the batch ID
    - D is the number of dimensions in the input image
    - N_f is the number of features per voxel

---
### FunctionDef: `forward`

Run a batch of data through the forward function.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
    - N is the the total number of voxels in the image
    - 1 is the batch ID
    - D is the number of dimensions in the input image
    - N_f is the number of features per voxel

Returns
-------
dict
    Dictionary of outputs

---
### FunctionDef: `forward`

Run a batch of data through the forward function.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
    - N is the the total number of voxels in the image
    - 1 is the batch ID
    - D is the number of dimensions in the input image
    - N_f is the number of features per voxel
seg_label : TensorBatch
    (N, 1 + D + 1) Tensor of segmentation labels
    - 1 is the segmentation label
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels
    - N_c is is the number of cluster labels

Returns
-------
dict
    Dictionary of outputs

---
### FunctionDef: `forward`

Run a batch of data through the foward function.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
    - N is the the total number of voxels in the image
    - 1 is the batch ID
    - D is the number of dimensions in the input image
    - N_f is the number of features per voxel
seg_label : TensorBatch, optional
    (N, 1 + D + 1) tensor of voxel/ghost label pairs

---
### FunctionDef: `forward`

Run a batch of data through the full chain.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
    - N is the the total number of voxels in the image
    - 1 is the batch ID
    - D is the number of dimensions in the input image
    - N_f is the number of features per voxel
sources : TensorBatch, optional
    (N, 2) tensor of module/tpc pair for each voxel
seg_label : TensorBatch, optional
    (N, 1 + D + 1) Tensor of segmentation labels
    - 1 is the segmentation label
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels
    - N_c is is the number of cluster labels
coord_label : TensorBatch, optional
    (N, 1 + D + N_p) Tensor of point of interest labels
    - N_p is the number point labels
energy_label : TensorBatch, optional
    (N, 1 + D + 1) Tensor of true energy deposition values
    - 1 is the energy deposition value in each voxel
meta : Meta, optional
    Image metadata information
run_info : List[RunInfo], optional
    Object containing information about the run, subrun and event

Returns
-------
TODO

---
### FunctionDef: `forward`

Run a batch of data through the loss function.

Parameters
----------
seg_label : TensorBatch
    (N, 1 + D + 1) Tensor of segmentation labels
    - 1 is the segmentation label
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labelresul
    - N_c is is the number of cluster labels
filter_index : IndexBatch
    (M) Index to narrow down the original tensor
**output : dict
    Output of the Graph-SPICE model

Returns
-------
dict
    Dictionary of outputs

---
### FunctionDef: `forward`

Run a batch of data through the loss function.

Parameters
----------
seg_label : TensorBatch
    (N, 1 + D + 1) Tensor of segmentation labels for the batch
ppn_label : TensorBatch
    (N, 1 + D + N_l) Tensor of PPN labels for the batch
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels
    - N_c is is the number of cluster labels
weights : torch.Tensor, optional
    (N) Tensor of segmentation weights for each pixel in the batch
**result : dict
    Outputs of the UResNet + PPN forward function

Returns
-------
TODO

---
### FunctionDef: `forward`

Run the full chain output through the full chain loss.

Parameters
----------
seg_label : TensorBatch, optional
    (N, 1 + D + 1) Tensor of segmentation labels
    - 1 is the segmentation label
ppn_label : TensorBatch, optional
    (N, 1 + D + N_l) Tensor of PPN labels
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels
    - N_c is is the number of cluster labels
clust_label_adapt : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels adapted to seg predictions
    - N_c is is the number of cluster labels
coord_label : TensorBatch, optional
    (P, 1 + D + 8) Tensor of start/end point labels for each
    true particle in the image
graph_label : EdgeIndexTensor, optional
    (2, E) Tensor of edges that correspond to physical
    connections between true particle in the image
meta : Meta, optional
    Image metadata information
ghost : TensorBatch, optional
    (N, 2) Tensor of logits from the deghosting model
ghost_pred : TensorBatch, optional
    (N,) Tensor of ghost predictions
segmentation : TensorBatch, optional
    (N, N_c) Tensor of logits from the segmentation model
seg_pred : TensorBatch, optional
    (N) Semantic prediction for each point
**output : dict, optional
    Additional outputs of the reconstruction chain

---
### FunctionDef: `forward`

Run the message passing steps on one batch of data.

Parameters
----------
node_feats : TensorBatch
    (C) Batch of node features
edge_index : torch.Tensor
    (2, E) Incidence matrix
edge_feats : TensorBatch
    (E) Edge features
glob_feats : TensorBatch
    (B) Global features
batch : torch.Tensor
    (B) Batch ID of each node in the batched graph

---
### FunctionDef: `forward`

Vanilla UResNet Decoder
INPUTS:
    - encoderTensors (list of SparseTensor): output of encoder.
RETURNS:
    - decoderTensors (list of SparseTensor):
    list of feature tensors in decoding path at each spatial resolution.

---
### FunctionDef: `forward`

queries: B, num_queries, d_model

---
### FunctionDef: `forward`

segmentation[0], label and weight are lists of size #gpus = batch_size.
segmentation has as many elements as UResNet returns.
label[0] has shape (N, dim + batch_id + 1)
where N is #pts across minibatch_size events.

---
### ClassDef: `FPN`

Feature Pyramid Network (FPN).

FPNs are a different implementation of the concept behind unets.

Configurations
--------------
depth : int
    Depth of FPN, also corresponds to how many times we down/upsample.
num_filters : int
    Number of filters in the first convolution of FPN.
    Will increase linearly with depth.
reps : int, optional
    Convolution block repetition factor
kernel_size : int, optional
    Kernel size for the SC (sparse convolutions for down/upsample).
input_kernel : int, optional
    Receptive field size for very first convolution after input layer.

---
### ClassDef: `FragmentBase`

Base fragment-specific information.

Attributes
----------
particle_id : int
    Index of the particle this fragment belongs to
interaction_id : int
    Index of the interaction this fragment belongs to
shape : int
    Semantic type (shower (0), track (1), Michel (2), delta (3),
    low energy scatter (4)) of this particle
is_primary : bool
    Whether this fragment was the first in the particle group
length : float
    Length of the particle (only assigned to track objects)
start_point : np.ndarray
    (3) Fragment start point
end_point : np.ndarray
    (3) Fragment end point (only assigned to track objects)
start_dir : np.ndarray
    (3) Fragment direction w.r.t. the start point
end_dir : np.ndarray
    (3) Fragment direction w.r.t. the end point (only assigned
    to track objects)

---
### ClassDef: `FragmentBuilder`

Builds reconstructed and truth fragments.

It takes the raw output of the reconstruction chain, extracts the
necessary information and builds :class:`RecoFragment` and
:class:`TruthFragment` objects from it.

---
### FunctionDef: `freeze_weights`

Freeze the weights of certain model components.

Breadth-first search for `freeze_weights` parameters in the model
configuration. If `freeze_weights` is `True` under a module block,
`requires_grad` is set to `False` for its parameters. The batch
normalization and dropout layers are set to evaluation mode.

---
### FunctionDef: `from_larcv`

Builds and returns a CRTHit object from a LArCV CRTHit object.

Parameters
----------
crthit : larcv.CRTHit
    LArCV-format CRT hit

Returns
-------
CRTHit
    CRT hit object

---
### FunctionDef: `from_larcv`

Builds and returns a Flash object from a LArCV Flash object.

Parameters
----------
flash : larcv.Flash
    LArCV-format optical flash

Returns
-------
Flash
    Flash object

---
### FunctionDef: `from_larcv`

Builds and returns a Meta object from a LArCV 2D metadata object

Parameters
----------
larcv_event : larcv.EventBase
     LArCV event object which contains the run information as attributes

Returns
-------
Meta
    Metadata object

---
### FunctionDef: `from_larcv`

Builds and returns a Meta object from a LArCV 2D metadata object.

Parameters
----------
meta : Union[larcv.ImageMeta, larcv.Voxel3DMeta]
    LArCV-format 2D metadata

Returns
-------
Meta
    Metadata object

---
### FunctionDef: `from_larcv`

Builds and returns a Neutrino object from a LArCV Neutrino object.

Parameters
----------
neutrino : larcv.Neutrino
    LArCV-format neutrino object

Returns
-------
Neutrino
    Neutrino object

---
### FunctionDef: `from_larcv`

Builds and returns a Particle object from a LArCV Particle object.

Parameters
----------
particle : larcv.Particle
    LArCV-format particle object

Returns
-------
Particle
    Particle object

---
### FunctionDef: `from_larcv`

Builds and returns a Trigger object from a LArCV Trigger object.

Parameters
----------
trigger : larcv.Trigger
    LArCV-format trigger information

Returns
-------
Trigger
    Trigger object

---
### FunctionDef: `from_list`

Builds a batch from a list of tensors.

Parameters
----------
data_list : List[Union[np.ndarray, torch.Tensor]]
    List of tensors, exactly one per batch

---
### FunctionDef: `from_particles`

Builds an Interaction instance from its constituent Particle objects.

Parameters
----------
particles : List[ParticleBase]
    List of Particle objects that make up the Interaction

Returns
-------
InteractionBase
    Interaction built from the particle list

---
### FunctionDef: `full_batch_ids`

Returns the batch ID of each element in the full index list.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (N) Complete batch ID array, one per element

---
### FunctionDef: `full_counts`

Returns the total number of elements in each batch entry.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (B) Number of elements in each batch entry

---
### FunctionDef: `full_index`

Returns the index combining all sub-indexes, if relevant.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (N) Complete concatenated index

---
### ClassDef: `FullChain`

Full reconstruction in all its glory.

Modular, end-to-end particle imaging detector reconstruction chain:
- Deghosting for 3D tomographic reconstruction artifiact removal
- Voxel-wise semantic segmentation
- Point proposal
- Particle clustering
- Shower primary identification
- Interaction clustering
- Particle type classification
- Primary identification
- Track orientation

Typical configuration can look like this:

.. code-block:: yaml

    model:
      name: grappa
      modules:
        chain:
           <dictionary of arguments to specify chain-wide configuration>
        uresnet_deghost:
           name: <name of the model used to deghost
           <dictionary of arguments to specify the deghosting module>
        uresnet_segmentation:
           name: <name of the model used to do segmentation>
           <dictionary of arguments to specify the segmentation module>
        dbscan:
           TODO
        graph_spice:
           name: <name of the model used to do segmentation>
           <dictionary of arguments to specify the segmentation module>
        grappa_shower:
           name: <name of the model used to do segmentation>
           <dictionary of arguments to specify the segmentation module>
        grappa_track:
           name: <name of the model used to do segmentation>
           <dictionary of arguments to specify the segmentation module>
        grappa_inter:
          TODO
        calibration:
          TODO

See configuration file(s) prefixed with `full_chain_` under the `config`
directory for detailed examples of working configurations.

The `chain` section enables or disables specific stages of the full
chain. When a module is disabled through this section, it will not be
constructed. The configuration blocks for each enabled module should
also live under the `modules` section of the configuration.

---
### ClassDef: `FullChainLoss`

Loss function for the full chain.

See Also
--------
FullChain

---
### ClassDef: `GainCalibrator`

Converts all charge depositions in ADC to a number of electrons. It can
either use a flat converstion factor or one per TPC in the detector

---
### ClassDef: `GATConvNodeLayer`

GATConv module for extracting graph node features.

This model simply takes a simple attention-based convolution of a node
with all of its neighbors to update the initial node feature vector (N_c),
returning an updated (N_o) vector.

Source: https://arxiv.org/abs/1710.10903

---
### FunctionDef: `generate`

Generate a loop-graph on a set of N nodes.

Parameters
----------
clusts : IndexBatch
    (C) Cluster indexes
**kwargs : dict, optional
    Unused graph generation arguments

Returns
-------
np.ndarray
    (2, E) Tensor of edges
np.ndarray
    (B) Number of edges in each entry of the batch

---
### FunctionDef: `generate`

Generates a complete graph on a set of batched nodes.

Parameters
----------
clusts : IndexBatch
    (C) Cluster indexes
**kwargs : dict, optional
    Unused graph generation arguments

Returns
-------
np.ndarray
    (2, E) Tensor of edges
np.ndarray
    (B) Number of edges in each entry of the batch

---
### FunctionDef: `generate`

Generates an incidence matrix that connects nodes
that share an edge in their corresponding Euclidean Delaunay graph.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Tensor of voxel/value pairs
clusts : IndexBatch
    (C) Cluster indexes
**kwargs : dict, optional
    Unused graph generation arguments

Returns
-------
np.ndarray
    (2, E) Tensor of edges

---
### FunctionDef: `generate`

Generates an incidence matrix that connects nodes that share an
edge in their corresponding Euclidean MST graph.

Parameters
----------
clusts : IndexBatch
    (C) Cluster indexes
dist_mat : Union[np.ndarray, torch.Tensor]
    (C, C) Matrix of pair-wise distances between clusters in the batch
**kwargs : dict, optional
    Unused graph generation arguments

Returns
-------
np.ndarray
    (2, E) Tensor of edges

---
### FunctionDef: `generate`

Generates an incidence matrix that connects nodes that share an
edge in their corresponding kNN graph.

Parameters
----------
clusts : IndexBatch
    (C) Cluster indexes
dist_mat : Union[np.ndarray, torch.Tensor]
    (C, C) Matrix of pair-wise distances between clusters in the batch
**kwargs : dict, optional
    Unused graph generation arguments

Returns
-------
np.ndarray
    (2, E) Tensor of edges

---
### FunctionDef: `generate`

Generates an incidence matrix that connects nodes that share an
edge in their corresponding kNN graph.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Tensor of voxel/value pairs
clusts : IndexBatch
    (C) Cluster indexes
**kwargs : dict, optional
    Unused graph generation arguments

Returns
-------
np.ndarray
    (2, E) Tensor of edges

---
### FunctionDef: `generate`

This function must be overridden in the constructor definition.

---
### FunctionDef: `generate_data`

Generates dummy data for the network and loss input to be used in tests.

Arguments
---------
N: int
    Spatial size
input_schema: list
    Description of input data
num_voxels_low: int, optional
    Lower boundary for generating (random) number of voxels.
num_voxels_high: int, optional
    Upper boundary for generating (random) number of voxels.
voxels: np.array, optional
    Allows to reuse the same voxels across different calls to generate_data
    specifically between network forward and loss forward.
loss: bool, optional
    If this input is going to be used for the loss forward, wrap it a bit
    differently (because of DataParallel) than for network forward.

---
### FunctionDef: `generate_matches`

Generate pairs for a srt of sources and targets.

Parameters
----------
source_objs : List[object]
    (N) List of source objects
target_objs : List[object]
    (M) List of truth objects
ovl_matrix : np.ndarray
    (N, M) Matrix of overlap values
ovl_valid : np.ndarray
    (N, M) Matrix of overlap validity

Returns
-------
pairs : List[tuple]
    (N) List of (source, target) matched pairs (best match only)
overlaps : List[float]
    (N) List of overlap between each source and the best matched target

---
### FunctionDef: `generate_meta2d`

Generates random 3D metadata information.

Parameters
----------
shape : int
    Number of voxels in each dimension
projection : int
    Projection ID

Returns
-------
larcv.ImageMeta
    2D sparse tensor metadata information

---
### FunctionDef: `generate_meta3d`

Generates random 3D metadata information.

Parameters
----------
shape : int
    Number of voxels in each dimension

Returns
-------
larcv.Voxel3DMeta
    3D sparse tensor metadata information

---
### FunctionDef: `generate_neutrino`

Generates a dummy larcv neutrino.

Parameters
----------
idx : int
    Index of the neutrino in the list

Returns
-------
larcv.Neutrino
    Single neutrino truth object

---
### FunctionDef: `generate_object_list`

Generates a dummy list of lists of objects of the request class.

Parameters
----------
cls : object
    Class that the objects should belong to
sizes : List[int]
    Number of objects in each list

Returns
-------
List[ObjectList[obj]]
    List of typed lists of objects

---
### FunctionDef: `generate_offset`

Generate an offset to apply to all the voxel index sets.

This offset is such that the the voxels will be randomly shifted
within the target bounding box.

Parameters
----------
meta : Meta
    Metadata of the original image

Returns
-------
np.ndarray
    Value by which to shift the pixels by

---
### FunctionDef: `generate_particle`

Generates a dummy larcv particle.

Parameters
----------
idx : int
    Index of the particle in the list

Returns
-------
larcv.Particle
    Single particle truth object

---
### FunctionDef: `generate_sparse2d_event`

Generates a dummy 2D larcv tensor.

Parameters
----------
meta : larcv.ImageMeta
    2D sparse tensor metadata information
num_voxels : int, default 10
    Number of voxels in the image

Returns
-------
larcv.EventSparseTensor2D
    Event containing one 2D larcv sparse tensor

---
### FunctionDef: `generate_sparse3d_event`

Generates a dummy 3D larcv tensor.

Parameters
----------
meta : larcv.Voxel3DMeta
    3D sparse tensor metadata information
num_voxels : int, default 10
    Number of voxels in the image
segmentation : bool, default False
    If `True`, generate features that are segmentation-like
ghost : bool, default True
    If `True`, include ghosts in the segmentation labels

Returns
-------
larcv.EventSparseTensor3D
    Event containing one 3D larcv sparse tensor

---
### ClassDef: `GeoDrawer`

Handles drawing all things related to the detector geometry.

This class is loads a :class:`Geometry` object once from a geometry file
and uses it to represent all things related to the detector geometry:
- TPC boundaries
- Optical detectors
- CRT detectors

---
### ClassDef: `Geometry`

Handles all geometry functions for a collection of box-shaped TPCs with
a arbitrary set of optical detectors organized in optical volumes and CRT
planes.

Attributes
----------
tpc : TPCDetector
    TPC detector properties
optical : OptDetector, optional
    Optical detector properties
crt : CRTDetector, optional
    CRT detector properties

---
### FunctionDef: `get`

Draw the requested object type with the requested mode.

Parameters
----------
obj_type : str
    Name of the object type to draw (one of 'fragment', 'particle' or
    'interaction'
attr : Union[str, List[str]], optional
    Name of list of names of attributes to draw
color_attr : str, optional
    Name of the attribute to use to determine the color
draw_raw : bool, default False
    If `True`, add a trace which corresponds to the raw depositions
draw_end_points : bool, default False
    If `True`, draw the fragment or particle end points
draw_vertices : bool, default False
    If `True`, draw the interaction vertices
draw_flashes : bool, default False
    If `True`, draw flashes that have been matched to interactions
synchronize : bool, default False
    If `True`, matches the camera position/angle of one plot to the other
titles : List[str], optional
    Titles of the two scenes (only relevant for split_scene True
split_traces : bool, default False
    If `True`, one trace is produced for each object
matched_flash_only : bool, default True
    If `True`, only flashes matched to interactions are drawn

Returns
-------
go.Figure
    Figure containing all the necessary information to draw

---
### FunctionDef: `get`

Placeholder to be defined by the daughter class.

---
### FunctionDef: `get`

Returns a specific entry in the file.

Parameters
----------
idx : int
    Integer entry ID to access

Returns
-------
data : dict
    Ditionary of data products corresponding to one event

---
### FunctionDef: `get`

Returns a specific entry in the file.

Parameters
----------
idx : int
    Integer entry ID to access

Returns
-------
dict
    Dictionary which maps each data product key to an entry in the tree

---
### FunctionDef: `get_base_dict`

Builds the entry information dictionary.

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
dict
    Dictionary of information for this entry

---
### FunctionDef: `get_base_features`

Generate base geometric cluster node features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    (C) Indexes that make up each cluster
add_value : bool, default False
    Add mean and RMS value of pixels in the cluster
add_shape : bool, default False
    Add the particle semantic type

---
### FunctionDef: `get_base_features`

Generate base geometric cluster node features for one batch of data.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) Batch of sparse tensors
clusts : IndexBatch
    (C) Indexes that make up each cluster
edge_index : EdgeIndexBatch
    Incidence map between clusters
closest_index : Union[np.ndarray, torch.Tensor], optional
    (C, C) : Combined index of the closest pair of voxels per
    pair of clusters

---
### FunctionDef: `get_cathode_offsets`

Find the distance one must shift a particle points by to make
both TPC contributions align at the cathode.

Parameters
----------
particle : Union[Particle, TruthParticle]
    Particle object
module : int
    Module ID
tpcs : List[int]
    List of TPC IDs

Returns
-------
np.ndarray
    Offsets to apply to the each TPC contributions
float
    General offset for this particle (proxy of out-of-time displacement)

---
### FunctionDef: `get_class_weights`

Computes class-wise weights based on their relative abundance.

Parameters
----------
labels : Union[np.ndarray, torch.Tensor]
    (N) Array of class values to base the weighting scheme on
num_classes : int
    Total number of classes (needed if there are some missing)
mode : str, default const
    Weigthing mode (one of 'const', 'log', 'sqrt'
per_class : bool, default True
    If `True`, returns one valuer per class. Otherwise, this function
    returns one value per input in the `classes` array

---
### FunctionDef: `get_closest_module`

For each point, find the ID of the closest module.

There is a natural assumption that all modules are boxes of identical
sizes, so that the relative proximitity of a point to a module is
equivalent to its proximity to the module center.

Parameters
----------
points : np.ndarray
    (N, 3) Set of point coordinates

Returns
-------
np.ndarray
    (N) List of module indexes, one per input point

---
### FunctionDef: `get_closest_module_indexes`

For each module, get the list of points that live closer to it
than any other module in the detector.

Parameters
----------
points : np.ndarray
    (N, 3) Set of point coordinates

Returns
-------
List[np.ndarray]
    List of index of points that belong to each module

---
### FunctionDef: `get_closest_path_labels`

Produce instance clusters using the closest-path method

Parameters
----------
voxels : np.ndarray
    (N, 3) Set of voxel coordinates
points : np.ndarray
    (P, 3) Set of particle end points

Returns
-------
np.ndarray
    (N) Array of cluster assignments for each voxel in the input

---
### FunctionDef: `get_closest_tpc`

For each point, find the ID of the closest TPC.

There is a natural assumption that all TPCs are boxes of identical
sizes, so that the relative proximitity of a point to a TPC is
equivalent to its proximity to the TPC center.

Parameters
----------
points : np.ndarray
    (N, 3) Set of point coordinates

Returns
-------
np.ndarray
    (N) List of TPC indexes, one per input point

---
### FunctionDef: `get_closest_tpc_indexes`

For each TPC, get the list of points that live closer to it than any
other TPC in the detector.

Parameters
----------
points : np.ndarray
    (N, 3) Set of point coordinates

Returns
-------
List[np.ndarray]
    List of index of points that belong to each TPC

---
### FunctionDef: `get_cluster_centers`

Returns the coordinate of the centroid associated with each cluster.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
clusts : List[np.ndarray]
    (C) List of cluster indexes

Returns
-------
np.ndarray
    (C, 3) Tensor of cluster centers

---
### FunctionDef: `get_cluster_closest_label`

Sets the label of clusters based on their proximity to the start point
of the particle which created them.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
coord_label : np.ndarray
    Coordinate labels associated with each particle
clusts : List[np.ndarray]
    (C) List of cluster indexes
labels : np.ndarray
    (C) Existing list of cluster labels (the new labels will be a subset)
default : np.ndarray
    Default label to assign to secondary clusters

Returns
-------
np.ndarray
    (C) List of cluster labels

---
### FunctionDef: `get_cluster_closest_label_batch`

Batched version of :func:`get_cluster_closest_label`.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
coord_label : TensorBatch
    Batch of particle end points labels
clusts : IndexBatch
    (C) List of cluster indexes
labels : TensorBatch
    (C) Existing list of cluster labels (the new labels will be a subset)
default : Union[int, List[int]]
    Default value to assign to secondary clusters

Returns
-------
TensorBatch
    (C) List of individual cluster labels

---
### FunctionDef: `get_cluster_closest_primary_label`

Sets the primary label of clusters based on their proximity to the start
point of the particle which created them.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
coord_label : np.ndarray
    Coordinate labels associated with each particle
clusts : List[np.ndarray]
    (C) List of cluster indexes
primary_ids : np.ndarray
    (C) Existing list of primary IDs (the new labels will be a subset)

Returns
-------
np.ndarray
    (C) List of cluster primary labels

---
### FunctionDef: `get_cluster_closest_primary_label_batch`

Batched version of :func:`get_cluster_cloest_primary_label`.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
coord_label : TensorBatch
    Batch of particle end points labels
clusts : IndexBatch
    (C) List of cluster indexes
primary_ids : TensorBatch
    (C) Existing list of primary IDs (the new labels will be a subset)

Returns
-------
TensorBatch
    (C) List of cluster primary labels

---
### FunctionDef: `get_cluster_dedxs`

Computes the initial local dE/dxs of each cluster.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
starts : np.ndarray
    (C, 3) Start points w.r.t. which to estimate the local dE/dxs
clusts : List[np.ndarray]
    (C) List of cluster indexes
max_dist : float, default -1
    Neighborhood radius around the point used to compute the dE/dx

Returns
-------
np.ndarray
    (C) Local dE/dx values for each cluster

---
### FunctionDef: `get_cluster_dedxs_batch`

Batched version of :func:`get_cluster_dedxs`.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
starts : TensorBatch
    (C, 3) Start points w.r.t. which to estimate the direction
clusts : IndexBatch
    (C) List of cluster indexes
max_dist : float, default -1
    Neighborhood radius around the point used t compute the dE/dx

Returns
-------
TensorBatch
    (C) List of cluster dE/dx value close to the start points

---
### FunctionDef: `get_cluster_directions`

Estimates the direction of each cluster.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
starts : np.ndarray
    (C, 3) Start points w.r.t. which to estimate the direction
clusts : List[np.ndarray]
    (C) List of cluster indexes
max_dist : float, default -1
    Neighborhood radius around the point used to estimate the direction
optimize : bool, default False
    If `True`, the neighborhood radius is optimized on the fly for
    each cluster.

Returns
-------
torch.tensor:
    (C, 3) Direction vector of each cluster

---
### FunctionDef: `get_cluster_directions_batch`

Batched version of :func:`get_cluster_directions`.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
starts : TensorBatch
    (C, 3) Start points w.r.t. which to estimate the direction
clusts : IndexBatch
    (C) List of cluster indexes
max_dist : float, default -1
    Neighborhood radius around the point used to estimate the direction
optimize : bool, default False
    If `True`, the neighborhood radius is optimized on the fly for
    each cluster.

Returns
-------
TensorBatch
    (C, 3) List of cluster directions

---
### FunctionDef: `get_cluster_edge_features`

Returns a tensor of edge features for each edge connecting 
point clusters in the graph.

The edge features (N_e = 19) include (in that order):
- Coordinates of the voxel in the first cluster closest to the second (3)
- Coordinates of the voxel in the second cluster closest to the first (3)
- Displacement vector between the aforementioned voxels (3)
- Magnitude of the displacement vector (1)
- Outer product of the displacement vector (9)

Parameters
----------
data : Union[np.ndarray, torch.Tensor]
    (N, 1 + D + N_f) Batched sparse tensors
clusts : List[np.ndarray]
    (C) List of arrays of voxels IDs in each cluster
edge_index : Union[np.ndarray, torch.Tensor]
    (2, E) Incidence map between voxels
closest_index : Union[np.ndarray, torch.Tensor], optional
    (C, C) : Combined index of the closest pair of voxels per edge
algorithm : str, default 'brute'
    Method used to compute the inter-cluster distance

Returns
-------
np.ndarray
    (E, N_e) Tensor of edge features

---
### FunctionDef: `get_cluster_edge_features_batch`

Batched version of :func:`get_cluster_edge_features`.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
clusts : IndexBatch
    (C) List of cluster indexes
edge_index : EdgeIndexBatch
    (2, E) Sparse incidence matrix
closest_index : Union[np.ndarray, torch.Tensor], optional
    (C, C) : Combined index of the closest pair of voxels per edge
algorithm : str, default 'brute'
    Method used to compute the inter-cluster distance

Returns
-------
TensorBatch
    (E, N_e) List of edge features between clusters

---
### FunctionDef: `get_cluster_energies`

Returns the total charge/energy deposited by each cluster.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
clusts : List[np.ndarray]
    (C) List of cluster indexes

Returns
-------
np.ndarray
    (C) List of cluster pixel sums

---
### FunctionDef: `get_cluster_features`

Returns an array of features for each cluster.

The basic 16 geometric features are composed of:
- Center (3)
- Covariance matrix (9)
- Principal axis (3)
- Voxel count (1)

The flag `add_value` adds the following 2 features:
- Mean energy (1)
- RMS energy (1)

The flag `add_shape` adds the particle shape information:
- Semantic type (1), i.e. most represented type in cluster

Parameters
----------
data : np.ndarray
    Cluster label data tensor
clusts : List[np.ndarray]
    (C) List of cluster indexes

Returns
-------
np.ndarray
    (C, N_c) Tensor of cluster features

---
### FunctionDef: `get_cluster_features_base`

Returns an array of 16 geometric features for each of cluster.

The 16 geometric features are composed of:
- Center (3)
- Covariance matrix (9)
- Principal axis (3)
- Voxel count (1)

Parameters
----------
data : np.ndarray
    Cluster label data tensor
clusts : List[np.ndarray]
    (C) List of cluster indexes

Returns
-------
np.ndarray
    (C, 16) Tensor of cluster features

---
### FunctionDef: `get_cluster_features_batch`

Batched version of :func:`get_cluster_features`.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
starts : TensorBatch
    (C, 3) Start points w.r.t. which to estimate the direction
clusts : IndexBatch
    (C) List of cluster indexes
max_dist : float, default -1
    Neighborhood radius around the point used t compute the dE/dx

Returns
-------
TensorBatch
    (C) List of cluster dE/dx value close to the start points

---
### FunctionDef: `get_cluster_features_extended`

Returns an array of 3 additional features for each of cluster.

The flag `add_value` adds the following 2 features:
- Mean energy (1)
- RMS energy (1)

The flag `add_shape` adds the particle shape information:
- Semantic type (1), i.e. most represented type in cluster

Parameters
----------
data : np.ndarray
    Cluster label data tensor
clusts : List[np.ndarray]
    (C) List of cluster indexes
add_value : bool, default True
    Whether to add the mean and std of the pixel values
add_shape : bool, default True
    Whether to add the shape of the cluster

Returns
-------
np.ndarray
    (C, 1/2/3) Tensor of additional cluster features

---
### FunctionDef: `get_cluster_label`

Returns the majority label of each cluster, specified by the
requested data column of the label tensor.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
clusts : List[np.ndarray]
    (C) List of cluster indexes
column : int, default CLUST_COL
    Column in the label tensor which specifies the requested label

Returns
-------
np.ndarray
    (C) List of individual cluster labels

---
### FunctionDef: `get_cluster_label_batch`

Batched version of :func:`get_cluster_label`.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
clusts : IndexBatch
    (C) List of cluster indexes
column : int, default CLUST_COL
    Column in the label tensor which specifies the requested label

Returns
-------
TensorBatch
    (C) List of individual cluster labels

---
### FunctionDef: `get_cluster_points_label`

Gets label points for each cluster.

Returns start point of primary shower fragment twice if shower, delta or
Michel and both end points of tracks if track.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
coord_label : np.ndarray
    (P, 9) Particle end points labels
    [batch_id, start_x, start_y, start_z, end_x, end_y, end_z, time, shape]
clusts : List[np.ndarray]
    (C) List of cluster indexes
random_order : bool, default True
    If `True`, randomize the order in which the start en end points of
    a track are stored in the output

Returns
-------
np.ndarray
    (C, 6) Cluster start and end points (in random order if requested)

---
### FunctionDef: `get_cluster_points_label_batch`

Batched version of :func:`get_cluster_points_label`

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
coord_label : TensorBatch
    Batch of particle end points labels
clusts : IndexBatch
    (C) List of cluster indexes
random_order : bool, default True
    If `True`, randomize the order in which the start en end points of
    a track are stored in the output

Returns
-------
np.ndarray
    (C, 6) Cluster-wise start and end points (in random order if requested)

---
### FunctionDef: `get_cluster_primary_label`

Returns the majority label of the primary cluster of the group each
cluster belongs to, specified in the requested data column of the label
tensor.

The primary component is identified by picking the set of label voxels
that have a `PART_COL` identical to the cluster `GROUP_COL`.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
clusts : List[np.ndarray]
    (C) List of cluster indexes
column : int
    Column in the label tensor which specifies the requested label

Returns
-------
np.ndarray
    (C) List of cluster primary labels

---
### FunctionDef: `get_cluster_primary_label_batch`

Batched version of :func:`get_cluster_primary_label`.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
clusts : IndexBatch
    (C) List of cluster indexes
column : int
    Column in the label tensor which specifies the requested label

Returns
-------
TensorBatch
    (C) List of cluster primary labels

---
### FunctionDef: `get_cluster_sizes`

Returns the sizes of each cluster.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
clusts : List[np.ndarray]
    (C) List of cluster indexes

Returns
-------
np.ndarray
    (C) List of cluster sizes

---
### FunctionDef: `get_cluster_start_points`

Estimates the start point of clusters based on their PCA and the 
local curvature at each of the PCA extrema.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
clusts : List[np.ndarray]
    (C) List of cluster indexes

Returns
-------
np.ndarray
    (C, 3) Cluster start points

---
### FunctionDef: `get_confluence_points`

Find the points where multiple particles touch.

Parameters
----------
start_points : np.ndarray
    (P, 3) Particle start points
end_points : np.ndarray, optional
    (P, 3) Particle end points
touching_threshold : float, default 2.0
    Maximum distance for two particle points to be considered touching

Returns
-------
List[np.ndarray]
    List of vertices that correspond to the confluence points

---
### FunctionDef: `get_contributors`

Gets the list of [module ID, tpc ID] pairs that contributed to a
particle or interaction object, as defined in this geometry.

Parameters
----------
sources : np.ndarray
    (N, 2) Array of [module ID, tpc ID] pairs, one per point

Returns
-------
List[np.ndarray]
    (2, N_t) Pair of arrays: the first contains the list of
    contributing modules, the second of contributing tpcs.

---
### FunctionDef: `get_coords`

Gets the coordinates of a larcv.Vertex object.

Parameters
----------
position : larcv.Vertex
    Encodes the position of a point with attributes x, y, z and t

Returns
-------
List[float]
    Coordinates of the point (x, y, z)

---
### FunctionDef: `get_counts`

Finds the number of elements in each entry, provided a batch ID list.

Parameters
----------
batch_ids : Union[np.ndarray, torch.Tensor]
    List of batch IDs
batch_size : int
    Number of entries that make up the batched data

Returns
-------
np.ndarray
    (B) Length of each entry

---
### FunctionDef: `get_depositions`

Get a certain pre-defined deposition attribute of an object.

The :class:`TruthFragment`, :class:`TruthParticle` and
:class:`TruthInteraction` objects points are obtained using the
`truth_dep_mode` attribute of the class.

Parameters
----------
obj : Union[FragmentBase, ParticleBase, InteractionBase]
    Fragment, Particle or Interaction object

Results
-------
np.ndarray
    (N) Depositions

---
### FunctionDef: `get_distance_weights`

Define weights for each of the points in the image based on their
distance from points of interests (typically vertices, but user defined).

Parameters
----------
seg_label : TensorBatch
    (N, 1 + D + 1) Tensor of segmentation labels for the batch
point_label : TensorBatch
    (P, 1 + D + 1) Tensor of points of interests for the batch. This
    is used to upweight the loss of points near a vertex.

Returns
-------
torch.Tensor
    (N) Array of weights associated with each point

---
### FunctionDef: `get_edge_distances`

For each edge, finds the closest points of approach (CPAs) between the
two voxel clusters it connects, and the distance that separates them.

Notes
-----
The voxel IDs correspond to the voxel list, not an index within a cluster.

Parameters
----------
voxels : Union[np.ndarray, torch.Tensor
    (N,3) Tensor of voxel coordinates
clusts : List[np.ndarray]
    (C) List of arrays of voxel IDs in each cluster
edge_index : Union[np.ndarray, torch.Tensor]
    (2, E) Incidence matrix

Returns
-------
np.ndarray
    (E) List of edge lengths
np.ndarray
    (E) List of voxel IDs corresponding to the first edge cluster CPA
np.ndarray
    (E) List of voxel IDs corresponding to the second edge cluster CPA

---
### FunctionDef: `get_edges`

Finds the edges between successive entries in the batch.

Parameters
----------
counts : Union[np.ndarray, torch.Tensor]
    (B)Length of each entry

Returns
-------
np.ndarray
    (B+1) Edges of successive entries in the batch

---
### FunctionDef: `get_entry`

Narrow down the graph to one specific (batch_id, shape) pair.

Parameters
----------
graph : dict
    Dictionary of graph attributes organized by batch and shape
batch_id : int
    Batch index
semantic_id : int
    Semantic type

Returns
-------
dict
    Dictionary of graph attributes for one (batch_id, shape) pair

---
### FunctionDef: `get_file_entry_index`

Returns the index of an entry within the file it lives in,
provided a global index over the list of files.

Parameters
----------
idx : int
    Integer entry ID to access

Returns
-------
int
    Index of the entry in the file

---
### FunctionDef: `get_file_index`

Returns the index of the file corresponding to a specific entry.

Parameters
----------
idx : int
    Integer entry ID to access

Returns
-------
int
    Index of the file in the file list

---
### FunctionDef: `get_file_path`

Returns the path to the file corresponding to a specific entry.

Parameters
----------
idx : int
    Integer entry ID to access

Returns
-------
str
    Path to the file

---
### FunctionDef: `get_flash`

Fetch a given flashmatch::Flash object.

Parameters
----------
idx : int
    ID of the flash to fetch
array : bool, default `False`
    If `True`, The flash is returned as an np.ndarray

Returns
-------
Union[flashmatch::Flash, np.ndarray]
    Flash object

---
### FunctionDef: `get_fragment_edges`

Function that converts a set of edges between cluster ids
to a set of edges between fragment ids (ordering in list).

Parameters
----------
graph : Union[np.ndarray, torch.Tensor]
    (E, 2) Tensor of [clust_id_1, clust_id_2]
clust_ids : np.ndarray
    (C) List of fragment cluster ids

Returns
-------
np.ndarray
    (E,2) Tensor of true edges [frag_id_1, frag_id2]

---
### FunctionDef: `get_group_primary_ids`

Gets the group primary status of particle fragments.

This could be handled somewhere else (e.g. Supera).

Parameters
----------
particles : List[larcv.Particle]
    (P) List of true particle instances
valid_mask : np.ndarray, optional
    (P) Particle label validity mask

Results
-------
np.ndarray
    (P) List of particle group primary IDs, one per true particle instance

---
### FunctionDef: `get_index`

Get a certain pre-defined index attribute of an object.

The :class:`TruthFragment`, :class:`TruthParticle` and
:class:`TruthInteraction` objects index are obtained using the
`truth_index_mode` attribute of the class.

Parameters
----------
obj : Union[FragmentBase, ParticleBase, InteractionBase]
    Fragment, Particle or Interaction object

Results
-------
np.ndarray
    (N) Object index

---
### FunctionDef: `get_index`

Get a certain pre-defined index attribute of an object.

The :class:`TruthFragment`, :class:`TruthParticle` and
:class:`TruthInteraction` objects index are obtained using the
`truth_index_mode` attribute of the class.

Parameters
----------
obj : Union[FragmentBase, ParticleBase, InteractionBase]
    Fragment, Particle or Interaction object

Results
-------
np.ndarray
   (N) Object index

---
### FunctionDef: `get_index`

Get a certain pre-defined index attribute of an object.

The :class:`TruthFragment`, :class:`TruthParticle` and
:class:`TruthInteraction` objects index are obtained using the
`truth_index_mode` attribute of the class.

Parameters
----------
obj : Union[FragmentBase, ParticleBase, InteractionBase]
    Fragment, Particle or Interaction object

Results
-------
np.ndarray
   (N) Object index

---
### FunctionDef: `get_inference_cfg`

Turns a training configuration into an inference configuration.

This script does the following:
- Turn `train` to `False`
- Set sequential sampling
- Load the specified validation file_keys, if requested
- Load the specified set of weight_path, if requested
- Reset the batch_size to a different value, if requested
- Sets num_workers to a different value, if requested
- Make the model run in CPU mode, if requested

Parameters
----------
cfg : Union[str, dict]
    Configuration file or Path to the configuration file
file_keys : str, optional
    Path to the dataset to use for inference
weight_path : str, optional
    Path to the weigths to use for inference
batch_size : int, optional
    Number of data samples per batch
num_workers : int, optional
    Number of workers that load data
cpu : bool, default False
    Whether or not to execute the inference on CPU

Returns
-------
dict
    Dictionary of parameters to initialize handlers

---
### FunctionDef: `get_input_data`

Fetches the required data products from the LArCV data trees, pass
them to the parser function.

Parameters
----------
trees : dict
    Dictionary which maps each data product name to a LArCV object

Results
-------
object
    Output(s) of the parser function

---
### FunctionDef: `get_instance_masks`

Given integer coded cluster instance labels, construct a
(N x max_num_instances) bool tensor in which each colume is a 
binary instance mask.

---
### FunctionDef: `get_inter_primary_ids`

Gets the interaction primary ID for each particle.

Parameters
----------
particles : List[larcv.Particle]
    (P) List of true particle instances
valid_mask : np.ndarray, optional
    (P) Particle label validity mask

Results
-------
np.ndarray
    (P) List of particle primary IDs, one per true particle instance

---
### FunctionDef: `get_interaction_ids`

Gets the interaction ID of each particle.

If the `interaction_id` attribute of the Particle class is filled,
it simply uses that quantity.

Otherwise, it leverages shared ancestor position as a basis for
interaction building and sets the interaction ID to -1 for particles with
invalid ancestor track IDs.

Parameters
----------
particles : List[larcv.Particle]
    (P) List of true particle instances
valid_mask : np.ndarray, optional
    (P) Particle label validity mask

Results
-------
np.ndarray
    (P) List of interaction IDs, one per true particle instance

---
### FunctionDef: `get_loss_accuracy`

Computes the loss, global and classwise accuracy.

Parameters
----------
logits : torch.Tensor
    (N, N_c) Output logits from the network for each voxel
labels : torch.Tensor
    (N) Target values for each voxel
weights : torch.Tensor, optional
    (N) Tensor of weights for each pixel in the batch

Returns
-------
torch.Tensor
    Cross-entropy loss value
float
    Global accuracy
np.ndarray
    (N_c) Vector of class-wise accuracy
torch.Tensor
    (N) Updated set of weights for each pixel in the batch

---
### FunctionDef: `get_masked_dbscan_labels`

Produce instance clusters using the masked-DBSCAN method.

Parameters
----------
voxels : np.ndarray
    (N, 3) Set of voxel coordinates
points : np.ndarray
    (P, 3) Set of particle end points

Returns
-------
np.ndarray
    (N) Array of cluster assignments for each voxel in the input

---
### FunctionDef: `get_match`

Fetch a match for a given TPC interaction ID.

Parameters
----------
idx : int
    Index of TPC object for which we want to retrieve a match

Returns
-------
flashmatch::FlashMatch_t
    Flash match associated with interaction idx

---
### FunctionDef: `get_matched_flash`

Fetch a matched flash for a given TPC interaction ID.

Parameters
----------
idx : int
    Index of TPC object for which we want to retrieve a match

Returns
-------
flashmatch::Flash_t
    Optical flash that matches interaction idx

---
### FunctionDef: `get_matches`

Find TPC interactions compatible with optical flashes.

Parameters
----------
interactions : List[Union[Interaction, TruthInteraction]]
    List of TPC interactions
flashes : List[Flash]
    List of optical flashes

Returns
-------
List[Tuple[Interaction, Flash, flashmatch::FlashMatch_t]]
    Set of interaction/flash matches with their matching characteristics

---
### FunctionDef: `get_matches`

Makes [interaction, flash] pairs that have compatible barycenters.

Parameters
----------
interactions : List[Union[RecoInteraction, TruthInteraction]]
    List of interactions
flashes : List[Flash]
    List of optical flashes

Returns
-------
List[[Interaction, larcv.Flash, float]]
    List of [interaction, flash, distance] triplets

---
### FunctionDef: `get_min_volume_offset`

Get the minimum offset to apply to a point cloud to bring it
within the boundaries of a volume.

Parameters
----------
points : np.ndarray
    (N, 3) : Point coordinates
module_id : int
    ID of the module
tpc_id : int, optional
    ID of the TPC within the module. If not specified, the volume
    offsets are estimated w.r.t. the module itself

Returns
-------
np.ndarray
    (3) Offsets w.r.t. to the volume location

---
### FunctionDef: `get_nu_ids`

Gets the neutrino-like ID of each partcile

Convention: -1 for non-neutrinos, neutrino index for others

If a list of multi-particle vertex (MPV) particles or neutrinos is
provided, that information is leveraged to identify which interactions
are neutrino-like and which are not.

If `particles_mpv` and `neutrinos` are not specified, it assumes that
only neutrino-like interactions have more than one true primary
particle in a single interaction.

Parameters
----------
particles : List[larcv.Particle]
    (P) List of true particle instances
inter_ids : np.ndarray
    (P) Array of interaction ID values, one per true particle instance
particles_mpv : List[larcv.Particle], optional
    (M) List of true MPV particle instances
neutrinos : list(larcv.Neutrino), optional
    (N) List of true neutrino instances

Results
-------
np.ndarray
    (P) List of neutrino IDs, one per true particle instance

---
### FunctionDef: `get_object_dtype`

Loop over the attributes of a class to figure out what to store.

This function assumes that the class only posseses getters that return
either a scalar, string or np.ndarrary.

Parameters
----------
object : class
    Instance of an class used to identify attribute types

Returns
-------
list
    List of (key, dtype) pairs

---
### FunctionDef: `get_optimal_parameters`

Retrives optimal seediness and probability thresholds for dense clustering.

INPUTS:
    - fname: post-processing output filename (*.csv file)
    - metric: name of performance metric for which to optimize values on.

RETURNS:
    - s_thresholds: dict of { semantic class : optimal seediness threshold } pairs
    - p_thresholds: dict of { semantic class : optimal pvalue threshold } pairs
    - max_values: maximum value of metric using optimal thresholding values.

---
### FunctionDef: `get_particle_ids`

Gets a particle species ID (PID) for each particle.

This function ensures:
- All shower daughters are labeled the same as their primary. This
  makes sense as otherwise an electron primary gets overruled by
  its many photon daughters (voxel-wise majority vote). This can
  lead to problems as, if an electron daughter is not clustered with
  the primary, it is labeled electron, which is counter-intuitive.
  This is handled downstream with the high_purity flag.
- Particles that are not in the list target are labeled -1

Parameters
----------
particles : List[Particle]
    (P) List of true particle instances
valid_mask : np.ndarray, optional
    (P) Particle label validity mask

Returns
-------
np.ndarray
    (P) List of particle IDs, one per true particle instance

---
### FunctionDef: `get_particle_points`

Associate PPN points with particle clusters.

Given a list particle or fragment clusters, leverage the raw PPN output
to produce a list of start points for shower objects and of start/end
points for track objects:
- For showers, pick the most likely PPN point
- For tracks, pick the two points farthest away from each other

Parameters
----------
coords : numpy.ndarray
    Array of coordinates of voxels in the image
clusts : List[numpy.ndarray]
    List of clusters representing the fragment or particle objects
clusts_seg : numpy.ndarray
    Array of cluster semantic types
ppn_points : numpy.ndarray
    Raw output of PPN
contained_first : bool, default True
    If `True`, for shower points, give precedence to voxels which
    predict a point within one voxel of their location
anchor_points : bool, default True
    If `True`, the point estimates are brought to the closest cluster voxel
enhance_track_points, default False
    If `True`, tracks leverage PPN predictions to provide a more
    accurate estimate of the end points. This needs to be avoided for
    track fragments, as PPN is typically not trained to find end points
    for them. If set to `False`, the two voxels farthest away from each
    other are picked.
approx_farthest_points: bool, default True
    If `True`, approximate the computation of the two farthest points

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_per_class_probabilities`

Computes binary foreground/background loss.

---
### FunctionDef: `get_pid`

Get a certain pre-defined PID prediction of an object.

The :class:`RecoParticle` PID predictions are obtained using the
`pid_mode` attribute of the class.

Parameters
----------
obj : Union[ParticleBase]
    Particle object

Results
-------
int
    Particle identification enumerator

---
### FunctionDef: `get_points`

Get a certain pre-defined point attribute of an object.

The :class:`TruthFragment`, :class:`TruthParticle` and
:class:`TruthInteraction` objects points are obtained using the
`truth_point_mode` attribute of the class.

Parameters
----------
obj : Union[FragmentBase, ParticleBase, InteractionBase]
    Fragment, Particle or Interaction object

Results
-------
np.ndarray
    (N, 3) Point coordinates

---
### FunctionDef: `get_points`

Get a certain pre-defined point attribute of an object.

The :class:`TruthFragment`, :class:`TruthParticle` and
:class:`TruthInteraction` objects points are obtained using the
`truth_point_mode` attribute of the class.

Parameters
----------
obj : Union[FragmentBase, ParticleBase, InteractionBase]
    Fragment, Particle or Interaction object

Results
-------
np.ndarray
   (N, 3) Point coordinates

---
### FunctionDef: `get_ppn_labels`

Gets particle point coordinates and informations for running PPN.

We skip some particles under specific conditions (e.g. low energy deposit,
low voxel count, nucleus track, etc.)

Parameters
----------
particle_v : List[larcv.Particle]
    List of LArCV particle objects in the image
meta : larcv::Voxel3DMeta or larcv::ImageMeta
    Metadata information
dtype : str
    Typing of the output PPN labels
dim : int, default 3
    Number of dimensions of the image
min_voxel_count : int, default 5
    Minimum number of voxels associated with a particle to be included
min_energy_deposit : float, default 0
    Minimum energy deposition associated with a particle to be included
include_point_tagging : bool, default True
    If True, include an a label of 0 for start points and 1 for end points

Returns
-------
np.array
    Array of points of shape (N, 5/6) where 5/6 = x,y,z + point type
    + particle index [+ start (0) or end (1) point tagging]

---
### FunctionDef: `get_ppn_positives`

Get ppn positive label mask, but with cluster restrictions.

Parameters
----------
coords : torch.Tensor
    (N, 3) 3D coordinates of the image voxels
labels : torch.Tensor
    (N) tensor of the particle id label for each voxel
ppn_label : torch.Tensor
    (N, 1 + D + N_l) Tensor of PPN labels for the batch
resolution : float
    Distance from a label point in pixels within which a voxel is
    considered positive (pixel of interest)
offset : int
    The index offset needed to transform within-batch index to
    global (image) index.

Returns
-------
positives : torch.Tensor
    (N) tensor of the positive label mask
closests : torch.Tensor
    (N) tensor of the closest label point index

---
### FunctionDef: `get_prefixes`

Builds an appropriate output prefix based on the list of input files.

Parameters
----------
file_paths : List[str]
    List of input file paths
split_output : bool
    Split the output of the process into one file per input file

Returns
-------
Union[str, List[str]]
    Shared input summary string to be used to prefix outputs

---
### FunctionDef: `get_pseudovertex`

Finds the vertex which minimizes the total distance from itself to all
the lines defined by the start points of particles and their directions.

Parameters
----------
start_points : np.ndarray
    (P, 3) Particle start points
directions : np.ndarray
    (P, 3) Particle directions
dim : int
    Number of dimensions

---
### FunctionDef: `get_qcluster`

Fetch a given flashmatch::QCluster_t object.

Parameters
----------
idx : int
    ID of the interaction to fetch
array : bool, default `False`
    If `True`, The QCluster is returned as an np.ndarray

Returns
-------
Union[flashmatch::QCluster_t, np.ndarray]
    QCluster object

---
### FunctionDef: `get_run_event`

Returns an entry corresponding to a specific (run, subrun, event)
triplet.

Parameters
----------
run : int
    Run number
subrun : int
    Subrun number
event : int
    Event number

Returns
-------
data_blob : dict
    Ditionary of input data products corresponding to one event
result_blob : dict
    Ditionary of result data products corresponding to one event

---
### FunctionDef: `get_run_event_index`

Returns an entry index corresponding to a specific
(run, subrun, event) triplet.

Parameters
----------
run : int
    Run number
event : int
    Event number

---
### FunctionDef: `get_sources`

Converts logical TPC indexes to physical TPC indexes.

Parameters
----------
sources : np.ndarray
    (N, 2) Array of logical [module ID, tpc ID] pairs, one per point

Returns
----------
np.ndarray
    (N, 2) Array of physical [module ID, tpc ID] pairs, one per point

---
### FunctionDef: `get_sources`

Get a certain pre-defined sources attribute of an object.

The :class:`TruthFragment`, :class:`TruthParticle` and
:class:`TruthInteraction` objects sources are obtained using the
`truth_source_mode` attribute of the class.

Parameters
----------
obj : Union[FragmentBase, ParticleBase, InteractionBase]
    Fragment, Particle or Interaction object

Results
-------
np.ndarray
    (N, 2) Object sources

---
### FunctionDef: `get_stored_keys`

Get the list of data product keys to store.

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
keys : list
    List of data keys to store to file

---
### FunctionDef: `get_t0`

Fetch a matched flash time for a given TPC interaction ID.

Parameters
----------
idx : int
    Index of TPC object for which we want to retrieve a match

Returns
-------
float
    Time in us with respect to simulation time reference

---
### FunctionDef: `get_track_deposition_gradient`

Given a set of point coordinates and their values associated with a
track and a start point, compute the deposition gradient with respect to
the start point.

Parameters
----------
coordinates : np.ndarray
    (N, 3) Coordinates of the points that make up the track
values : np.ndarray
    (N) Values associated with each point
start_point : np.ndarray
    (3) End point of the track
segment_length : float, default 5
    Segment length in the units that specify the coordinates
method : str, default 'step_next'
    Method used to segment the track (one of 'step', 'step_next'
    or 'bin_pca')
anchor_point : bool, default True
    Weather or not to collapse end point onto the closest track point
min_count : int, default 10
    Minimum number of points in a segment for it to be valid. If not valid,
    the dedx value for that segment is not used to compute the gradient.

Returns
-------
gradient : float
   Deposition gradient along the track from the start point
segment_dedxs : np.ndarray
   (S) Array of energy/charge deposition rate values
segment_rrs : np.ndarray
   (S) Array of residual ranges (center of the segment w.r.t. end point)
segment_lengths : np.ndarray
   (S) Array of segment lengths

---
### FunctionDef: `get_track_length`

Given a set of point coordinates associated with a track and one of its
end points, compute its length.

Parameters
----------
coordinates : np.ndarray
    (N, 3) Coordinates of the points that make up the track
segment_length : float, optional
    Segment length in the units that specify the coordinates
point : np.ndarray, optional
    (3) An end point of the track
method : str, default 'bin_pca'
    Method used to compute the track length (one of 'displacement', 'step',
    'step_next', 'bin_pca' or 'spline')
anchor_point : bool, default True
    Weather or not to collapse end point onto the closest track point
min_count : int, default 10
    Minimum number of points in a segment to use it to evaluate the
    direction of the next step along the track.
spline_smooth : float, optional
    The smoothing factor to be used in spline regression, when used

Returns
-------
float
   Total length of the track

---
### FunctionDef: `get_track_segment_dedxs`

Given a set of point coordinates and their values associated with a
track and one of its end points, compute the energy/charge deposition rate
as a function of the residual range.

Parameters
----------
coordinates : np.ndarray
    (N, 3) Coordinates of the points that make up the track
values : np.ndarray
    (N) Values associated with each point
end_point : np.ndarray, optional
    (3) End point of the track
segment_length : float, default 5.
    Segment length in the units that specify the coordinates
method : str, default 'step_next'
    Method used to segment the track (one of 'step', 'step_next'
    or 'bin_pca')
anchor_point : bool, default True
    Weather or not to collapse end point onto the closest track point
min_count : int, default 10
    Minimum number of points in a segment for it to be valid. If not valid,
    the dedx value returned for the segment is -1.

Returns
-------
seg_dedxs : np.ndarray
   (S) Array of energy/charge deposition rate values
seg_errs : np.ndarray
   (S) Array of uncertainties on the energy/charge deposition rate
seg_rrs : np.ndarray
   (S) Array of residual ranges (center of the segment w.r.t. end point)
seg_clusts : List[np.ndarray]
   (S) List of indexes which correspond to each segment cluster of points
seg_dirs : np.ndarray
   (S, 3) Array of segment direction vectors
seg_lengths : np.ndarray
   (S) Array of segment lengths

---
### FunctionDef: `get_track_segments`

Given a set of point coordinates associated with a track and one of its
end points, divide the track into segments of the requested length.

Parameters
----------
coordinates : np.ndarray
    (N, 3) Coordinates of the points that make up the track
segment_length : float
    Segment length in the units that specify the coordinates
point : np.ndarray, optional
    (3) A preferred end point of the track from which to start
method : str, default 'step_next'
    Method used to segment the track (one of 'step', 'step_next'
    or 'bin_pca')
anchor_point : bool, default True
    Weather or not to collapse end point onto the closest track point
min_count : int, default 10
    Minimum number of points in a segment to use it to evaluate the
    direction of the next step along the track.

Returns
-------
segment_clusts : List[np.ndarray]
   (S) List of indexes which correspond to each segment cluster of points
segment_dirs : np.ndarray
   (S, 3) Array of segment direction vectors
segment_lengths : np.ndarray
   (S) Array of segment lengths

---
### FunctionDef: `get_track_spline`

Estimate the best approximating curve defined by a point cloud using
univariate 3D splines.

The length is computed by measuring the length of the piecewise linear
interpolation of the spline at points defined by the bin size.

Parameters
----------
coordinatea : np.ndarray
    (N, 3) point cloud
segment_length : float
    The subdivision length at which to sample points from the spline.
    If the track length is less than the segment_length, then the returned
    length will be computed from the farthest two projected points along
    the track's principal direction.
s : float, optional
    The smoothing factor to be used in spline regression, by default None

Returns
-------
u : np.ndarray
    (N) The principal axis parametrization of the curve
    C(u) = (spx(u), spy(u), spz(u))
sppoints : np.ndarray
    (N, 3) The graph of the spline at points u
splines : scipy.interpolate.UnivariateSpline
    Approximating splines for the point cloud defined by points
length : float
    The estimate of the total length of the curve

---
### FunctionDef: `get_training_df`

Finds all training log files inside the specified directory and
concatenates them. If the range of iterations overlap, keep only that
from the file started further in the training.

Assumes that the formatting of the log file names is of the form
`self.train_prefix-x.csv`, with `x` the number of iterations.

Parameters
----------
log_dir : str
    Path to the directory that contains the training log files
keys : List[str]
    List of quantities to extract from the log files

Returns
-------
pd.DataFrame
    Combined training log data

---
### FunctionDef: `get_valid_mask`

Gets a mask corresponding to particles with valid labels.

This function checks that the particle labels have been filled properly at
the Supera level. It checks that the ancestor track ID of each particle is
not an invalid number and that the ancestor creation process is filled.

Parameters
----------
particles : List[larcv.Particle]
    (P) List of true particle instances

Results
-------
np.ndarray
    (P) Boolean list of validity, one per true particle instance

---
### FunctionDef: `get_validation_df`

Finds all validation log files inside the specified directory and
build a single dataframe out of them. It returns the mean and std of
the requested keys for each file.

Assumes that the formatting of the log file names is of the form
`self.val_prefix-x.csv`, with `x` the number of iterations.

The key list allows for `:`-separated names, in case separate files
use different names for the same quantity.

Parameters
----------
log_dir : str
    Path to the directory that contains the validation log files
keys : List[str]
    List of quantities to extract from the log files

Returns
-------
pd.DataFrame
    Combined validation log data

---
### FunctionDef: `get_vertex`

Reconstruct the vertex of an individual interaction.

Parameters
----------
start_points : np.ndarray
    (P, 3) Particle start points
end_points : np.ndarray
    (P, 3) Particle end points
directions : np.ndarray
    (P, 3) Particle directions
semantics : np.ndarray
    (P) : particle semantic type
anchor_vertex : bool, default True
    If true, anchor the candidate vertex to particle objects,
    with the expection of interactions only composed of showers.
touching_threshold : float, default 2.0
    Maximum distance for two particle points to be considered touching
return_mode : bool, default False
    If `True`, return the method used to find the vertex

---
### FunctionDef: `get_vertex_labels`

Gets particle vertex coordinates.

It provides the coordinates of points where multiple particles originate:
- If the `neutrino_event` is provided, it simply uses the coordinates of
  the neutrino interaction points.
- If the `particle_event` is provided instead, it looks for ancestor point
  positions shared by at least two **primary** particles.

Parameters
----------
particle_v : List[larcv.Particle]
    List of LArCV particle objects in the image
neutrino_v : List[larcv.Neutrino]
    List of LArCV neutrino objects in the image
meta : larcv::Voxel3DMeta or larcv::ImageMeta
    Metadata information
dtype : str
    Typing of the output PPN labels

Returns
-------
np.array
    Array of points of shape (N, 4) where 4 = x, y, z, vertex_id

---
### FunctionDef: `get_volume_index`

Gets the list of indices of points that belong to a certain
detector volume (module or individual TPC).

Parameters
----------
sources : np.ndarray
    (N, 2) Array of [module ID, tpc ID] pairs, one per point
module_id : int
    ID of the module
tpc_id : int, optional
    ID of the TPC within the module. If not specified, the volume
    offsets are estimated w.r.t. the module itself

Returns
-------
np.ndarray
    (N) Index of points that belong to the requested detector volume

---
### FunctionDef: `get_volume_offsets`

Compute how far each point is from a certain detector volume.

Parameters
----------
points : np.ndarray
    (N, 3) : Point coordinates
module_id : int
    ID of the module
tpc_id : int, optional
    ID of the TPC within the module. If not specified, the volume
    offsets are estimated w.r.t. the module itself

Returns
-------
np.ndarray
    (N, 3) Offsets w.r.t. to the volume boundaries

---
### FunctionDef: `get_voxel_edge_features`

Returns a tensor of edge features for each edge connecting 
point individual voxels in the graph.

The edge features (N_e = 19) include (in that order):
- Coordinates of the source voxel (3)
- Coordinates of the target voxel (3)
- Displacement vector between the two aforementioned voxels (3)
- Magnitude of the displacement vector (1)
- Outer product of the displacement vector (9)

Parameters
----------
data : Union[np.ndarray, torch.Tensor]
    (N, 1 + D + N_f) Batched sparse tensors
clusts : List[np.ndarray]
    (C) List of arrays of voxels IDs in each cluster
edge_index : Union[np.ndarray, torch.Tensor]
    (2, E) Incidence map between voxels

Returns
-------
np.ndarray
    (E, N_e) Tensor of edge features

---
### FunctionDef: `get_voxel_edge_features_batch`

Batched version of :func:`get_voxel_edge_features`.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
edge_index : EdgeIndexBatch
    (2, E) Sparse incidence matrix

Returns
-------
TensorBatch
    (E, N_e) List of edge features between voxels.

---
### FunctionDef: `get_voxel_features`

Returns an array of features for each voxel.

The basic 16 geometric features are composed of:
- Voxel coordinates
- Covariance matrix of its neighborhood (3)
- Principal axis of its neighborhood (3)
- Voxel count in its neighborhood (1)

The neighborhood of the voxel i defined as all voxels within some distance
of the voxel to get features for.

Parameters
----------
data : np.ndarray
    Cluster label data tensor
max_dist : float, default 5.0
    Neighborhood radius

Returns
-------
np.ndarray
    (C, N_c) Tensor of voxels features

---
### FunctionDef: `get_voxel_features_batch`

Returns an array of features for each voxel.

The basic 16 geometric features are composed of:
- Voxel coordinates
- Covariance matrix of its neighborhood (3)
- Principal axis of its neighborhood (3)
- Voxel count in its neighborhood (1)

The neighborhood of the voxel i defined as all voxels within some distance
of the voxel to get features for.

Parameters
----------
data : TensorBatch
    Batch of cluster label data tensor
max_dist : float, default 5.0
    Neighborhood radius

Returns
-------
np.ndarray
    (C, N_c) Tensor of voxels features

---
### FunctionDef: `global_encoder_factory`

Instantiates a global graph encoder from a configuration dictionary.

Parameters
----------
cfg : dict
    Global graph encoder configuration

Returns
-------
object
    Instantiated global graph encoder

---
### FunctionDef: `global_layer_factory`

Instantiates a GNN global update layer from a configuration dictionary.

Parameters
----------
cfg : dict
    GNN global update layer configuration
node_in : int
    Number of input node features
glob_in : int
    Number of input global graph features

Returns
-------
object
    Instantiated GNN global update layer

---
### FunctionDef: `global_loss_factory`

Instantiates a global graph loss from a configuration dictionary.

Parameters
----------
cfg : dict
    Global graph loss configuration

Returns
-------
object
    Instantiated global graph loss

---
### FunctionDef: `gnn_model_factory`

Instantiates a GNN model from a configuration dictionary.

Parameters
----------
cfg : dict
    GNN model configuration

Returns
-------
object
    Instantiated GNN model

---
### ClassDef: `GNNExplainerWrapper`

Wrapper module for formatting GNN models into GNNExplainer
applicable modules.

---
### FunctionDef: `graph_factory`

Instantiates a graph constructor from a configuration dictionary.

Parameters
----------
cfg : dict
    Graph constructor configuration
classes : Union[int, list]
    List of classes to build a graph on

Returns
-------
object
    Instantiated graph constructor

---
### ClassDef: `GraphBase`

Parent class for all graph constructors.

---
### ClassDef: `GraphSPICE`

Graph Scalable Proposal-free Instance Clustering Engine (Graph-SPICE).

Graph-SPICE has two components:
1. Voxel embedder: UNet-type CNN architecture used for feature
   extraction and feature embeddings.
2. Edge probability kernel function: A kernel function (any callable
   that takes two node attribute vectors to give a edge proability score).

Prediction is done in two steps:
1. A neighbor graph (ex. KNN, Radius) is constructed to compute
   edge probabilities between neighboring edges;
2. Edges with low probability scores are dropped;
3. The voxels are clustered through connected component clustering.

A typical configuration is broken down into multiple components:

.. code-block:: yaml

    model:
      name: graph_spice
      modules:
        graph_spice:
          <Basic parameters>
          embedder:
            <Feature embedding configuration block>
          kernel:
            <Edge kernel function configuration block>
          constructor:
            <Graph construction base parameters>
            graph:
              <Graph configuration block>
            orphan:
              <Orphan assignment configuration block>

See configuration file(s) prefixed with `graph_spice` under the `config`
directory for detailed examples of working configurations.

---
### ClassDef: `GraphSPICEEmbedder`

Model which produces embeddings of an input sparse point cloud.

---
### ClassDef: `GraphSPICEEmbeddingLoss`

Loss function for Sparse Spatial Embeddings Model, with fixed
centroids and symmetric gaussian kernels.

---
### ClassDef: `GraphSPICELoss`

Loss function for Graph-SPICE.

For use in config:

..  code-block:: yaml

    model:
      name: graph_spice
      modules:
        graph_spice_loss:
          <Basic parameters>
          edge_loss:
            <Edge loss configuration block>

See configuration files prefixed with `graph_spice` under the `config`
directory for detailed examples of working configurations.

See Also
--------
:class:`GraphSPICE`

---
### ClassDef: `GrapPA`

Graph Particle Aggregator (GrapPA) model.

This class mostly acts as a wrapper that will hand the graph data
to the underlying graph neural network (GNN).

When trained standalone, this model must be provided with a cluster
label tensor, allowing it to build a set of intput clusters based on the
label boundaries of the clusters and their semantic types.

Typical configuration can look like this:

.. code-block:: yaml

    model:
      name: grappa
      modules:
        grappa:
          nodes:
            <dictionary of arguments to specify the input type>
          graph:
            name: <name of the input graph type>
            <dictionary of arguments to specify the graph>
          node_encoder:
            name: <name of the type of node encoder>
            <dictionary of arguments to specify the node encoder>
          edge_encoder:
            name: <name of the type of edge encoder>
            <dictionary of arguments to specify the edge encoder>
          global_encoder:
            name: <name of the type of global encoder>
            <dictionary of arguments to specify the global encoder>
          gnn_model:
            name: <name of the type of backbone GNN feature extractor>
            <dictionary of arguments to specify the GNN>

See configuration files prefixed with `grappa_` under the `config`
directory for detailed examples of working configurations.

See Also
--------
:class:`GrapPALoss`

---
### ClassDef: `GrapPALoss`

Takes the output of the GrapPA and computes the total loss.

For use in config:

..  code-block:: yaml

    model:
      name: grappa
      modules:
        grappa_loss:
          node_loss:
            name: <name of the node loss>
            <dictionary of arguments to pass to the loss>
          edge_loss:
            name: <name of the edge loss>
            <dictionary of arguments to pass to the loss>
          global_loss:
            name: <name of the global loss>
            <dictionary of arguments to pass to the loss>

Each of the specific loss blocks can also contain multiple losses by
providing a name key in a loss block nested below it. Each loss name of a
specific type should be provided with a corresponding output from GRaPA.

See configuration files prefixed with `grappa_` under the `config`
directory for detailed examples of working configurations.

---
### FunctionDef: `group_labels`

Aggregate particles using labels.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
clusts : IndexBatch
    List of clusters to aggregate using GrapPA
clust_shapes : TensorBatch
    Semantic type of each of the clusters
aggregate_shapes : bool, default False
    Combine shapes to give a shape to the aggregated object
shape_use_primary : bool, default False
    Use primary shape as the group shape
retain_primaries : bool, default False
    Retain the primary cluster

Returns
-------
groups : IndexBatch
    List of cluster groups aggregated using labels
group_shapes : TensorBatch
    Semantic type of each of the cluster groups
group_primaries : IndexBatch
    List of primary clusters for each group
shape_index : np.ndarray
    List of indexes used to restrict the original cluster list

---
### FunctionDef: `grouping_loss`

Defines the graph clustering score.

Given a target adjacency matrix A and a predicted adjacency P, the score is
evaluated the average CE, L1 or L2 distance between truth and prediction.

Parameters
----------
pred_mat : np.ndarray
    (C*C) Predicted adjacency matrix scores (flattened)
target_mat : np.ndarray
    (C*C) Target adjacency matrix scores (flattened)
loss : str, default 'ce'
    Loss mode used to compute the graph score

Returns
-------
float
    Graph grouping loss

---
### ClassDef: `HDF5Reader`

Class which reads information stored in HDF5 files.

This class inherits from the :class:`ReaderBase` class. It provides
methods to load HDF5 files and extract their data products. The files
must be structured as follows:
  - An `events` dataset with all the region references
  - One dataset per data product corresponding to each region reference in
    the `events` dataset

---
### ClassDef: `HDF5Writer`

Writes data to an HDF5 file.

Builds an HDF5 file to store the input and/or the output of the
reconstruction chain. It can also be used to append an existing HDF5 file
with information coming out of the analysis tools.

Typical configuration should look like:

.. code-block:: yaml

    io:
      ...
      writer:
        name: hdf5
        file_name: output.h5
        keys:
          - input_data
          - segmentation
          - ...

---
### FunctionDef: `heatmap`

Create a heatmap from a numpy array and two lists of labels.

Parameters
----------
data
    A 2D numpy array of shape (N, M).
row_labels
    A list or array of length N with the labels for the rows.
col_labels
    A list or array of length M with the labels for the columns.
ax
    A `matplotlib.axes.Axes` instance to which the heatmap is plotted.  If
    not provided, use current axes or create a new one.  Optional.
**kwargs
    All other arguments are forwarded to `imshow`.

---
### FunctionDef: `highland`

Highland scattering formula

Parameters
----------
p : float
   Momentum in MeV/c
M : float
   Impinging particle mass in MeV/c^2
dx : float
    Step length in cm
z : int, default 1
   Impinging partile charge in multiples of electron charge
X0 : float, default LAR_X0
   Radiation length in the material of interest in cm

Results
-------
float
    Expected scattering angle in radians

---
### FunctionDef: `hull_trace`

Converts a cloud of points into a 3D convex hull.

This function represents a point cloud by forming a mesh with the points
that belong to the convex hull of the point cloud.

Parameters
----------
points : np.ndarray
    (N, 3) Array of point coordinates
color : Union[str, float, np.ndarray], optional
    Color of hull
intensity : Union[int, float], optional
    Color intensity of the box along the colorscale axis
hovertext : Union[int, str, np.ndarray], optional
    Text associated with the cone
showscale : bool, default False
    If True, show the colorscale of the :class:`plotly.graph_objs.Mesh3d`
alphahull : float, default 0
    Parameter that sets how to define the hull. 0 is the convex hull,
    larger numbers correspond to alpha-shapes.
**kwargs : dict, optional
    Additional parameters to pass to the underlying
    :class:`plotly.graph_objs.Mesh3d` object

---
### FunctionDef: `image_contains`

Checks whether a point is contained in the image box defined by meta.

Parameters
----------
meta : larcv::Voxel3DMeta or larcv::ImageMeta
    Metadata information
point : larcv::Point3D or larcv::Point2D
    Point to check on
dim: int, default 3
     Number of dimensions of the image

Returns
-------
bool
    True if the point is contained in the image box

---
### FunctionDef: `image_coordinates`

Returns the coordinates of a point in units of pixels with an image.

Parameters
----------
meta : larcv::Voxel3DMeta or larcv::ImageMeta
    Metadata information
point : larcv::Point3D or larcv::Point2D
    Point to convert the units of
dim: int, default 3
     Number of dimensions of the image

Returns
-------
bool
    True if the point is contained in the image box

---
### ClassDef: `ImageClassifier`

Whole-image classification model.

This model uses various encoder declinations to classifier an entire
image as belonging to a certain class.

.. code-block:: yaml
    model:
      name: image_class
      modules:
        classifier:
          # Image classifier configuration
        classifier_loss:
          # Image classifier loss configuration

---
### ClassDef: `ImageClassLoss`

Image classication loss.

---
### FunctionDef: `include`

Load and include a YAML file that is requested in the base config.

Parameters
----------
node : str
    Name of the YAML block to load

---
### FunctionDef: `index`

Alias for the underlying data stored.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (2, E) Underlying batch of edge indexes

---
### FunctionDef: `index`

Alias for the underlying data stored.

Returns
-------
Union[np.ndarray, torch.Tensor]
    Underlying index

---
### FunctionDef: `index`

Unique pix associated with individual axis indexes.

Parameters
----------
coords : np.ndarray
    (N, 2/3) Input pixel indices

Returns
-------
np.ndarray
    (N) Unique pixel index per input pixel

---
### FunctionDef: `index_ids`

Returns the ID of the index in the list each element belongs to.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (M) List of index IDs for each element

---
### FunctionDef: `index_list`

Alias for the underlying data list stored.

Returns
-------
List[Union[np.ndarray, torch.Tensor]]
    Underlying index list

---
### FunctionDef: `index_t`

Alias for the underlying data stored, transposed

Returns
-------
Union[np.ndarray, torch.Tensor]
    (E, 2) Underlying batch of edge indexes, transposed

---
### ClassDef: `IndexBatch`

Batched index with the necessary methods to slice it.

Attributes
----------
offsets : Union[np.ndarray, torch.Tensor]
    (B) Offsets between successive indexes in the batch
single_counts : Union[np.ndarray, torch.Tensor]
    (I) Number of index elements per index in the index list. This
    is the same as counts if the underlying data is a single index

---
### FunctionDef: `inference_single`

Execute a model in inference mode in a single process

Parameters
----------
cfg : dict
    Full driver configuration

---
### FunctionDef: `inherit_docstring`

Inherits docstring attributes of a parent class.

Only handles numpy-style docstrings.

Parameters
----------
*parents : List[object]
    Parent class(es) to inherit attributes from

Returns
-------
callable
    Class with updated docstring

---
### FunctionDef: `initialize`

Initialize one stopwatch. If it's already been initialized,
reset the global counters to 0.

Parameters
----------
key : Union[str, List[str]]
    Key or list of keys to initialize a `Stopwatch` for

---
### FunctionDef: `initialize_backend`

Initialize OpT0Finder (backend).

Expects that the environment variable `FMATCH_BASEDIR` is set.
You can either set it by hand (to the path where one can find
OpT0Finder) or you can source `OpT0Finder/configure.sh` if you
are running code from a command line.

Parameters
----------
cfg: str
    Path to config for OpT0Finder
detector : str, optional
    Detector to get the geometry from
parent_path : str, optional
    Path to the parent configuration file (allows for relative paths)

---
### FunctionDef: `initialize_base`

Initialize the base driver parameters.

Parameters
----------
seed : int
    Random number generator seed
dtype : str, default 'float32'
    Data type of the model parameters and input data
world_size : int, optional
    Number of GPUs to use in the underlying model
gpus : List[int], optional
    List of indexes of GPUs to expose to the model
log_dir : str, default 'logs'
    Path to the directory where the logs will be written to
prefix_log : bool, default False
    If True, use the input file name to prefix the log name
overwrite_log : bool, default False
    If True, overwrite log even if it already exists
parent_path : str, optional
    Path to the parent directory of the analysis configuration file
iterations : int, optional
    Number of entries/batches to process (-1 means all entries)
epochs : int, optional
    Number of times to iterate over the full dataset
unwrap : bool, default False
    Wheather to unwrap batched data (only relevant when using loader)
rank : int, optional
    Rank of the GPU in the multi-GPU training process
log_step : int, default 1
    Number of iterations before the logging is called (1: every step)
distributed : bool, default False
    If `True`, this process is distributed among multiple processes
train : dict, optional
    Training configuration dictionary
split_output : bool, default False
    Split the output of the process into one file per input file
verbosity : int, default 'info'
    Verbosity level to pass to the `logging` module. Pick one of
    'debug', 'info', 'warning', 'error', 'critical'.

Returns
-------
dict
    Training configuration
rank
    Updated rank

---
### FunctionDef: `initialize_calibrator`

Switch model to calibration mode.

Allows to calibrate logits to respond linearly to probability,
for instance.

Parameters
----------
calibrator : dict
    Calibrator configuration dictionary
calibrator_loss : dict
    Calibrator loss configuration dictionary

---
### FunctionDef: `initialize_datasets`

Create place hodlers for all the datasets to be filled.

Parameters
----------
out_file : h5py.File
    HDF5 file instance

---
### FunctionDef: `initialize_io`

Initializes the input/output scripts.

Parameters
----------
loader : dict, optional
    PyTorch DataLoader configuration dictionary
reader : dict, optional
    Reader configuration dictionary
writer : dict, optional
    Writer configuration dictionary

---
### FunctionDef: `initialize_log`

Initialize the output log for this driver process.

---
### FunctionDef: `initialize_manager`

Initialize an IOManager object given a configuration.

Parameters
----------
file_path : str
    Path to the input file

Returns
-------
larcv.IOManager
    IOManager object

---
### FunctionDef: `initialize_matplotlib`

Initialize the style parameters for matplotlib.

paper : bool, default False
    If `True`, format the figure for a paper, using latext style

---
### FunctionDef: `initialize_model`

Initializes the PPN-specific decoder.

---
### FunctionDef: `initialize_plotly`

Initialize the style parameters for plotly.

---
### FunctionDef: `initialize_train`

Initialize the training regimen.

Parameters
----------
optimizer : dict
    Configuration of the optimizer
weight_prefix : str, default 'snapshot'
    Path + name of the weight file prefix
save_step : int, default -1
    Number of iterations before recording the model weights (-1: never)
restore_optimizer : bool, default False
    Whether to load the  opimizer state from the torch checkpoint
lr_scheduler : dict, optional
    Configuration of the learning rate scheduler

---
### FunctionDef: `initialize_writer`

Adds a CSV writer to the list of writers for this script.

Parameters
----------
name : str
    Name of the writer

---
### FunctionDef: `instantiate`

Instantiates a class based on a configuration dictionary and a list of
possible classes to chose from.

This function supports two YAML configuration structures
(parsed as a dictionary):

.. code-block:: yaml

    function:
      name: function_name
      kwarg_1: value_1
      kwarg_2: value_2
      ...

or

.. code-block:: yaml

    function:
      name: function_name
      args:
        value_1
        value_2
        ...
      kwargs:
        kwarg_1: value_1
        kwarg_2: value_2
        ...

The `name` field can have a different name, as long as it is specified.

Parameters
----------
module_dict : dict
    Dictionary which maps a class name onto an object class.
cfg : dict
    Configuration dictionary
alt_name : str, optional
    Key under which the class name can be specfied, beside 'name' itself
**kwargs : dict, optional
    Additional parameters to pass to the function

Returns
-------
object
    Instantiated object

---
### FunctionDef: `inter_cluster_distance`

Finds the inter-cluster distance between every pair of clusters within
each batch, returned as a block-diagonal matrix.

Parameters
----------
voxels : Union[np.ndarray, torch.Tensor]
    (N, D) Tensor of voxel coordinates
clusts : List[np.ndarray]
    (C) List of cluster indexes
counts : np.ndarray, optional
    (B) Number of clusters in each entry of the batch
method : str, default 'voxel'
    Either the closest voxel distance ('voxel') of the cluster centroid
    distance ('centroid')
algorithm : str, default 'brute'
    Algorithm used to compute the 'voxel' distance. The 'brute' method
    is exact but slow, 'recursive' uses a fast but approximate method.
return_index : bool, default True
    Returns a combined index of the closest pair of voxels for each
    cluster, if the 'voxel' distance method is used

Returns
-------
Union[np.ndarray, torch.Tensor]
    (C, C) Tensor of pair-wise cluster distances
Union[np.ndarray, torch.Tensor], optional
    (C, C) Tensor of pair-wise closest voxel pair

---
### FunctionDef: `inter_cluster_loss`

Implementation of distance loss in Discriminative Loss.
Inputs:
    cluster_means (torch.Tensor): output from find_cluster_means
    margin (float/int): the magnitude of the margin delta_d in the paper.
    Think of it as the distance between each separate clusters in
    embedding space.
Returns:
    inter_loss (float): computed cross-centroid distance loss (see paper).
    Factor of 2 is included for proper normalization.

---
### FunctionDef: `inter_cluster_loss`

Implementation of distance loss in Discriminative Loss.
Inputs:
    cluster_means (torch.Tensor): output from find_cluster_means
    margin (float/int): the magnitude of the margin delta_d in the paper.
    Think of it as the distance between each separate clusters in
    embedding space.
Returns:
    inter_loss (float): computed cross-centroid distance loss (see paper).
    Factor of 2 is included for proper normalization.

---
### FunctionDef: `inter_cluster_loss`

Implementation of distance loss in Discriminative Loss.
Inputs:
    cluster_means (torch.Tensor): output from find_cluster_means
    margin (float/int): the magnitude of the margin delta_d in the paper.
    Think of it as the distance between each separate clusters in
    embedding space.
Returns:
    inter_loss (float): computed cross-centroid distance loss (see paper).
    Factor of 2 is included for proper normalization.

---
### ClassDef: `InteractionBase`

Base interaction-specific information.

Attributes
----------
particles : List[object]
    List of particles that make up the interaction
primary_particles: List[object]
    List of primary particles associated with the interaction
particle_ids : np.ndarray
    List of Particle IDs that make up this interaction
primary_particle_ids : np.ndarray
    List of primary Particle IDs associated with this interaction
num_particles : int
    Number of particles that make up this interaction
num_primary_particles : int
    Number of primary particles associated with this interaction
particle_counts : np.ndarray
    (P) Number of particles of each species in this interaction
primary_particle_counts : np.ndarray
    (P) Number of primary particles of each species in this interaction
vertex : np.ndarray
    (3) Coordinates of the interaction vertex
is_fiducial : bool
    Whether this interaction vertex is inside the fiducial volume
is_flash_matched : bool
    True if the interaction was matched to an optical flash
flash_ids : np.ndarray
    (F) Indices of the optical flashes the interaction is matched to
flash_volume_ids : np.ndarray
    (F) Indices of the optical volumes the flashes where recorded in
flash_times : np.ndarray
    (F) Times at which the flashes occurred in microseconds
flash_scores : np.ndarray
    (F) Flash matching quality scores reported for each match
flash_total_pe : float
    Total number of photoelectrons associated with the flash
flash_hypo_pe : float
    Total number of photoelectrons expected to be produced by the interaction
topology : str
    String representing the interaction topology

---
### ClassDef: `InteractionBuilder`

Builds reconstructed and truth interactions.

It takes the raw output of the reconstruction chain, extracts the
necessary information and builds :class:`RecoInteraction` and
:class:`TruthInteraction` objects from it.

---
### ClassDef: `InteractionTopologyProcessor`

Adjust the topology of interactions by applying thresholds on the
minimum kinetic energy of particles.

---
### FunctionDef: `intra_cluster_loss`

Computes the intra-cluster loss between an embedding point cloud and
a set of attractor points.

<labels> must range between 0 to the number of <cluster_means>, otherwise
the loss will be underestimated as <scatter_mean> zero value placeholders.

---
### FunctionDef: `intra_cluster_loss`

Implementation of variance loss in Discriminative Loss.
Inputs:
    features (torch.Tensor): pixel embedding, same as in find_cluster_means.
    labels (torch.Tensor): ground truth instance labels
    cluster_means (torch.Tensor): output from find_cluster_means
    margin (float/int): constant used to specify delta_v in paper. Think of it
    as the size of each clusters in embedding space.
Returns:
    intra_loss: (float) variance loss (see paper).

---
### FunctionDef: `inv_bethe_bloch_lar`

Inverse Bethe-Bloch energy loss function for liquid argon.

Parameters
----------
T : float
   Kinetic energy in MeV
M : float
   Impinging particle mass in MeV/c^2
z : int, default 1
   Impinging partile charge in multiples of electron charge

Returns
-------
float
   Value of the inverse energy loss rate in liquid argon in MeV/cm

---
### FunctionDef: `inv_birks`

Inverse Birks equation to undo electron quenching (higher local
energy deposition are prone to more electron-ion recombination).

Parameters
----------
dqdx : Union[float, np.ndarray]
    Value or array of values of dQ/dx in electrons/cm

Returns
-------
Union[float, np.ndarray]
    Inverse quenching factors in MeV/electrons

---
### FunctionDef: `inv_mbox`

Inverse modified box model equation to undo electron quenching
(higher local energy deposition are prone to more electron-ion
recombination).

Parameters
----------
dqdx : Union[float, np.ndarray]
    Value or array of values of dQ/dx in electrons/cm
cosphi : Union[float, np.ndarray]
    Value or array of values of the cosine of the angle w.r.t. the
    drift direction (in [0,1]).

Returns
-------
Union[float, np.ndarray]
    Inverse quenching factors in MeV/electrons

---
### FunctionDef: `inv_recombination_factor`

Calls the predefined inverse recombination models to evaluate the
appropriate correction factors.

Parameters
----------
dqdx : Union[float, np.ndarray]
    Value or array of values of dQ/dx in electrons/cm
cosphi : Union[float, np.ndarray]
    Value or array of values of the cosine of the angle w.r.t. the
    drift direction (in [0,1]).

Returns
-------
Union[float, np.ndarray]
    Inverse quenching factors in MeV/electrons

---
### FunctionDef: `iou`

Array of IoU for each (non ignored) class

---
### FunctionDef: `iou_batch`

pred: N x C
labels: N x C (one-hot)

---
### FunctionDef: `iou_binary`

IoU for foreground class
binary: 1 foreground, 0 background

---
### ClassDef: `IoUScore`

Intersection over union score for binary predictions.

---
### FunctionDef: `items`

Get the list of all initialized stopwatch tags and the
corresponding Stopwatch object for each of them.

Returns
-------
List[Tuple[str, Stopwatch]]
    List of (key, stopwatch) pairs

---
### FunctionDef: `ke`

Best-guess kinetic energy in MeV.

Uses calorimetry for EM activity and this order for track:
- CSDA-based estimate if it is available
- MCS-based estimate if it is available
- Calorimetry if all else fails

Returns
-------
float
    Best-guess kinetic energy

---
### FunctionDef: `ke`

Converts the particle initial energy to a kinetic energy.

This only works for particles with a known mass (as defined in
`spine.utils.globals`).

Returns
-------
float
    Initial kinetic energy of the particle

---
### FunctionDef: `kernel_factory`

Instantiates an edge kernel from a configuration dictionary.

Parameters
----------
cfg : dict
    Kernel configuration

Returns
-------
object
    Instantiated kernel function

---
### FunctionDef: `keys`

Converts a dictionary of keys to an immutable tuple.

Parameters
----------
Dict[str, bool]
    Dictionary of (key, necessity) pairs to be used

---
### FunctionDef: `keys`

Dictionary of (key, necessity) pairs which determine which data keys
are needed/optional for the post-processor to run.

Returns
-------
Dict[str, bool]
    Dictionary of (key, necessity) pairs to be used

---
### FunctionDef: `keys`

Dictionary of (key, necessity) pairs which determine which data keys
are needed/optional for the post-processor to run.

Returns
-------
Dict[str, bool]
    Dictionary of (key, necessity) pairs to be used

---
### FunctionDef: `keys`

Get the list of all initialized stopwatch tags.

Returns
-------
List[str]
    List of stopwatch names

---
### FunctionDef: `knn_sklearn`

Create a kNN graph using `scikit-learn`.

Parameters
----------
coords : Union[np.ndarray, torch.Tensor]
    (N, 3) Set of point coordinates
k : int
    Number of neighbors in the kNN graph

Returns
-------
Union[np.ndarray, torch.Tensor]
    (2, E) Edge index

---
### ClassDef: `KNNGraph`

Generates graphs based on the k nearest-neighbor (kNN) graph of the
input node locations.

Makes an edge for each nearest neighbor connection.

See :class:`GraphBase` for attributes/methods shared
across all graph constructors.

---
### FunctionDef: `label_cols`

Dictionary of (key, column_id) pairs which determine which column
in the label tensor corresponds to a specific clustering target.

Returns
-------
Dict[str, int]
    Dictionary of (key, column_id) mapping from name to label column

---
### ClassDef: `LArCVDataset`

A generic interface for LArCV data files.

This Dataset is designed to produce a batch of arbitrary number of data
chunks (e.g. input data matrix, segmentation label, point proposal target,
clustering labels, etc.). Each data chunk is processed by parser functions
defined in the io.parsers module. LArCVDataset object can be
configured with arbitrary number of parser functions where each function
can take arbitrary number of LArCV event data objects. The assumption is
that each data chunk respects the LArCV event boundary.

This class utilizes the :class:`LArCVReader` class. It uses it to
load data and to push it through the parsers.

---
### ClassDef: `LArCVReader`

Class which reads information stored in LArCV files.

This class inherits from the :class:`ReaderBase` class. It provides
methods to load LArCV2 files and extract their data products:
  - EventSparseTensor: voxel IDs and their values
  - EventClusterSparseTensor: list of sparse tensors
  - EventParticle: list of Geant4 particle information
  - EventNeutrino: list of generstor neutrino information
  - EventFlash: list of optical flashes information
  - EventCRTHit: list of cosmic-ray tagger hits
  - EventTrigger: trigger information

It builds a TChain from the list of files provided with the appropriate
trees corresponding to each of the requested data products.

---
### FunctionDef: `layout3d`

Produces plotly.graph_objs.Layout object for a certain format.

Parameters
----------
ranges : np.ndarray, optional
    (3, 2) or (N, 3) Array used to specify the plot region in (x,y,z)
    directions. If not specified (None), the range will be set to include
    all points. Alternatively can be an array of shape (3,2) specifying
    (x,y,z) axis (min,max) range for a display, or simply a list of points
    with shape (N,3+) where [:,0],[:,1],[:,2] correspond to (x,y,z) values
    and the plotting region is decided by measuring the min,max range in
    each coordinates. This last option is useful if one wants to define
    the region based on a set of points that is not same as what's plotted.
meta : Meta, optional
    Metadata information used to infer the full image range
detector : str
    Name of a recognized detector to get the geometry from
titles : List[str], optional
    (3) Array of strings for (x,y,z) axis title respectively
detector_coords : bool, default False
    Whether or not the coordinates being drawn are in detector_coordinates
    or pixel IDs
backgroundcolor : Union[str, int], default 'white'
    Color of the layout background
gridcolor : Union[str, int], default 'lightgray'
    Color of the grid
width : int, default 900
    Width of the layout in pixels
height : int, default 900
    Height of the layout in pixels
showlegend : bool, default True
    Whether or not to show the image legend
aspectmode : str, default manual
    Plotly aspect mode. If manual, will define it based on the ranges
aspectratio : dict, optional
    Plotly dictionary which specifies the aspect ratio for x, y an d z
dark : bool, default False
    Dark layout
margin : dict, optional
    Specifies the margin in each subplot
hoverlabel : dict, optional
    Specifies the style hovertext labels
**kwargs : dict, optional
    List of additional arguments to pass to plotly.graph_objs.Layout

Results
-------
plotly.graph_objs.Layout
    Object that can be given to plotly.graph_objs.Figure for visualization
    (together with traces)

---
### FunctionDef: `le_corr_lar`

Low energy corrections to the Bethe-Bloch formula.

Parameters
----------
beta : float
    Lorentz beta (v/c)
z : int, default 1
    Impinging partile charge in multiples of electron charge

Returns
-------
float
    Low energy correction to the energy loss function

---
### ClassDef: `LifetimeCalibrator`

Applies a correction based on drift electron lifetime and the distance
from the ionization point to the closest readout plane.

---
### ClassDef: `LikelihoodFlashMatcher`

Interface class between full chain outputs and OpT0Finder

See https://github.com/drinkingkazu/OpT0Finder for more details about it.

---
### FunctionDef: `list_data`

Dumps top-level information about the contents of a LArCV root file.

Parameters
----------
file_path : str
    Path to the file to scan

Returns
-------
dict
    Dictionary which maps data types onto a list of keys

---
### FunctionDef: `list_data`

Dumps top-level information about the contents of the LArCV root
file.

Parameters
----------
file_path : str
    Path to the file to scan

Returns
-------
dict
    Dictionary which maps data types onto a list of keys

---
### FunctionDef: `lite_skip_attrs`

Fetches the list of attributes to not store to lite file.

Returns
-------
List[str]
    List of attributes to exclude from the storage process

---
### FunctionDef: `load`

Loads one batch/entry to process.

If the model is run on the fly, the data is batched. Otherwise,
a single entry is loaded at this stage.

Parameters
----------
entry : int, optional
    Entry number, only valid with reader
run : int, optional
    Run number, only valid with reader
subrun : int, optional
    Subrun number to load
event : int, optional
    Event number, only valid with reader

Returns
-------
data: dict
    Data dictionary containing the input

---
### FunctionDef: `load_config`

Load a configuration file to a dictionary.

Parameters
----------
cfg_path : str
    Path to the configuration file

---
### FunctionDef: `load_key`

Fetch a specific key for a specific event.

Parameters
----------
in_file : h5py.File
    HDF5 file instance
event : dict
    Dictionary of objects that make up one event
data : dict
    Dictionary of data products corresponding to one event
key: str
    Name of the dataset in the entry

---
### FunctionDef: `load_match_pairs`

Generate lists of matched object pairs from stored matches.

Parameters
----------
data : dict
    Dictionary of input data and model outputs
name : str
    Object type name
entry : int, optional
    Entry number

---
### FunctionDef: `load_reco`

Construct :class:`RecoParticle` objects from their stored versions.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `load_reco`

Load :class:`RecoFragment` objects from their stored versions.

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
List[RecoFragment]
    List of restored reconstructed fragment instances

---
### FunctionDef: `load_reco`

Load :class:`RecoInteraction` objects from their stored versions.

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
List[RecoInteraction]
    List of restored reconstructed interaction instances

---
### FunctionDef: `load_reco`

Place-holder for a method used to load reconstructed objects.

Parameters
----------
data : dict
    Dictionary which contains the necessary data products

---
### FunctionDef: `load_tables`

Loads one look-up table per TPC.

Parameters
----------
df_run : pd.DataFrame
    Dataframe which corresponds to the run being loaded
quantity : str
    Name of the quantity to load for each bin

Returns
-------
np.ndarray
    (N_tpc) Array of calibration look-up tables

---
### FunctionDef: `load_truth`

Construct :class:`TruthParticle` objects from their stored versions.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `load_truth`

Load :class:`TruthFragment` objects from their stored versions.

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
List[TruthFragment]
    List of restored true fragment instances

---
### FunctionDef: `load_truth`

Load :class:`TruthInteraction` objects from their stored versions.

Parameters
----------
data : dict
    Dictionary of data products

Returns
-------
List[TruthInteraction]
    List of restored truth interaction instances

---
### FunctionDef: `load_truth`

Place-holder for a method used to load truth objects.

Parameters
----------
data : dict
    Dictionary which contains the necessary data products

---
### FunctionDef: `load_values`

Loads one value per TPC.

Parameters
----------
df_run : pd.DataFrame
    Dataframe which corresponds to the run being loaded
quantity : str
    Name of the quantity to load

Returns
-------
np.ndarray
    (N_tpc) Array of calibration values

---
### FunctionDef: `load_weights`

Load the weights of certain model components.

Breadth-first search for `weight_path` parameters in the model
configuration. If 'weight_path' is found under a module block,
the weights are loaded for its parameters.

If a `weight_path` is not found for a given module, load the overall
weights from `weight_path` under `trainval` for that module instead.

Parameters
----------
full_weight_path : str
    Path to the weights for the full model

---
### FunctionDef: `loader_factory`

Instantiates a DataLoader based on configuration.

Dataset comes from `dataset_factory`.

Parameters
----------
dataset : dict
    Dataset configuration dictionary
dtype : str
    Data type to cast the input data to
batch_size : int, optional
    Number of data samples to load per iteration
minibatch_size : int, optional
    Number of data samples to load per iteration, per process
num_workers : bool, default 0
    Number of CPU cores to use to load data. If 0, the process which
    runs the model will also load the data.
shuffle : bool, default True
    If True, shuffle the dataset entries
sampler : str, optional
    Name of the function used to sample data into batches
collate_fn : dict, optional
    Dictionary of collate function and collate parameters, if any
entry_list : list, optional
    List of entry numbers to include in the dataset
distributed : bool, default False
    If True, the loader will be prepared for distributed execution
world_size : int, default 1
    Total number of GPUs using the sampler
rank : int, default 0
    Unique identifier of the process sampling data

Returns
-------
torch.utils.data.DataLoader
    Initialized dataloader

---
### FunctionDef: `local_cdist`

Computes the pairwise distances between two `torch.Tensor` objects.

This is necessary because the torch.cdist implementation is either
slower (with the `donot_use_mm_for_euclid_dist` option) or produces
dramatically wrong answers under certain situations (with the
`use_mm_for_euclid_dist_if_necessary` option).

Parameters
----------
v1 : torch.Tensor
    (N, D) tensor of coordinates
v2 : torch.Tensor
    (M, D) tensor of coordinates

Returns
-------
torch.Tensor
    (N, M) tensor of pairwise distances

---
### FunctionDef: `log`

Log relevant information to CSV files and stdout.

Parameters
----------
data : dict
    Dictionary of data products to extract scalars from
tstamp : str
    Time when this iteration was run
iteration : int
    Iteration counter
epoch : float
    Progress in the training process in number of epochs

---
### FunctionDef: `log_dice_loss_flat`

Parameters
----------
logits: (N x num_queries)
targets: (N x num_queries)

---
### FunctionDef: `log_loss`

Numba implementation of cross-entropy loss.

Parameters
----------
label : np.ndarray
    (N) array of boolean labels (0 or 1)
pred : np.ndarray
    (N) array of float scores (between 0 and 1)

Returns
-------
float
    Cross-entropy loss

---
### ClassDef: `LogRMSE`

Applies RMSE loss to in the log space for regression tasks.

---
### ClassDef: `LoopGraph`

Generates loop-only graphs.

Connects every node in the graph with itself but nothing else.

See :class:`GraphBase` for attributes/methods shared
across all graph constructors.

---
### FunctionDef: `loss_factory`

Instantiates a clustering loss from a configuration dictionary.

Parameters
----------
cfg : dict
    Clustering loss configuration

Returns
-------
object
    Instantiated clustering loss function

---
### FunctionDef: `loss_fn_factory`

Instantiates a loss function from a configuration dictionary.

Parameters
----------
cfg : dict
    Final layer configuration
functional : bool, default False
    Whether to return the loss function as a functional
**kwargs : dict, optional
    Additional parameters to pass to the loss function

Returns
-------
object
    Instantiated loss function

---
### FunctionDef: `lovasz_grad`

Computes gradient of the Lovasz extension w.r.t sorted errors
See Alg. 1 in paper

---
### FunctionDef: `lovasz_hinge`

Binary Lovasz hinge loss
  logits: [B, H, W] Variable, logits at each pixel (between -\infty and +\infty)
  labels: [B, H, W] Tensor, binary ground truth masks (0 or 1)
  per_image: compute the loss per image instead of per batch
  ignore: void class id

---
### FunctionDef: `lovasz_hinge_flat`

Binary Lovasz hinge loss
  logits: [P] Variable, logits at each prediction (between -\infty and +\infty)
  labels: [P] Tensor, binary ground truth labels (0 or 1)
  ignore: label to ignore

---
### FunctionDef: `lovasz_softmax`

Multi-class Lovasz-Softmax loss
  probas: [B, C, H, W] Variable, class probabilities at each prediction (between 0 and 1).
          Interpreted as binary (sigmoid) output with outputs of size [B, H, W].
  labels: [B, H, W] Tensor, ground truth labels (between 0 and C - 1)
  classes: 'all' for all, 'present' for classes present in labels, or a list of classes to average.
  per_image: compute the loss per image instead of per batch
  ignore: void class labels

---
### FunctionDef: `lovasz_softmax_flat`

Multi-class Lovasz-Softmax loss
  probas: [P, C] Variable, class probabilities at each prediction (between 0 and 1)
  labels: [P] Tensor, ground truth labels (between 0 and C - 1)
  classes: 'all' for all, 'present' for classes present in labels, or a list of classes to average.

---
### FunctionDef: `lower`

Lower bounds of the box.

Returns
-------
np.ndarray
    Lower bounds of the box

---
### FunctionDef: `lr_sched_factory`

Instantiates a learning-rate scheduler from a configuration dictionary.

Parameters
----------
cfg : dict
    Learning-rate scheduler configuration
optimizer : object
    Torch optimizer instance

Returns
-------
object
    Instantiated learning-rate optimizer

---
### FunctionDef: `main`

Checks the number of entries in a file/list of files.

Parameters
----------
source : Union[str, List[str]]
    Path or list of paths to the input files
source_list : str
    Path to a text file containing a list of data file paths
tree_name : str
    Name of the tree to use as a reference to count the number of entries.
    If not specified, takes the first tree in the list.

---
### FunctionDef: `main`

Checks the output of the SPINE process.

The script loops over the input files, check that there is an output file
in the expected location and further checks that the output file entry
count matches that of the input file.

Produces a list of input files that have no or incomplete output in a text
file (the name of which is provided with the `-o` or `--output` flag). This
can be used to reprocess missing/incomplete input files.

.. code-block:: bash

    $ python3 bin/output_check_valid.py -S file_list.txt -o missing.txt
      --dest /path/to/output/files/ --suffix output_file_suffix

Parameters
----------
source : List[str]
    List of paths to the input files
source_list : str
    Path to a text file containing a list of data file paths
output : str
    Path to the output text file with the list of badly processed files
dest : str
    Destination directory for the original SPINE process
suffix : str
    Suffix added to the end of the input files by the original SPINE process
event_list : str
    Path to a file containing a list of events to process. If provided, only
    events which appear on this list are required for in the output.
tree_name : str
    Name of the tree to use as a reference to count the number of entries.
    If not specified, takes the first tree in the list.
larcv_output, bool
    If `True`, the output file is also a ROOT file

---
### FunctionDef: `main`

Checks the output of the SPINE process.

The script loops over the input files, fetch the list of keys in the file
and injects a run number of each event in each file.

.. code-block:: bash

    $ python3 bin/inject_run_number.py -S file_list.txt
      --overwrite --run_number 123

Parameters
----------
source : List[str]
    List of paths to the input files
source_list : str
    Path to a text file containing a list of data file paths
dest : str
    Destination folder to write the files to
overwrite : bool
    If `True`, overwrite the original files
run_number : int
    Run number to inject in the input file list. If it is specied as -1,
    each file is assigned a unique run number
suffix : str
    String to append to the end of the input file names to form the name
    of the output file with the updated run numbers

---
### FunctionDef: `main`

Checks the validity of a LArCV root file.

This script loops over all TTrees in a given ROOT file and check that they
have the same, non-zero, number of entries.

Produces a list of bad files in 'bad_files.txt' (one per line) that can then
be used to move/remove these bad files before doing hadd. For example using:

.. code-block:: bash

    $ for file in $(cat bad_files.txt); do mv "$file" bad_files/; done

Parameters
----------
source : List[str]
    List of paths to the input files
source_list : str
    Path to a text file containing a list of data file paths
output : str
    Path to the output text file with the list of bad files

---
### FunctionDef: `main`

Loops over a list of files and finds those which belong to a certain run.

Parameters
----------
source : Union[str, List[str]]
    Path or list of paths to the input files
source_list : str
    Path to a text file containing a list of data file paths
output : str
    Path to the output text file with the list of run files
run_number : int
    Run number to look for
tree_name : str
    Name of the tree to use as a reference to get the run number from.
    If not specified, takes the first tree in the list.

---
### FunctionDef: `main`

Loops over a list of files and identifies files which contain the same
set of (run, subrun, event) triplets.

In order to save time, this script only checks if:
1. The number of entries in the files are the same
2. The run, subrun and event numbers in the first entry are the same

Parameters
----------
source : Union[str, List[str]]
    Path or list of paths to the input files
source_list : str
    Path to a text file containing a list of data file paths
output : str
    Path to the output text file with the list of duplicates
tree_name : str
    Name of the tree to use as a reference to count the number of entries.
    If not specified, takes the first tree in the list.

---
### FunctionDef: `main`

Main driver for training/validation/inference/analysis.

Performs these basic functions:
- Update the configuration with the command-line arguments
- Run the appropriate piece of code

Parameters
----------
config : str
    Path to the configuration file
source : List[str]
    List of paths to the input files
source_list : str
    Path to a text file containing a list of data file paths
output : str
    Path to the output file
n : int
    Number of iterations to run
nskip : int
    Number of iterations to skip
detect_anomaly : bool
    Whether to turn on anomaly detection in torch
log_dir : str
    Path to the directory for storing the training log
weight_prefix : str
    Path to the directory for storing the training weights
weight_path : str
    Path string a weight file or pattern for multiple weight files to load
    the model weights

---
### FunctionDef: `make_config`

Use hyperparameter search domain specification dictionary to
prepare new training config with model/optimizer hyperparameters
changed accordingly.

---
### FunctionDef: `make_crthit`

Parameters
==========
larcv_crthits: list of list of larcv::CRTHit

Returns
=======
list of matcha:CRTHit

---
### FunctionDef: `make_flash_list`

Creates a list of flashmatch.Flash_t from the local class.

Parameters
----------
flashes : List[Flash]
    List of optical flashes

Returns
-------
List[Flash_t]
    List of flashmatch::Flash_t objects

---
### FunctionDef: `make_qcluster_list`

Converts a list of SPINE interaction into a list of OpT0Finder
flashmatch.QCluster_t objects.

Parameters
----------
interactions : List[Union[Interaction, TruthInteraction]]
    List of TPC interactions

Returns
-------
List[QCluster_t]
   List of OpT0Finder flashmatch::QCluster_t objects

---
### ClassDef: `Mask3dLoss`

Loss function for GraphSpice.

Configuration
-------------
name: str, default 'se_lovasz_inter'
    Loss function to use.
invert: bool, default True
    You want to leave this to True for statistical weighting purpose.
kernel_lossfn: str
edge_loss_cfg: dict
    For example

    .. code-block:: yaml

      edge_loss_cfg:
        loss_type: 'LogDice'

eval: bool, default False
    Whether we are in inference mode or not.

    .. warning::

        Currently you need to manually switch ``eval`` to ``True``
        when you want to run the inference, as there is no way (?)
        to know from within the loss function whether we are training
        or not.

Output
------
To be completed.

See Also
--------
MinkGraphSPICE

---
### ClassDef: `Mask3DModel`

Transformer-Instance Query based particle clustering

Configuration
-------------
skip_classes: list, default [2, 3, 4]
    semantic labels for which to skip voxel clustering
    (ex. Michel, Delta, and Low Es rarely require neural network clustering)
dimension: int, default 3
    Spatial dimension (2 or 3).
min_points: int, default 0
    If a value > 0 is specified, this will enable the orphans assignment for
    any predicted cluster with voxel count < min_points.

---
### FunctionDef: `mask_module`

Inputs
------
    - queries: [B, num_queries, query_dim] torch.Tensor
    - mask_features: ME.SparseTensor from mask head output

---
### ClassDef: `MaskBCELoss`

Loss function for Sparse Spatial Embeddings Model, with fixed
centroids and symmetric gaussian kernels.

---
### ClassDef: `MaskBCELoss2`

Spatial Embeddings Loss with trainable center of attention.

---
### ClassDef: `MaskBCELossBivariate`

Spatial Embeddings Loss with trainable center of attraction and
bivariate gaussian probability kernels.

---
### ClassDef: `MaskFocalLoss`

Spatial Embeddings Loss with trainable center of attention.

---
### ClassDef: `MaskLovaszHingeLoss`

Spatial Embeddings Loss using Lovasz Hinge for foreground/background
segmentation and trainable center of attention.

---
### FunctionDef: `mass`

Computes the rest mass of the particle from its energy/momentum.

Returns
-------
float
    Rest mass of the particle in MeV/c^2

---
### FunctionDef: `mass`

Rest mass of the particle in MeV/c^2.

The mass is inferred from the predicted mass.

Returns
-------
float
    Rest mass of the particle

---
### ClassDef: `Matcher`

Simple data class to store matching methods per object.

Attributes
----------
fn : function
    Function which computes overlaps between pairs of objects
match_mode : str, defualt 'both'
    Matching mode. One of 'reco_to_truth', 'truth_to_reco' or 'both'
overlap_mode : str, default 'iou'
    Overlap estimatation method. One of 'count', 'iou', 'dice', 'chamfer'
min_overlap : float, default 0.
    Overlap value above which a pair is considered a match
weight_overlap : bool, default False
    Whether to weight the overlap metric
ghost : bool, default False
    Whether a deghosting process was applied (in which case the indexes
    of the reco and the truth particles do not align)

---
### ClassDef: `MatchProcessor`

Does the matching between reconstructed and true objects.

---
### ClassDef: `MB3Encoder`

Vanilla UResNet with access to intermediate feature planes.

Configurations
--------------
depth : int
    Depth of UResNet, also corresponds to how many times we down/upsample.
num_filters : int
    Number of filters in the first convolution of UResNet.
    Will increase linearly with depth.
reps : int, optional
    Convolution block repetition factor
kernel_size : int, optional
    Kernel size for the SC (sparse convolutions for down/upsample).
input_kernel : int, optional
    Receptive field size for very first convolution after input layer.

---
### ClassDef: `MBConv`

MBConv block.

---
### FunctionDef: `mbox`

Modified box model equation to calculate electron quenching (higher
local energy deposition are prone to more electron-ion recombination).

Parameters
----------
dedx : Union[float, np.ndarray]
    Value or array of values of dE/dx in MeV/cm
cosphi : Union[float, np.ndarray]
    Value or array of values of the cosine of the angle w.r.t. the
    drift direction (in [0,1]).

Returns
-------
Union[float, np.ndarray]
    Quenching factors in electrons/MeV

---
### ClassDef: `MBResConv`

MBResConv block.

---
### ClassDef: `MBResConvSE`

MBResConvSE block.

---
### FunctionDef: `mc_forward`

Forwarding operation for MC Dropout segmentation network.

Args:
    num_samples: number of stochastic forward samples to be taken

---
### ClassDef: `MCDropoutDecoder`

Convolutional decoder with dropout layers.

The architecture is exactly the same as the ME ResidualEncoders,
except for the additional DropoutBlocks

Attributes:

    dropout_p: dropping probability value for dropout layers
    dropout_layer_index: layer numbers to swap resnet blocks with
    dropout resnet blocks.

---
### ClassDef: `MCDropoutEncoder`

Convolutional decoder with dropout layers.

The architecture is exactly the same as the ME ResidualEncoders,
except for the additional DropoutBlocks

Attributes:

    dropout_p: dropping probability value for dropout layers
    dropout_layer_index: layer numbers to swap resnet blocks with
    dropout resnet blocks.

---
### FunctionDef: `mcs_fit`

Finds the kinetic energy which best fits a set of scattering angles
measured between successive segments along a particle track.

Parameters
----------
theta : np.ndarray
    (N) Vector of scattering angle at each step in radians
M : float
    Particle mass in MeV/c^2
dx : float
    Step length in cm
z : int, default 1
    Impinging partile charge in multiples of electron charge
split_angle : bool, default False
    Whether or not to project the 3D angle onto two 2D planes
res_a : float, default 0.25 rad*cm^res_b
    Parameter a in the a/dx^b which models the angular uncertainty
res_b : float, default 1.25
    Parameter b in the a/dx^b which models the angular uncertainty

---
### FunctionDef: `mcs_nll_lar`

Computes the MCS negative log likelihood for a given list of segment angles
and an initial momentum. This function checks the agreement between the
scattering expection and the observed scattering at each step.

Parameters
----------
T0 : float
    Candidate particle kinetic energy in MeV
theta : np.ndarray
    (N) Vector of scattering angle at each step in radians
M : float
    Particle mass in MeV/c^2
dx : float
    Step length in cm
z : int, default 1
   Impinging partile charge in multiples of electron charge
split_angle : bool, default False
    Whether or not to project the 3D angle onto two 2D planes
res_a : float, default 0.25 rad*cm^res_b
    Parameter a in the a/dx^b which models the angular uncertainty
res_b : float, default 1.25
    Parameter b in the a/dx^b which models the angular uncertainty

---
### ClassDef: `MCSEnergyProcessor`

Reconstruct the kinetic energy of tracks based on their Multiple-Coulomb
scattering (MCS) angles while passing through liquid argon.

---
### ClassDef: `MCTSNode`

Node class for Monte Carlo Tree Search in SubgraphX.

Attributes:
    - graph: the (sub)graph representing the MCTS node
    - actions: the set of all actions that can be taken at this MCTS node.
    - W: 

---
### FunctionDef: `mean`

Numba implementation of `np.mean(x, axis)`.

Parameters
----------
x : np.ndarray
    (N,M) array of values
axis : int
    Array axis ID

Returns
-------
np.ndarray
    (N) or (M) array of `mean` values

---
### FunctionDef: `mean`

nanmean compatible with generators.

---
### FunctionDef: `merge`

Merge another particle instance into this one.

This method can only merge two track objects with well defined start
and end points.

Parameters
----------
other : RecoParticle
    Other reconstructed particle to merge into this one

---
### FunctionDef: `merge`

Merge this index batch with another.

Parameters
----------
index_batch : IndexBatch
    Other index batch object to merge with

Returns
-------
IndexBatch
    Merged index batch

---
### FunctionDef: `merge`

Merge this tensor batch with another.

Parameters
----------
tensor_batch : TensorBatch
    Other tensor batch object to merge with

Returns
-------
TensorBatch
    Merged tensor batch

---
### FunctionDef: `merge_track_to_shower`

Merge a track p2 into shower p1.

Parameters
----------
p1 : RecoParticle
    Shower particle to merge p1 into.
p2 : RecoParticle
    Track particle p2 that will be merged into p1.

---
### FunctionDef: `merge_volumes`

Given a list of volumes and their boundaries, find the smallest box
that encompass all volumes combined.

Parameters
----------
volumes : np.ndarray
    (N, 3, 2) List of volume boundaries

Returns
-------
np.ndarray
    (3, 2) Boundaries of the combined volume

---
### ClassDef: `MergeConcat`

Merge one sparse tensor with another.

---
### ClassDef: `Meta`

Meta information about a rasterized image.

Attributes
----------
lower : np.ndarray
    (2/3) Array of image lower bounds in detector coordinates (cm)
upper : np.ndarray
    (2/3) Array of image upper bounds in detector coordinates (cm)
size : np.ndarray
    (2/3) Array of pixel size in each dimension (cm)
count : np.ndarray
    (2/3) Array of pixel count in each dimension

---
### ClassDef: `MetaLayerGNN`

Completely generic message-passing GNN.

---
### ClassDef: `MetaLayerModelExplainer`

GNN Explainer reformatted to handle MetaLayerModels

This implementation is largely a copy from Pytorch Geometric:
https://pytorch-geometric.readthedocs.io/en/latest/_modules/torch_geometric/nn/models/gnn_explainer.html
© Copyright 2021, Matthias Fey. Revision 788a4c05.

This patchwork is only temporary. 

---
### ClassDef: `MetaParser`

Get the metadata information to translate into real world coordinates.

Each entry in a dataset is a cube, where pixel/voxel coordinates typically
go from 0 to some integer N in each dimension. If you wish to translate
these pixel/voxel coordinates back into real world coordinates, you can use
the output of this parser to compute it.

.. code-block. yaml

    schema:
      meta:
        parser: meta
        sparse_event: sparse3d_pcluster

---
### FunctionDef: `metric_fn_factory`

Instantiates a metric function from a configuration dictionary.

Parameters
----------
cfg : dict
    Metric function configuration

Returns
-------
object
    Instantiated metric function

---
### FunctionDef: `minimize_rr`

Find the residual range which minimises the chi2 fit between the
observed dE/dx values and the spline fit to the template.

Parameters
----------
dedxs : np.ndarray
    (S) Measured values of dedxs at a set of unknown residual ranges
rrs : np.ndarray
    (S) Residual ranges assuming the particle came to a complete stop
pid : int
    Particle species enumerator

Returns
-------
float
    Value of the residual range at the end of the track
float
    Value of the chi2 for the optimal residual range

---
### ClassDef: `MinkGhostMask`

Ghost mask downsampler.

Downsamples the ghost mask and prunes a tensor with current
ghost mask to obtain nonghost tensor and the new ghost mask.

---
### ClassDef: `MinkowskiAdaIN`

Adaptive Instance Normalization Layer.

Many parts of the code is borrowed from pytorch original
`BatchNorm` implementation.

Original paper: https://arxiv.org/pdf/1703.06868.pdf

---
### ClassDef: `MinkowskiMish`

Mish non-linearity layer.

Reference: https://arxiv.org/pdf/1908.08681.pdf

---
### ClassDef: `MinkowskiPixelNorm`

Pixel Normalization Layer for Sparse Tensors.

PixelNorm layers were used in NVIDIA's ProGAN.

This layer normalizes the feature vector in each
pixel to unit length, and has no trainable weights.

Original paper: https://arxiv.org/pdf/1710.10196.pdf

---
### ClassDef: `MixedKernel`

Kernel producing edge score based on feature L2 similarity and cosine
similarity between node features.

This Kernel assumes that the upstream embedder produces a set of spatial
and embedding coordinates and computes the L2 similarity between the two
node feature vectors. It scales the L2 distance by the covariance and
penalizes for cluster size dissimilarity.

In addition, it computes cosine similarity between the feature vectors.

---
### ClassDef: `MLP`

Generic multi-layer perceptron to be used as a feature extractor.

---
### ClassDef: `MLPEdgeLayer`

Model used to update the set of edge features.

For each edge, this model first aggregates the features from the source
node (N_c) with those of the sink node (N_c) and those of the edge (N_e)
and those of the graph (N_g) to form an input feature vector of dimension
(E, 2*N_c + N_e + N_g). This feature vector is then passed through a
multi-layer perceptron (MLP) and outputs an (E, N_o) vector, with N_o the
width of the MLP (feature size of the hidden representation).

---
### ClassDef: `MLPGlobalLayer`

Model used to update the set of global graph features.

For each graph (one per entry in the batch of B graphs), this model first
takes a summary statistic of the information from all the nodes in the
graph (N_c). It then aggregates this feature vector with the one associated
with the graph itself (N_g) to form a feature fector of dimension
(N_c + N_g). This feature vector is then passed through a multi-layer
perceptron (MLP) and outputs a (B, N_o) vector, with N_o the width of the
MLP (feature size of the hidden representation).

---
### ClassDef: `MLPKernel`

Kernel producing edges scores based on an MLP and a linear layer.

---
### ClassDef: `MLPNodeLayer`

Model used to update the set of node features.

For each node, this model proceeds in two seperate steps:
- A message formation step
- A message aggregation step

For each edge, the message formation step consists in first aggregating
the source node features (N_c) with the edge features (N_e) to form an
input feature vector of dimension (N_c + N_e). This feature vector is
then passed through a multi-layer perceptron (MLP) and outputs an (N_o)
vector, with N_o the width of the MLP (feature size of the hidden
representation). This feature vector is the message associated with that
edge.

For each node, the message aggregations step consists in taking a
summary statistic of all edge features which correspond to edges that have
that node as a sink. The so-formed feature vector of size (N_o) is then
stacked with the node features (N_c) and the global graph features (N_g)
to form a (N_o + N_c + N_g) feature vector. This new vector is passed
through a second MLP to update the node features to (N_o').

---
### ClassDef: `MobileNetV3`

Vanilla UResNet with access to intermediate feature planes.

Configurations
--------------
depth : int
    Depth of UResNet, also corresponds to how many times we down/upsample.
num_filters : int
    Number of filters in the first convolution of UResNet.
    Will increase linearly with depth.
reps : int, optional
    Convolution block repetition factor
kernel_size : int, optional
    Kernel size for the SC (sparse convolutions for down/upsample).
input_kernel : int, optional
    Receptive field size for very first convolution after input layer.

---
### FunctionDef: `model_dict`

Returns dictionary of model classes using name keys (strings).

Returns
-------
dict
    Dictionary of available models

---
### FunctionDef: `model_factory`

Returns an instance of a model class based on its name key (string).

Parameters
----------
name: str
    Key for the model. See source code for list of available models.

Returns
-------
object

---
### ClassDef: `ModelManager`

Groups all relevant functions to construct a model and its loss.

---
### FunctionDef: `modes`

Dictionary of (stage, modes) pairs which determine which options
are available to each of the the reconstruction stage.

Returns
-------
Dict[str, Tuple(str)]
    Dictionary of (stage, modes) pairs to be used

---
### FunctionDef: `modes`

Dictionary of (stage, modes) pairs which determine which options
are available to each of the the reconstruction stage.

Returns
-------
Dict[str, Tuple(str)]
    Dictionary of (stage, modes) pairs to be used

---
### ClassDef: `Module`

Class which holds all properties of a TPC module.

A module can hold either one chamber or two chambers with a shared cathode.

Attributes
----------
chambers : List[Chamber]
    List of individual TPCs that make up the module

---
### FunctionDef: `module_dict`

Converts module into a dictionary which maps class names onto classes.

Parameters
----------
module : module
    Module from which to fetch the classes
class_name : str, optional
    If specified, only allow aliases that match it
pattern : str, optional
    If specified, looks for a specific pattern in the class name

Returns
-------
dict
    Dictionary which maps acceptable class names to classes themselves

---
### FunctionDef: `module_ids`

List of modules that contribute to this object.

Returns
-------
np.ndarray
    List of unique modules contributing to this object.

---
### FunctionDef: `momentum`

Best-guess momentum in MeV/c.

Returns
-------
np.ndarray
    (3) Momentum vector

---
### ClassDef: `MSTGraph`

Generates graphs based on the minimum-spanning tree (MST) of the input
node locations.

Makes an edge for each branch in the minimum-spanning tree.

See :class:`GraphBase` for attributes/methods shared
across all graph constructors.

---
### FunctionDef: `network_schematic`

Network 2D schematic representation.

This is to be used exclusevely with bipartite graphs where the nodes
are either classified as primary or secondaries under clust_labels and
connections only exist between primaries and secondaries.

Parameters
----------
clusts : List[np.ndarray]
    (C) List of cluster indexes
edge_index : np.ndarray
    (E, 2) List of connections between clusters
clust_labels : np.ndarray
    (C) Whether a cluster is a primary or a secondary
edge_labels : np.ndarray, optional
    (E) List of edge labels
linewidth : float, default 2
    Width of the edge lines
color : Union[str, np.ndarray], optional
    Color of clusters or (C) list of color of clusters
name : str, optional
    Name of the network
linewidth : float, default 2
    Width of the edge lines
**kwargs : dict, optional
    List of additional arguments to pass to plotly

Returns
-------
List[plotly.graph_objs.Scatter]
    Node and edge traces in the same list

---
### FunctionDef: `network_topology`

Network 3D topological representation in Euclidean space.

Parameters
----------
points : np.ndarray
    (N, 3) array of N points of (..., x, y, z,...) coordinate information
clusts : List[np.ndarray]
    (C) List of cluster indexes
edge_index : np.ndarray
    (E, 2) List of connections between clusters
clust_labels : np.ndarray, optional
    (C) List of cluster labels
edge_labels : np.ndarray, optional
    (E) List of edge labels
mode : str, default 'scatter'
    Drawing mode; one of 'circle', 'scatter', 'ellipsoid', 'cone' or 'hull'
color : Union[str, np.ndarray], optional
    Color of clusters or (C) list of color of clusters
line : dict, optional
    Line property dictionary
linewidth : float, default 2
    Width of the edge lines
name : str, optional
    Name of the network
**kwargs : dict, optional
    List of additional arguments to pass to plotly

Returns
-------
List[Union[plotly.graph_objs.Scatter3d, plotly.graph_objs.Mesh3d]]
    Node and edge traces in the same list

---
### ClassDef: `Neutrino`

Neutrino truth information.

Attributes
----------
id : int
    Index of the neutrino in the list
interaction_id : int
    Index of the neutrino at the generator stage (e.g. Genie)
mct_index : int
    Index in the original MCTruth array from whence it came
track_id : int
    Geant4 track ID of the neutrino
lepton_track_id : int
    Geant4 track ID of the lepton (if CC)
pdg_code : int
    PDG code of the neutrino
lepton_pdg_code : int
    PDF code of the outgoing lepton
current_type : int
    Enumerated current type of the neutrino interaction
interaction_mode : int
    Enumerated neutrino interaction mode
interaction_type : int
    Enumerated neutrino interaction type
target : int
    PDG code of the target object
nucleon : int
    PDG code of the target nucleon (if QE)
quark : int
    PDG code of the target quark (if DIS)
energy_init : float
    Energy of the neutrino at its interaction point in GeV
hadronic_invariant_mass : float
    Hadronic invariant mass (W) in GeV/c^2
bjorken_x : float
    Bjorken scaling factor (x)
inelasticity : float
    Inelasticity (y)
momentum_transfer : float
    Squared momentum transfer (Q^2) in (GeV/c)^2
momentum_transfer_mag : float
    Magnitude of the momentum transfer (Q3) in GeV/c
energy_transfer : float
    Energy transfer (Q0) in GeV
lepton_p : float
    Absolute momentum of the lepton
distance_travel : float
    True amount of distance traveled by the neutrino before interacting
theta : float
    Angle between incoming and outgoing leptons in radians
t : float
    Interaction time (ns)
creation_process : str
    Creation process of the neutrino
position : np.ndarray
    Location of the neutrino interaction
momentum : np.ndarray
    3-momentum of the neutrino at its interaction point
units : str
    Units in which the position coordinates are expressed

---
### ClassDef: `NeutrinoParser`

Class which loads larcv.Neutrino objects to local Neutrino ones.

.. code-block. yaml

    schema:
      neutrinos:
        parser: neutrino
        neutrino_event: neutrino_mpv
        cluster_event: cluster3d_pcluster
        pixel_coordinates: True
        asis: False

---
### FunctionDef: `nll_evd_loss`

Negative log loss for Dirichlet prior evidential learning.

INPUTS:
    - alpha (FloatTensor): N x C concentration parameters, 
    where C is the number of class labels.
    - y (FloatTensor): N x C one-hot encoded class labels

RETURNS:
    - loss (FloatTensor): N x 1 non-reduced loss for each example. 

---
### FunctionDef: `nll_regression_loss`

Negative log loss for Dirichlet prior evidential learning.

INPUTS:
    - alpha (FloatTensor): N x C concentration parameters, 
    where C is the number of class labels.
    - y (FloatTensor): N x 1 regression targets

RETURNS:
    - loss (FloatTensor): N x 1 non-reduced loss for each example. 

---
### ClassDef: `NNConvNodeLayer`

NNConv module for extracting graph node features.

This model starts by passing the edge feature vectors (N_e) through a
multi-layer perceptron (MLP) and outputs a (N_c, N_o) matrix per edge. For
each edge connected to a specific node, this matrix is multiplied with the
source node features (N_c) to form an (N_o) feature per edge. These
messages are aggregated using a summary statistic. This aggregated message
is then added to the original node features, which have been updated by
a weight matrix to a feature vector of size (N_o).

Source: https://arxiv.org/abs/1704.02901

---
### FunctionDef: `node_assignment`

Assigns each node to a group, based on the edge assigment provided.

This uses the locally-defined union find implementation.

Parameters
----------
edge_index : np.ndarray
    (2, E) Sparse incidence matrix
edge_pred : np.ndarray
    (E, 2) Logits associated with each edge
num_nodes : int
    Number of nodes in the graph, C

Returns
-------
np.ndarray
    (C) Assigned node group IDs

---
### FunctionDef: `node_assignment_batch`

Batched version of :func:`node_assignment`.

Parameters
----------
edge_index : EdgeIndexBatch
    (2, E) Sparse incidence matrix
edge_pred : TensorBatch
    (E, 2) Logits associated with each edge
clusts : IndexBatch
    (C) List of cluster indexes

Returns
-------
    np.ndarray: (C) List of group ids

---
### FunctionDef: `node_assignment_bipartite`

Assigns each node to a group represented by a primary node.

This function loops over secondaries and associates it to the primary with
that is connected to it with the strongest edge.

Parameters
----------
edge_index : np.ndarray
    (2, E) Sparse incidence matrix
edge_pred : np.ndarray
    (E, 2) Logits associated with each edge
primaries : np.ndarray
    (P) List of primary IDs
num_nodes : int
    Number of nodes in the graph, C

Returns
-------
np.ndarray
    (C) Assigned node group IDs

---
### FunctionDef: `node_assignment_score`

Finds the graph that produces the lowest grouping score and use
union-find to find group IDs for each of the nodes in the graph.

Parameters
----------
edge_index : np.ndarray
    (2, E) Sparse incidence matrix
edge_pred : TensorBatch
    (E, 2) Logits associated with each edge
num_nodes : int
    Number of nodes in the graph, C
track_node : np.ndarray, optional
    (C) Whether a node is a track fragment/particle or not

Returns
-------
np.ndarray
    (C) Optimal group ID for each node

---
### FunctionDef: `node_assignment_score_batch`

Finds the graph that produces the lowest grouping score and use
union-find to find group IDs for each of the nodes in the graph.

Parameters
----------
edge_index : EdgeIndexBatch
    (2, E) Sparse incidence matrix
edge_pred : TensorBatch
    (E, 2) Logits associated with each edge
clusts : IndexBatch
    (C) List of cluster indexes
track_node : TensorBatch, optional
    (C) Whether a node is a track fragment/particle or not

Returns
-------
np.ndarray
    (C) Optimal group ID for each node

---
### FunctionDef: `node_encoder_factory`

Instantiates a node encoder from a configuration dictionary.

Parameters
----------
cfg : dict
    Node encoder configuration

Returns
-------
object
    Instantiated node encoder

---
### FunctionDef: `node_layer_factory`

Instantiates a GNN node update layer from a configuration dictionary.

Parameters
----------
cfg : dict
    GNN node update layer configuration
node_in : int
    Number of input node features
edge_in : int
    Number of input edge features
glob_in : int
    Number of input global graph features

Returns
-------
object
    Instantiated GNN node update layer

---
### FunctionDef: `node_loss_factory`

Instantiates a node loss from a configuration dictionary.

Parameters
----------
cfg : dict
    Node loss configuration

Returns
-------
object
    Instantiated node loss

---
### FunctionDef: `node_purity_mask`

Creates a mask that is `True` only for node which belong to a group
with more exactly one primary.

This is useful for shower clustering only, for which there can be no or
multiple primaries in the group, making the primary identification
ill-defined.

Note: It is possible that the single true primary has been broken into
several nodes. In that case, the primary is also ambiguous, skip. 
TODO: pick the most sensible primary in that case, too restrictive
otherwise (complicated, though).

Parameters
----------
group_ids : np.ndarray
    (C) Array of cluster group IDs
primary_ids : np.ndarray
    (C) Cluster of cluster primary IDs

Returns
-------
np.ndarray
    (C) High purity node mask

---
### FunctionDef: `node_purity_mask_batch`

Batched version of :func:`node_purity_mask`.

Parameters
----------
group_ids : TensorBatch
    (C) Array of cluster group IDs
primary_ids : TensorBatch
    (C) Cluster of cluster primary IDs

Returns
-------
np.ndarray
    (C) High purity node mask

---
### ClassDef: `NodeClassLoss`

Generic loss used to train node identification.

Takes the C-channel node output of the GNN and optimizes node-wise scores
such that the score corresponding to the correct class is maximized.

For use in config:

..  code-block:: yaml

    model:
      name: grappa
      modules:
        grappa_loss:
          node_loss:
            name: class
            <dictionary of arguments to pass to the loss>

See configuration files prefixed with `grappa_` under the `config`
directory for detailed examples of working configurations.

---
### ClassDef: `NodeEdgeLoss`

Combined Node + Edge Loss

---
### ClassDef: `NodeOrientLoss`

Loss to learn how to point a track node in the right direction.

Takes the 2-channel node output of the GNN and optimizes node-wise scores
such that the score corresponding to the correct orientation is maximized.

For use in config:

..  code-block:: yaml

    model:
      name: grappa
      modules:
        grappa_loss:
          node_loss:
            name: orient
            <dictionary of arguments to pass to the loss>

See configuration files prefixed with `grappa_` under the `config`
directory for detailed examples of working configurations.

---
### ClassDef: `NodeRegressionLoss`

Generic loss used to train node regression.

Takes the C-channel node output of the GNN and optimizes node-wise values
such that it matches the label values as closely as possible.

For use in config:

..  code-block:: yaml

    model:
      name: grappa
      modules:
        grappa_loss:
          node_loss:
            name: reg
            <dictionary of arguments to pass to the loss>

See configuration files prefixed with `grappa_` under the `config`
directory for detailed examples of working configurations.

---
### ClassDef: `NodeShowerPrimaryLoss`

Loss used to train the EM shower primary identification.

Takes the two-channel node output of the GNN and optimizes node-wise scores
such that nodes that initiate a particle cascade are given a high score
(exclusively relevant for showers for now).

For use in config:

..  code-block:: yaml

    model:
      name: grappa
      modules:
        grappa_loss:
          node_loss:
            name: shower_primary
            <dictionary of arguments to pass to the loss>

See configuration files prefixed with `grappa_` under the `config`
directory for detailed examples of working configurations.

---
### ClassDef: `NodeVertexLoss`

Loss used to predict the position of the vertex within each interaction.

This loss formulates the problem as a node problem:
- Predict which nodes are primary nodes (originate from the vertex);
- Primary nodes predict the vertex position;
- The positions predicted by each primary particle are aggregated
  downstream to form a vertex prediction for each interaction.

This loss expects 5 outputs per node:
- 2 for the primary identification
- 3 for the position regression

For use in config:

..  code-block:: yaml

    model:
      name: grappa
      modules:
        grappa_loss:
          node_loss:
            name: vertex
            <dictionary of arguments to pass to the loss>

See configuration files prefixed with `grappa_` under the `config`
directory for detailed examples of working configurations.

---
### FunctionDef: `norm`

Numba implementation of `np.linalg.norm(x, axis)`.

Parameters
----------
x : np.ndarray
    (N,M) array of values
axis : int
    Array axis ID

Returns
-------
np.ndarray
    (N) or (M) array of `norm` values

---
### FunctionDef: `norm_dict`

Dictionary of recognized normalization functions.

---
### FunctionDef: `norm_dict`

Dictionary of valid normalization functions.

---
### FunctionDef: `norm_factory`

Instantiates a normalization layer.

Parameters
----------
cfg : dict
    Normalization layer configuration
num_features : int
    Number of features to normalize

Return
------
object
    Instantiated normalization layer

---
### FunctionDef: `norm_factory`

Instantiates a normalization layer.

Parameters
----------
cfg : dict
    Normalization layer configuration
num_features : int
    Number of features to normalize

Return
------
object
    Instantiated normalization layer

---
### FunctionDef: `num_chambers`

Number of individual TPC voulmes.

Returns
-------
int
    Number of TPC volumes, N_t

---
### FunctionDef: `num_chambers`

Number of individual TPCs that make up this module.

Returns
-------
int
    Number of TPCs in the module

---
### FunctionDef: `num_chambers_per_module`

Number of TPC volumes per module.

Returns
-------
int
    Number of TPC volumes per module, N_t

---
### FunctionDef: `num_detectors`

Number of optical detectors.

Returns
-------
int
    Total number of optical detector, N_v*N_o

---
### FunctionDef: `num_detectors`

Returns the number of CRT planes around the detector.

Returns
-------
int
    Number of CRT planes, N_c

---
### FunctionDef: `num_detectors_per_volume`

Returns the number of optical detectors in each optical volume.

Returns
-------
int
    Number of optical detectors in each volume, N_o

---
### FunctionDef: `num_elements`

Total number of pixel in the image.

Returns
-------
int
    Total number of pixel in the image.

---
### FunctionDef: `num_fragments`

Number of fragments that make up this particle.

Returns
-------
int
    Number of fragments that make up the particle instance

---
### FunctionDef: `num_modules`

Number of detector modules.

Returns
-------
int
    Number of detector modules, N_m

---
### FunctionDef: `num_particles`

Number of particles that make up this interaction.

Returns
-------
int
    Number of particles that make up the interaction instance

---
### FunctionDef: `num_primary_particles`

Number of primary particles associated with this interaction.

Returns
-------
int
    Number of particles associated with the interaction instance

---
### FunctionDef: `num_volumes`

Returns the number of optical volumes.

Returns
-------
int
    Number of optical volumes, N_v

---
### FunctionDef: `numbafy`

Function which wraps a `numba` function with some checks on the input
to make the relevant conversions to numpy where necessary.

Parameters
----------
cast_args : list(str), optional
    List of arguments to be cast to numpy
list_args : list(str), optional
    List of arguments which need to be cast to a numba typed list
keep_torch : bool, default False
    Make the output a torch object, if the reference argument is one
ref_arg : str, optional
    Reference argument used to assign a type and device to the torch output

Returns
-------
callable
    Wrapped function which ensures input type compatibility with numba

---
### ClassDef: `ObjectList`

List with a default object used to type it when it is empty.

Attributes
----------
default : object
    Default object class to use to type the list, if it is empty

---
### FunctionDef: `occupancy_loss`

INPUTS:
    - occ (N x 1)
    - groups (N)

---
### ClassDef: `OptDetector`

Handles all geometry queries for a set of optical detectors.

Attributes
----------
volume : str
    The boundaries of each optical volume ('tpc' or 'module'), as defined
    by the the set of PMTs in each volume
positions : np.ndarray
    (N_v, N_o, 3) Location of the center of each of the optical detectors
    - N_v is the number of optical volumes
    - N_o is the number of optical detectors in each volume
shape : List[str]
    (N_d) Optical detector shape(s), combination of 'ellipsoid' and 'box'
    - N_d is the number of detector types
dimensions : np.ndarray
    (N_d, 3) Dimensions of each of the optical detector types
    - N_d is the number of detector types
shape_ids : np.ndarray, optional
    (N_o) Type of each of the optical detectors
    - N_o is the number of optical detectors
det_ids : np.ndarray, optional
    (N_c) Mapping between the optical channel and its corresponding detector
    - N_c is the number of optical channels (this number can be larger
    than the number of detectors if e.g. multiple SiPMs are used per
    optical detector)

---
### FunctionDef: `optical_traces`

Function which produces a list of traces which represent the optical
detectors in a 3D event display.

Parameters
----------
meta : Meta, optional
    Metadata information (only needed if pixel_coordinates is True)
shared_legend : bool, default True
    If True, the legend entry in plotly is shared between all the
    detector volumes
legendgroup : str, optional
    Legend group to be shared between all boxes
name : Union[str, List[str]], default 'Detector'
    Name(s) of the detector volumes
color : Union[int, str, np.ndarray]
    Color of optical detectors or list of color of optical detectors
cmin : float, optional
    Minimum value along the color scale
cmax : float, optional
    Maximum value along the color scale
zero_supress : bool, default False
    If `True`, do not draw optical detectors that are not activated
volume_id : int, optional
    Specifies which optical volume to represent. If not specified, all
    the optical volumes are drawn
**kwargs : dict, optional
    List of additional arguments to pass to
    spine.vis.ellipsoid.ellipsoid_traces or spine.vis.box.box_traces

Returns
-------
List[plotly.graph_objs.Mesh3D]
    List of optical detector traces (one per optical detector)

---
### FunctionDef: `optim_dict`

Dictionary of valid optimizers.

---
### FunctionDef: `optim_factory`

Instantiates an optimizer from a configuration dictionary.

Parameters
----------
cfg : dict
    Optimizer configuration
params : dict
    Torch model parameters to optimize

Returns
-------
object
    Instantiated optimizer

---
### ClassDef: `OrphanAssigner`

Clustering orphan assignment.

This class takes care of finding the best match cluster ID for points that
have not found a suitable group in the upstream clustering.

This is a wrapper class for two `scikit-learn` classes:
- :class:`KNeighborsClassifier`
- :class:`RadiusNeighborsClassifier`

---
### ClassDef: `OutBase`

Base data structure shared among all output classes.

Attributes
----------
id : int
    Unique index of the object within the object list
index : np.ndarray
    (N) Voxel indexes corresponding to this object in the input tensor
size : int
    Number of points, N, that make up this object
points : np.ndarray
    (N, 3) Set of voxel coordinates that make up this object
depositions : np.ndarray
    (N) Array of charge deposition values for each voxel
depositions_sum : float
    Total amount of depositions
sources : np.ndarray
    (N, 2) Set of voxel sources as (Module ID, TPC ID) pairs
module_ids : np.ndarray
    (M) List of module indexes that make up this object
is_contained : bool
    Whether this object is fully contained within the detector
is_matched: bool
    True if a true object match was found
match_ids : np.ndarray
    List of true object IDs this object is matched to
match_overlaps : np.ndarray
    List of match overlaps (IoU) between the object and its matches
is_cathode_crosser : bool
    True if the particle crossed a cathode, i.e. if it is made up
    of space points coming from > 1 TPC in one module
cathode_offset : float
    If the particle is a cathode crosser, this corresponds to the offset
    to apply to the particle to match its components at the cathode
is_truth: bool
    Whether this object contains truth information or not
units : str
    Units in which coordinates are expressed

---
### FunctionDef: `overlap_chamfer`

Computes a set overlap matrix by Chamfer distance.

This function can match two arbitrary points clouds, hence there is no need
for the two particle lists to share the same underlying voxel sets.

Parameters
----------
points_x: nb.types.List[np.ndarray]
    (N, 3) nb.types.List of coordinates, one per object to match
points_y: nb.types.List[np.ndarray]
    (M, 3) nb.types.List of coordinates, one per object to be matched to

Returns
-------
np.ndarray
    (M, N) Chamfer distance matrix

Notes
-----
Unlike the overlap metrics, this metric should be minimized.

---
### FunctionDef: `overlap_count`

Computes a set overlap matrix by overlap count.

Parameters
----------
index_x: nb.types.List[np.ndarray]
    (N) nb.types.List of tensor index, one per object to match
index_y: nb.types.List[np.ndarray]
    (M) nb.types.List of tensor index, one per object to be matched to

Returns
-------
np.ndarray
    (M, N) Overlap count matrix

---
### FunctionDef: `overlap_dice`

Computes a set overlap matrix by Dice coefficient.

The Dice coefficient corresponds to the 2 times the intersection of two
sets over the sum of set sizes.

Parameters
----------
index_x: nb.types.List[np.ndarray]
    (N) nb.types.List of tensor index, one per object to match
index_y: nb.types.List[np.ndarray]
    (M) nb.types.List of tensor index, one per object to be matched to

Returns
-------
np.ndarray
    (M, N) Overlap weighted IoU matrix

---
### FunctionDef: `overlap_iou`

Computes a set overlap matrix by IoU.

IoU stands for Intersection-over-Union.

Parameters
----------
index_x: nb.types.List[np.ndarray]
    (N) nb.types.List of tensor index, one per object to match
index_y: nb.types.List[np.ndarray]
    (M) nb.types.List of tensor index, one per object to be matched to

Returns
-------
np.ndarray
    (M, N) Overlap IoU matrix

---
### FunctionDef: `overlap_weighted_dice`

Computes a set overlap matrix by Dice coefficient, weighted by the
set sizes.

The Dice coefficient corresponds to the 2 times the intersection of two
sets over the sum of set sizes. The weighting scheme is as follows:
w = (|size_x + size_y| / (|size_x - size_y| + 1).

Parameters
----------
index_x: nb.types.List[np.ndarray]
    (N) nb.types.List of tensor index, one per object to match
index_y: nb.types.List[np.ndarray]
    (M) nb.types.List of tensor index, one per object to be matched to

Returns
-------
np.ndarray
    (M, N) Overlap weighted IoU matrix

---
### FunctionDef: `overlap_weighted_iou`

Computes a set overlap matrix by IoU, weighted by the set sizes.

IoU stands for Intersection-over-Union. The weighting scheme is as follows:
w = (|size_x + size_y| / (|size_x - size_y| + 1).

Parameters
----------
index_x: nb.types.List[np.ndarray]
    (N) nb.types.List of tensor index, one per object to match
index_y: nb.types.List[np.ndarray]
    (M) nb.types.List of tensor index, one per object to be matched to

Returns
-------
np.ndarray
    (M, N) Overlap weighted IoU matrix

---
### FunctionDef: `p`

Computes the magnitude of the initial momentum.

Returns
-------
float
    Norm of the initial momentum vector

---
### FunctionDef: `p`

Computes the magnitude of the initial momentum.

Returns
-------
float
    Norm of the initial momentum vector

---
### FunctionDef: `parse_config`

Parse the analysis tool configuration.

Parameters
----------
log_dir : str
    Output CSV file directory (shared with driver log)
prefix : str
    Input file prefix. If requested, it will be used to prefix
    all the output CSV files.
overwrite : bool, optional
    If `True`, overwrite the CSV logs if they already exist
prefix_output : bool, optional
    If `True`, will prefix the output CSV names with the input file name
**modules : dict
    List of analysis script modules

---
### FunctionDef: `parse_configuration`

Parse the geometry configuration.

Parameters
----------
tpc : dict
    Detector boundary configuration
optical : dict, optional
    Optical detector configuration
crt : dict, optional
    CRT detector configuration

---
### FunctionDef: `parse_entry_list`

Parses a list into an np.ndarray.

The list can be passed as a simple python list or a path to a file
which contains space or comma separated numbers (can be on multiple
lines or not)

Parameters
----------
list_source : Union[list, str]
    List as a python list or a text file path

Returns
-------
np.ndarray
    List as a numpy array

---
### FunctionDef: `parse_optical`

Parse the optical detector configuration.

Parameters
----------
volume : str
    Optical volume boundaries (one of 'tpc' or 'module')
**optical : dict
    Reset of the optical detector configuration

---
### FunctionDef: `parse_run_event_list`

Parses a list of (run, subrun, event) triplets into an np.ndarray.

The list can be passed as a simple python list or a path to a file
which contains one (run, subrun, event) pair per line.

Parameters
----------
list_source : Union[list, str]
    List as a python list or a text file path

Returns
-------
Tuple[Tuple[int]]
    List as a numpy array

---
### ClassDef: `ParserBase`

Abstract parent class of all parser classes.

Provides basic functionality shared by all parsers:
1. Defines a :meth:`__call__` function shared by all classes

Attributes
----------
name : str
    Name of the parser
aliases : List[str]
    Aliases of the parser (allowed but disfavored names)
data_map : dict[str, str]
    Maps function parameter names onto a file data product name
tree_keys : List[str]
    List of file data product name

---
### ClassDef: `Particle`

Particle truth information.

Attributes
----------
id : int
    Index of the particle in the list
mct_index : int
    Index in the original MCTruth array from whence it came
mcst_index : int
    Index in the original MCTrack/MCShower array from whence it came
group_id : int
    Index of the group the particle belongs to
interaction_id : int
    Index of the interaction the partile belongs to
nu_id : int
    Index of the neutrino this particle belongs to
interaction_primary : int
    Whether the particle is primary in its interaction or not
group_primary : int
    Whether this particle is primary in its group or not
parent_id : int
    Index of the parent particle
children_id : np.ndarray
    List of indexes of the children particles
track_id : int
    Geant4 track ID
parent_track_id : int
    Geant4 track ID of the parent particle
ancestor_track_id : int
    Geant4 track ID of the ancestor particle
shape : int
    Enumerated semantic type of the particle
num_voxels : int
    Number of voxels matched to this particle instance
energy_init : float
    True initial energy in MeV
energy_deposit : float
    Amount of energy matched to this particle instance in MeV
distance_travel : float
    True amount of distance traveled by the particle in the active volume
creation_process : str
    Creation process
parent_creation_process : str
    Creation process of the parent particle
ancestor_creation_process : str
    Creation process of the ancestor particle
pid : int
    Enumerated particle species type of the particle
pdg_code : int
    Particle PDG code
parent_pdg_code : int
    Particle PDG code of the parent particle
ancestor_pdg_code : int
    Particle PDG code of the ancestor particle
t : float
    Particle creation time (ns)
end_t : float
    Particle death time (ns)
parent_t : float
    Particle creation time of the parent particle (ns)
ancestor_t : float
    Particle creation time of the ancestor particle (ns)
position : np.ndarray
    Location of the creation point of the particle
end_position : np.ndarray
    Location where the particle stopped
parent_position : np.ndarry
    Location of the creation point of the parent particle
ancestor_position : np.ndarray
    Location of the creation point of the ancestor particle
first_step : np.ndarray
    Location of the first energy deposition of the particle
last_step : np.ndarray
    Location of the last energy deposition of the particle
momentum : np.ndarray
    3-momentum of the particle at the production point
end_momentum : np.ndarray
    3-momentum of the particle at where it stops or exits the detector
p : float
    Momentum magnitude of the particle at the production point
end_p : float
    Momentum magnitude of the particle where it stops or exits the detector
mass : float
    Rest mass of the particle in MeV/c^2
units : str
    Units in which the position attributes are expressed

---
### FunctionDef: `particle_counts`

Number of particles of each PID species in this interaction.

Returns
-------
np.ndarray
    (P) Number of particles of each PID

---
### ClassDef: `ParticleBase`

Base particle-specific information.

Attributes
----------
fragments : List[object]
    List of fragments that make up the interaction
fragment_ids : np.ndarray
    List of Fragment IDs that make up this particle
num_fragments : int
    Number of fragments that make up this particle
interaction_id : int
    Index of the interaction this particle belongs to
shape : int
    Semantic type (shower (0), track (1), Michel (2), delta (3),
    low energy scatter (4)) of this particle
pid : int
    Particle species (Photon (0), Electron (1), Muon (2), Charged Pion (3),
    Proton (4), Kaon (5)) of this particle
chi2_pid : int
    Particle species as predicted by the chi2 template method (Muon (2),
    Charged Pion (3), Proton (4), Kaon (5)) of this particle
chi2_per_pid : np.ndarray
    (P) Array of chi2 values associated with each particle class
pdg_code : int
    PDG code corresponding to the PID number
is_primary : bool
    Whether this particle was the first in the particle group
length : float
    Length of the particle (only assigned to track objects)
start_point : np.ndarray
    (3) Particle start point
end_point : np.ndarray
    (3) Particle end point (only assigned to track objects)
start_dir : np.ndarray
    (3) Particle direction w.r.t. the start point
end_dir : np.ndarray
    (3) Particle direction w.r.t. the end point (only assigned
    to track objects)
mass : float
    Rest mass of the particle in MeV/c^2
ke : float
    Kinetic energy of the particle in MeV
calo_ke : float
    Kinetic energy reconstructed from the energy depositions alone in MeV
csda_ke : float
    Kinetic energy reconstructed from the particle range in MeV
csda_ke_per_pid : np.ndarray
    (P) Same as `csda_ke` but for every available track PID hypothesis
mcs_ke : float
    Kinetic energy reconstructed using the MCS method in MeV
mcs_ke_per_pid : np.ndarray
    (P) Same as `mcs_ke` but for every available track PID hypothesis
momentum : np.ndarray
    3-momentum of the particle at the production point in MeV/c
p : float
    Momentum magnitude of the particle at the production point in MeV/c
is_valid : bool
    Whether this particle counts towards an interaction topology. This
    may be False if a particle is below some defined energy threshold.

---
### ClassDef: `ParticleBuilder`

Builds reconstructed and truth particles.

It takes the raw output of the reconstruction chain, extracts the
necessary information and builds :class:`RecoParticle` and
:class:`TruthParticle` objects from it.

---
### ClassDef: `ParticleCoordinateParser`

Class that retrieves that end points of particles.

It provides the coordinates of the end points, time and shape.

.. code-block. yaml

    schema:
      coords:
        parser: particle_coordinates
        particle_event: particle_pcluster
        sparse_event: sparse3d_pcluster

---
### ClassDef: `ParticleGraphParser`

Class that uses larcv.EventParticle to construct edges
between particles (i.e. clusters).

.. code-block. yaml

    schema:
      graph:
        parser: particle_graph
        particle_event: particle_pcluster
        cluster_event: cluster3d_pcluster
        include_fragment_edges: false

---
### ClassDef: `ParticleNeutrinoLogicProcessor`

Enforce that there is at most 1 primary lepton per interaction.

In particular:
- If there is no muon and the interactions with a MIP are required to have
  one, turn one of the MIPs into a muon (and neutralize the pion score)
- If there are more than 1 muon per interaction, pick one muon and switch
  other muons to pions (and neutralize the muon score)

---
### ClassDef: `ParticleParser`

Class which loads larcv.Particle objects to local Particle ones.

.. code-block. yaml

    schema:
      particles:
        parser: particle
        particle_event: particle_pcluster
        cluster_event: cluster3d_pcluster
        asis: False
        pixel_coordinates: True
        post_process: True

---
### ClassDef: `ParticlePointParser`

Class that retrieves the points of interests.

It provides the coordinates of the end points, types and particle index.

.. code-block. yaml

    schema:
      points:
        parser: particle_points
        particle_event: particle_pcluster
        sparse_event: sparse3d_pcluster
        include_point_tagging: True

---
### ClassDef: `ParticleShapeLogicProcessor`

Enforce logical connections between semantic predictions and
particle-level predictions (PID and primary).

In particular:
- If a particle has shower shape, it can only have a shower PID
- If a particle has track shape, it can only have a track PID
- If a particle has delta/michel shape, it can only be a secondary electron

---
### ClassDef: `ParticleThresholdProcessor`

Adjust the particle PID and primary properties according to customizable
thresholds and priority orderings.

---
### FunctionDef: `pause`

Temporarily pause a watch for a unique key.

Parameters
----------
key : str
    Key for which to pause the clock

---
### FunctionDef: `pause`

Time when the stopwatch was last paused.

---
### FunctionDef: `pdg_code`

Translates the enumerated particle type to a sign-less PDG code.

Returns
-------
int
    Reconstructed sign-less PDG code

---
### FunctionDef: `pdist`

Numba implementation of
`scipy.spatial.distance.pdist(x, p=2)` in 3D.

Parameters
----------
x : np.ndarray
    (N, 3) array of point coordinates in the set
metric : str, default 'euclidean'
    Distance metric

Returns
-------
np.ndarray
    (N, N) array of pair-wise Euclidean distances

---
### FunctionDef: `pid_metrics`

Script which stores the scores, predictions and labels related
to particle identification in order to evaluate PID performance.

Parameters
----------
data_dict : dict
    Input data dictionary after post-processing
result_dict : dict
    Chain output dictionary after post-processing
primary_only : bool, default True
    If True, only store particles corresponding to primary particles
mpv_only : bool, default True
    If True, only store particles corresponding to particles from MPV interactions

Returns
-------
List[dict]
    One dictionary of relevant particle attribute per particle in
    the image being processed.
    
Information in <pid_metrics> will be saved to $log_dir/pid_metrics.csv.

---
### ClassDef: `PIDEnum`

Enumerates all possible particle species values.

---
### ClassDef: `PIDTemplateProcessor`

Produces particle species classification estimates based on dE/dx vs
residual range templates of tracks.

---
### FunctionDef: `point_modes`

Dictionary which makes the correspondance between the name of a true
object point attribute with the underlying point tensor it points to.

Returns
-------
Dict[str, str]
    Dictionary of (attribute, key) mapping for point coordinates

---
### FunctionDef: `point_modes`

Dictionary which makes the correspondance between the name of a true
object point attribute with the underlying point tensor it points to.

Returns
-------
Dict[str, str]
    Dictionary of (attribute, key) mapping for point coordinates

---
### FunctionDef: `point_modes`

Dictionary which makes the correspondance between the name of a true
object point attribute with the underlying point tensor it points to.

Returns
-------
Dict[str, str]
    Dictionary of (attribute, key) mapping for point coordinates

---
### ClassDef: `PointBreakClusterer`

Leverages particles start/end point positions to break up instances
of particles which touch (vertex, secondary interaction point, etc.).

Two methods are supported: `masked_dbscan` and `closest_path`.

The masked DBSCAN method proceeds as follows:
- Break up the input point cloud into DBSCAN clusters
- For each cluster, mask out regions around the particle end points
- Run DBSCAN on the masked point cloud
- Each new instance is a particle instance
- Unlabeled, masked points are merged to the closest instance

The closest path method proceeds as follows:
- Break up the input point cloud into DBSCAN clusters
- For each cluster, build a radius graph on its constituents
- Find the closest graph paths for each pair of particle end points
- The paths that belong to the minimum spanning tree are particles
- Points from the cloud are assigned to a particle using their
  proximity to a particle path

The latter only works on track clusters, not on EM showers.

---
### ClassDef: `PointNet`

Pytorch Geometric's implementation of PointNet, modified for
use in lartpc_spine3d and generalized. 

---
### ClassDef: `PointProposalAna`

Class which computes and stores the necessary data to evaluate the
point proposal accuracy.

It evaluates the following metrics:
- Distance from true to closest predicted point (efficiency)
- Distance from predicted to closest true point (purity)
- Point type classification accuracy
- Point end classification accuracy

---
### ClassDef: `PosDataBase`

Base class of for data structures with positional attributes.

Includes method to convert positional attributes

Attributes
----------
units : str
    Units in which the position attributes are expressed

---
### FunctionDef: `post_processor_factory`

Instantiates a post-processor module from a configuration dictionary.

Parameters
----------
name : str
    Name of the post-processor module
cfg : dict
    Post-processor module configuration

Returns
-------
object
     Initialized post-processor object

---
### ClassDef: `PostBase`

Base class of all post-processors.

This base class performs the following functions:
  - Ensures that the necessary method exist
  - Checks that the post-processor is provided the necessary information
    to do its job
  - Fetches the appropriate coordinate attributes
  - Ensures that the appropriate units are provided

Attributes
----------
name : str
    Name of the post-processor as defined in the configuration file
aliases : Tuple[str]
    Alternative acceptable names for a post-processor

---
### ClassDef: `PostHocCalibrationModel`

Base Class for Post-Hoc Uncertainty Calibration Methods

Post-hoc calibration methods are trained on a validation set
after its client model's (the model to be calibrated) training
has converged in the training set. 

The client model must be freezed so that the parameters does not
change over the course of training the calibration model.

Also, it is desirable that the calibration model preserves the
ordering of the logit predictions, so that the accuracy of the 
client model is completely unchanged after calibration (isotonicity)

---
### ClassDef: `PostManager`

Manager in charge of handling post-processing scripts.

It loads all the post-processor objects once and feeds them data.

---
### ClassDef: `PPN`

Point Proposal Network (PPN).

It requires a UResNet network as a backbone. Typical configuration:

.. code-block:: yaml

    model:
      name: uresnet_ppn_chain
      modules:
        uresnet:
          # Your uresnet config here
        ppn:
          # Your ppn config here

Configuration
-------------
dimension: int, default 3
num_input: int, default 1
allow_bias: bool, default False
spatial_size: int, default 512
leakiness: float, default 0.33
activation: dict
    For activation function, defaults to `{'name': 'lrelu', 'args': {}}`
norm_layer: dict
    For normalization function, defaults to `{'name': 'batch_norm', 'args': {}}`

depth: int, default 5
    Depth of UResNet, also corresponds to how many times we down/upsample.
filters: int, default 16
    Number of filters in the first convolution of UResNet.
    Will increase linearly with depth.
reps: int, default 2
    Convolution block repetition factor
input_kernel: int, default 3
    Receptive field size for very first convolution after input layer.
num_classes: int, default 5
mask_score_threshold: float, default 0.5
classify_endpoints: bool, default False
    Enable classification of points into start vs end points.
ppn_resolution: float, default 1.0
ghost: bool, default False
use_true_ghost_mask: bool, default False
mask_loss_name: str, default 'BCE'
    Can be 'BCE' or 'LogDice'

Output
------
ppn_points: torch.Tensor
    Contains  X, Y, Z predictions, semantic class prediction logits, and prob score
ppn_masks: list of torch.Tensor
    Binary masks at various spatial scales of PPN predictions (voxel-wise score > some threshold)
ppn_coords: list of torch.Tensor
    List of XYZ coordinates at various spatial scales.
ppn_layers: list of torch.Tensor
    List of score features at various spatial scales.
ppn_output_coords: torch.Tensor
    XYZ coordinates tensor at the very last layer of PPN (initial spatial scale)
ppn_classify_endpoints: torch.Tensor
    Logits for end/start point classification.

See Also
--------
:class:`PPNLoss`, :class:`spine.model.uresnet_ppn_chain`

---
### ClassDef: `PPNLoss`

Loss function for PPN.

Output
------
reg_loss : float
    Distance loss
mask_loss : float
    Binary voxel-wise prediction loss (is there an object of interest or not)
classify_endpoints_loss : float
    Endpoint classification loss
type_loss : float
    Semantic prediction loss
output_mask_accuracy: float
    Binary voxel-wise prediction accuracy in the last layer
type_accuracy : float
    Semantic prediction accuracy
classify_endpoints_accuracy : float
    Endpoint classification accuracy

See Also
--------
PPN, spine.model.uresnet_ppn_chain

---
### ClassDef: `PPNPredictor`

PPN post-processing class to convert PPN raw predictions into points.

---
### ClassDef: `PPNProcessor`

Run the PPN post-processing function to produce PPN candidate points
from the raw PPN output.

If requested, for each particle, match ppn_points that have hausdorff
distance less than a threshold and update the particle `ppn_candidates`
attribute in place.

If `restrict_shape` is `True`, points will be matched to particles with
the same predicted semantic type only.

---
### FunctionDef: `prepare_data`

Fetches the necessary data products to form the input to the forward
function and the input to the loss function.

Parameters
----------
data : dict
    Dictionary of input data product keys, each of which maps to its
    associated batched data product

Returns
-------
input_dict : dict
    Input to the forward pass of the model
loss_dict : dict
    Labels to be used in the loss computation

---
### FunctionDef: `prepare_grappa_input`

Prepares the input to a GrapPA model.

It builds the following input to GrpPA:
- points: end points of fragments/particles
- value: mean/std of charge distribution in each cluster
- shape: shape of each fragment/particle

Parameters
----------
model : torch.nn.Module
    GrapPA model to feed information to
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
clusts : IndexBatch
    List of clusters to aggregate using GrapPA
clust_shapes : TensorBatch
    Semantic type of each of the clusters
clust_primaries : IndexBatch, optional
    List of primary fragment within each cluster to aggregate
coord_label : TensorBatch, optional
    (N, 1 + D + 6) Array of label particle end points
point_use_primaries:
    Use the primary fragment only to infer primaries

Returns
-------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
clusts : IndexBatch
    Input clusters to the model
shapes : TensorBatch
    List of semantic type of each clusters
points : TensorBatch
    List of start/end points associated with each cluster
extra : TensorBatch
    List of additional features to pass to the GrapPA model

---
### FunctionDef: `primary_assignment`

Select shower primary fragments based on the node-score.

If node groupings are provided, selects a single primary per node
group: the one that is most likely.

Parameters
----------
node_pred : np.ndarray
    (C, 2) Logits associated with each node
group_ids : np.ndarray, optional
    (C) List of node group IDs

Returns
-------
np.ndarray
    (C) Primary labels

---
### FunctionDef: `primary_assignment_batch`

Batched version of :func:`primary_assignment`.

Parameters
----------
node_pred : TensorBatch
    (C, 2) Logits associated with each node
group_ids : TensorBatch, optional
    (C) List of node group IDs

Returns
-------
TensorBatch
    (C) Primary labels

---
### FunctionDef: `primary_particle_counts`

Number of primary particles of each PID species in this interaction.

Returns
-------
np.ndarray
    (P) Number of primary particles of each PID

---
### FunctionDef: `primary_particle_ids`

List of primary Particle IDs associated with this interaction.

Returns
-------
np.darray
    List of primary Particle IDs associated with this interaction

---
### FunctionDef: `primary_particles`

List of primary particles associated with this interaction.

Returns
-------
List[obect]
    List of primary Particle objects associated with this interaction

---
### FunctionDef: `principal_components`

Computes the principal components of a point cloud by computing the
eigenvectors of the centered covariance matrix.

Parameters
----------
x : np.ndarray
    (N, d) Coordinates in d dimensions

Returns
-------
np.ndarray
    (d, d) List of principal components (row-ordered)

---
### FunctionDef: `process`

Apply calibrations to each particle in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Apply the lifetime correction.

Parameters
----------
points : np.ndarray
    (N, 3) array of point coordinates
values : np.ndarray
    (N) array of values associated with each point
geo : Geometry
    Detector geometry object
tpc_id : int
    ID of the TPC to use
run_id : int, optional
    If provided, used to get the appropriate lifetime/drift velocities

Returns
-------
np.ndarray
    (N) array of corrected values

---
### FunctionDef: `process`

Apply the transparency correction.

Parameters
----------
points : np.ndarray
    (N, 3) array of point coordinates
values : np.ndarray
    (N) array of values associated with each point
tpc_id : int
    ID of the TPC to use
run_id : int
    Used to get the appropriate transparency map

Returns
-------
np.ndarray
    (N) array of corrected values

---
### FunctionDef: `process`

Assign track end points in one entry

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Build representations for a single entry.

Parameters
----------
data : dict
    Dictionary of data products
mode : str
    Type of object to reconstruct ('reco' or 'truth')
entry : int, optional
    Entry to process

---
### FunctionDef: `process`

Check the containment of all objects in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Check the fiducial status of all interactions in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Converts a 2D clusters tensor into a single tensor.

Parameters
----------
cluster_event : larcv.EventClusterPixel2D
    Event which contains the 2D clusters

Returns
-------
np_voxels : np.ndarray
    (N, 2) array of [x, y] coordinates
np_features : np.ndarray
    (N, 2) array of [pixel value, cluster ID]
meta : Meta
    Metadata of the parsed image

---
### FunctionDef: `process`

Converts deposition values from ADC to a number of electrons.

Parameters
----------
values : np.ndarray
    (N) array of depositions in ADC in a specific TPC
tpc_id : int
    ID of the TPC to use

Returns
-------
np.ndarray
    (N) array of depositions in number of electrons

---
### FunctionDef: `process`

Corrects for electron recombination.

Parameters
----------
values : np.ndarray
    (N) array of depositions in number of electrons
points : np.ndarray, optional
    (N, 3) array of point coordinates associated with one particle.
    Only needed if `track` is set to `True`.
track : bool, defaut `False`
    Whether the object is a track or not. If it is, the track gets
    segmented to evaluate local dE/dx and track angle.

Returns
-------
np.ndarray
    (N) array of depositions in MeV

---
### FunctionDef: `process`

Corrects for field non-uniformities.

Notes
-----
Placeholder until this module is implemented

---
### FunctionDef: `process`

Count children of each true particle in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Evaluate shower start dE/dx for one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Evaluate track completeness for tracks in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Fetch the kinetic energy of the first particle.

Configuration
-------------
particle_event : larcv.EventParticle
    Particle event which contains the list of true particles

Returns
-------
float
    Kinetic energy of the first particle

---
### FunctionDef: `process`

Fetch the list of label points of interest.

Parameters
----------
particle_event : larcv.EventParticle
    Particle event which contains the list of true particles
sparse_event : larcv.EventSparseTensor3D, optional
    Tensor which contains the metadata needed to convert the
    positions in voxel coordinates
cluster_event : larcv.EventClusterVoxel3D, optional
    Cluster which contains the metadata needed to convert the
    positions in voxel coordinates

Returns
-------
np_voxels : np.ndarray
    (N, 3) array of [x, y, z] coordinates
np_features : np.ndarray
    (N, 2/3) array of [point type, particle index(, end point tagging)]
meta : Meta
    Metadata of the parsed image

---
### FunctionDef: `process`

Fetch the list of label vertex points.

Parameters
----------
particle_event : larcv.EventParticle
    Particle event which contains the list of true particles
neutrino_event : larcv.EventNeutrino
    Neutrino event which contains the list of true neutrinos
sparse_event : larcv.EventSparseTensor3D, optional
    Tensor which contains the metadata needed to convert the
    positions in voxel coordinates
cluster_event : larcv.EventClusterVoxel3D, optional
    Cluster which contains the metadata needed to convert the
    positions in voxel coordinates

Returns
-------
np_voxels : np.ndarray
    (N, 3) array of [x, y, z] coordinates
np_features : np.ndarray
    (N, 1) array of [vertex ID]
meta : Meta
    Metadata of the parsed image

---
### FunctionDef: `process`

Fetch the list of true neutrino objects.

Parameters
----------
neutrino_event : larcv.EventNeutrino
    Neutrino event which contains the list of true neutrinos
sparse_event : larcv.EventSparseTensor3D, optional
    Tensor which contains the metadata needed to convert the
    positions in voxel coordinates
cluster_event : larcv.EventClusterVoxel3D, optional
    Cluster which contains the metadata needed to convert the
    positions in voxel coordinates

Returns
-------
List[Neutrino]
    List of true neutrino objects

---
### FunctionDef: `process`

Fetch the list of true particle objects.

Parameters
----------
particle_event : larcv.EventParticle
    Particle event which contains the list of true particles
sparse_event : larcv.EventSparseTensor3D, optional
    Tensor which contains the metadata needed to convert the
    positions in voxel coordinates
cluster_event : larcv.EventClusterVoxel3D, optional
    Cluster which contains the metadata needed to convert the
    positions in voxel coordinates
particle_mpv_event : larcv.EventParticle, optional
    Particle event which contains the list of true MPV particles
neutrino_event : larcv.EventNeutrino, optional
    Neutrino event which contains the list of true neutrinos

Returns
-------
List[Particle]
    List of true particle objects

---
### FunctionDef: `process`

Fetch the parentage connections from the true particle list.

Configuration
-------------
particle_event : larcv.EventParticle
    Particle event which contains the list of true particles
cluster_event : larcv.EventClusterVoxel3D, optional
    Cluster used to check if particles have 0 pixel in the image. If
    so, the edges to those clusters are removed and the broken
    parantage is subsequently patched.

Returns
-------
np.ndarray
    (2, E) Array of directed edges for each [parent, child] connection
int
    Number of particles in the input

---
### FunctionDef: `process`

Fetch the species of the first particle.

Configuration
-------------
particle_event : larcv.EventParticle
    Particle event which contains the list of true particles

Returns
-------
int
    Species of the first particle

---
### FunctionDef: `process`

Fetch the start/end point and time of each true particle.

Parameters
----------
particle_event : larcv.EventParticle
    Particle event which contains the list of true particles
sparse_event : larcv.EventSparseTensor3D, optional
    Tensor which contains the metadata needed to convert the
    positions in voxel coordinates
cluster_event : larcv.EventClusterVoxel3D, optional
    Cluster which contains the metadata needed to convert the
    positions in voxel coordinates

Returns
-------
np_voxels : np.ndarray
    (N, 6) array of [x_s, y_s, z_s, x_e, y_e, z_e] start and end
    point coordinates
np_features : np.ndarray
    (N, 2) array of [first_step_t, shape_id]
meta : Meta
    Metadata of the parsed image

---
### FunctionDef: `process`

Fetches one or a list of tensors, concatenate their feature vectors.

Parameters
----------
sparse_event: larcv.EventSparseTensor3D, optional
    Sparse tensor to get the voxel/features from
sparse_event_list: List[larcv.EventSparseTensor3D], optional
    List of sparse tensors to get the voxel/features from

Returns
-------
np_voxels : np.ndarray
    (N, 3) array of [x, y, z] coordinates
np_features : np.ndarray
    (N, C) array of [pixel value 0, pixel value 1, ...]
meta : Meta
    Metadata of the parsed images

---
### FunctionDef: `process`

Fetches one or a list of tensors, concatenate their feature vectors.

Parameters
-------------
sparse_event: larcv.EventSparseTensor2D, optional
    Sparse tensor to get the voxel/features from
sparse_event_list: List[larcv.EventSparseTensor2D], optional
    List of sparse tensors to get the voxel/features from

Returns
-------
np_voxels : np.ndarray
    (N, 2) array of [x, y] coordinates
np_features : np.ndarray
    (N, C) array of [pixel value 0, pixel value 1, ...]
meta : Meta
    Metadata of the parsed images

---
### FunctionDef: `process`

Fetches the list of CRT hits.

Parameters
----------
crthit_event : larcv.CRTHitEvent

Returns
-------
List[CRTHit]
    List of CRT hit objects

---
### FunctionDef: `process`

Fetches the list of optical flashes.

Parameters
-------------
flash_event : larcv.EventFlash, optional
    Optical flash event which contains a list of flash objects
flash_event_list : List[larcv.EventFlash], optional
    List of optical flash events, each a list of flash objects

Returns
-------
List[Flash]
    List of optical flash objects

---
### FunctionDef: `process`

Fetches the metadata from one object that has it.

Parameters
----------
sparse_event : Union[larcv.EventSparseTensor2D
                     larcv.EventSparseTensor3D], optional
    Tensor which contains the metadata information as an attribute
cluster_event : Union[larcv.EventClusterPixel2D,
                      larcv.EventClusterVoxel3D], optional
    Cluster which contains the metadata information as an attribute

Returns
-------
Meta
    Metadata information for one image

---
### FunctionDef: `process`

Fetches the run information from one object that has it.

Parameters
----------
sparse_event : Union[larcv.EventSparseTensor2D
                     larcv.EventSparseTensor3D], optional
    Tensor which contains the run information as an attribute
cluster_event : Union[larcv.EventClusterPixel2D,
                      larcv.EventClusterVoxel3D], optional
    Cluster which contains the run information as an attribute

Returns
-------
RunInfo
    Run information object

---
### FunctionDef: `process`

Fetches the trigger information.

Parameters
----------
trigger_event : larcv.TriggerEvent

Returns
-------
Trigger
    Trigger object

---
### FunctionDef: `process`

Find [interaction, flash] pairs.

Parameters
----------
data : dict
    Dictionary of data products

Notes
-----
This post-processor modifies the list of `interaction` objectss
in-place by filling the following attributes
- interaction.is_flash_matched: (bool)
       Indicator for whether the given interaction has a flash match
- interaction.flash_ids: np.ndarray
       The flash IDs in the flash list
- interaction.flash_volume_ids: np.ndarray
       The flash optical volume IDs in the flash list
- interaction.flash_times: np.ndarray
       The flash time(s) in microseconds
- interaction.flash_total_pe: float
       Total number of PEs associated with the matched flash(es)
- interaction.flash_hypo_pe: float, optional
       Total number of PEss associated with the hypothesis flash

---
### FunctionDef: `process`

Find cathode crossing particles in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Find particle/CRT matches for one entry.
Parameters

----------
data : dict
    Dictionary of data products

Notes
-----
This post-processor also modifies the list of Interactions
in-place by adding the following attributes:
    particle.is_crthit_matched: bool
        Indicator for whether the given particle has a CRT-TPC match
    particle.crthit_ids: List[int]
        List of IDs for CRT hits that were matched to that particle

---
### FunctionDef: `process`

Loop over the reco interactions and merge tracks into showers,
if they pass the selection criteria.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Loop through reco interactions and modify reco particle's
primary label based on the proximity to reconstructed vertex.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Match all the requested objects in one entry.

Parameters
----------
data: dict
    Dictionary of data products

---
### FunctionDef: `process`

Parse a list of 3D clusters into a single tensor.

Parameters
----------
cluster_event : larcv.EventClusterVoxel3D
    Event which contains the 3D clusters
particle_event : larcv.EventParticle, optional
    List of true particle information. If prodided, allows to fetch
    more information about each of the pixels in the image
particle_mpv_event : larcv.EventParticle, optional
    List of true particle information for MPV particles only. If
    provided, it is used to determine which particles are MPV
particle_mpv_event: larcv.EventNeutrino, optional
    List of true neutrino information. If provided, it is used
    to determine which particles are MPV
sparse_semantics_event : larcv.EventSparseTensor3D, optional
    Semantics of each of the voxels in the image. If provided,
    overrides the order of precedence used in combining clusters
    which share voxels.
sparse_value_event : larcv.EventSparseTensor3D, optional
    Value of each of the voxels in the image. If provided,
    overrides the value provided byt eh list of 3D clusters itself

Returns
-------
np_voxels : np.ndarray
    (N, 3) array of [x, y, z] coordinates
np_features : np.ndarray
    (N, 2/14) array of features, minimally [voxel value, cluster ID].
    If `add_particle_info` is `True`, the additonal columns are
    [particle ID, group ID, interaction ID, neutrino ID, particle type,
    group primary bool, interaction primary bool, vertex x, vertex y,
    vertex z, momentum, semantic type]
meta : Meta
    Metadata of the parsed image

---
### FunctionDef: `process`

Parse the trigger information of one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Pass data products corresponding to one entry through the analysis.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Pass data products corresponding to one entry through the processor.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Place-holder method to be defined in each analysis script.

Parameters
----------
data : dict
    Filtered data dictionary for one entry

---
### FunctionDef: `process`

Place-holder method to be defined in each post-processor.

Parameters
----------
data : dict
    Dictionary of processed data products

---
### FunctionDef: `process`

Process one entry or a batch of entries.

Run single step of main SPINE driver. This includes data loading,
model forwarding, data structure building, post-processing
and appending desired information to each row of output csv files.

Parameters
----------
entry : int, optional
    Entry number to load
run : int, optional
    Run number to load
subrun : int, optional
    Subrun number to load
event : int, optional
    Event number to load
iteration : int, optional
    Iteration number. Only needed to train models and/or to apply
    time-dependant model losses, no-op otherwise

Returns
-------
Union[dict, List[dict]]
    Either one combined data dictionary, or one per entry in the batch

---
### FunctionDef: `process`

Produce PPN candidates for one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Reconstruct the CSDA KE estimates for each particle in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Reconstruct the CSDA KE estimates for each particle in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Reconstruct the MCS KE estimates for each particle in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Reconstruct the calorimetric KE for each particle in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Reconstruct the directions of all particles in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Reconstruct the vertex position for each interaction in one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Store basic event information for one entry.

Parameters
----------
data : dict
    Dictionary of data products containing particle representations

---
### FunctionDef: `process`

Store the clustering metrics for one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Store the flash matching metrics for one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Store the information from one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Store the semantic segmentation metrics for one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Store the semantic segmentation metrics for one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Update PID and primary predictions of each particle in one entry

Parameters
----------
data : dict
    Dictionaries of data products

---
### FunctionDef: `process`

Update PID and primary predictions of each particle in one entry

Parameters
----------
data : dict
    Dictionaries of data products

---
### FunctionDef: `process`

Update PID predictions of each particle one entry.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Update each interaction topology in one interaction.

Parameters
----------
data : dict
    Dictionary of data products

---
### FunctionDef: `process`

Update reco interaction topologies using the conversion
distance cut.

Parameters
----------
data : dict
    Dictionaries of data products

Raises
------
ValueError
    If provided vertex mode is invalid.

---
### FunctionDef: `process`

Update reco interaction topologies using the shower multi-arm check.

Parameters
----------
data : dict
    Dictionaries of data products

---
### FunctionDef: `process`

Update the shower startpoint using the closest point to the vertex.

Parameters
----------
data : dict
    Dictionaries of data products

---
### FunctionDef: `process_aggr`

Fetches a list of tensors, aggregate their feature vectors.

Parameters
-------------
sparse_event_list: List[larcv.EventSparseTensor3D]
    Sparse tensor list to get the voxel/features from

Returns
-------
np_voxels : np.ndarray
    (N, 3) array of [x, y, z] coordinates
np_features : np.ndarray
    (N, 1) array of aggregated features
meta : Meta
    Metadata of the parsed image

---
### FunctionDef: `process_aggr`

Parse a list of 3D clusters into a single tensor and fetch the
value column by aggregating multiple tensor features.

Parameters
----------
sparse_value_event_list : List[larcv.EventSparseTensor3D]
    List of sparse value tensors
**kwargs : dict, optional
    Extra data products to pass to the parent Cluster3DParser

Returns
-------
np_voxels : np.ndarray
    (N, 3) array of [x, y, z] coordinates
np_features : np.ndarray
    (N, 2/14) array of features, minimally [voxel value, cluster ID].
    If `add_particle_info` is `True`, the additonal columns are
    [group ID, interaction ID, neutrino ID, particle type,
    group primary bool, interaction primary bool, vertex x, vertex y,
    vertex z, momentum, semantic type, particle ID]
meta : Meta
    Metadata of the parsed image

---
### FunctionDef: `process_backbone_config`

Initialize the underlying UResNet model configuration.

Parameters
----------
num_classes : int
    Number of classes to classify the voxels as
ghost : bool, default False
    Whether to add a deghosting step in the classification model
**backbone : dict
    UResNet backbone configuration

---
### FunctionDef: `process_backbone_config`

Process the parameters of the backbone model needed for in the loss.

Parameters
----------
depth : int
    Depth of the UResNet
**kwargs : dict, optional
    Leftover model configuration (no need in the loss)

---
### FunctionDef: `process_chain_config`

Process the full chain configuration and dump it.

Parameters
----------
dump_config : bool, default False
    Whether to dump the chain configuration in the log file or not
**parameters : dict
    Dictionary of chain configuration parameters

---
### FunctionDef: `process_config`

Reads the configuration and dumps it to the logger.

Parameters
----------
io : dict
    I/O configuration dictionary
base : dict, optional
    Base driver configuration dictionary
model : dict, optional
    Model configuration dictionary
build : dict, optional
    Representation building configuration dictionary
post : dict, optional
    Post-processor configutation dictionary
ana : dict, optional
    Analysis script configurationdictionary
rank : int, optional
    Rank of the GPU. The model will be run on CPU if `world_size` is not
    specified or 0 and on GPU is `world_size` is > 0.

Returns
-------
dict
    Processed configuration

---
### FunctionDef: `process_dbscan_config`

Process the DBSCAN fragmenter configuration.

Parameters
----------
shapes : Union[int, list], optional
    This should not be specified (fetched from the node configuration)
min_size : Union[int, list], optional
    This should not be specified (fetched from the node configuration)
**kwargs : dict, optional
    Rest of the DBSCAN configuration

---
### FunctionDef: `process_domain_config`

Process hyperparameter domain configuration dictionary 
into Ax-compatible form.

---
### FunctionDef: `process_entry_list`

Create a list of entries that can be accessed by :meth:`__getitem__`.

Parameters
----------
n_entry : int, optional
    Maximum number of entries to load
n_skip : int, optional
    Number of entries to skip at the beginning
entry_list : list, optional
    List of integer entry IDs to add to the index
skip_entry_list : list, optional
    List of integer entry IDs to skip from the index
run_event_list: list((int, int, int)), optional
    List of (run, subrun, event) triplets to add to the index
skip_run_event_list: list((int, int, int)), optional
    List of (run, subrun, event) triplets to skip from the index
allow_missing : bool, default False
    If `True`, allows missing entries in the entry or event list

Returns
-------
list
    List of integer entry IDs in the index

---
### FunctionDef: `process_file_paths`

Process list of files.

Parameters
----------
file_keys : list
    List of paths to the HDF5 files to be read
limit_num_files : int, optional
    Integer limiting number of files to be taken per data directory
max_print_files : int, default 10
    Maximum number of loaded file names to be printed

---
### FunctionDef: `process_final_config`

Process a final layer configuration.

Parameters
----------
final : Union[int, dict]
    Final layer configuration
prefix : dict
    Name of the final layer

---
### FunctionDef: `process_ghost`

Fetches one or a list of tensors, concatenate their feature vectors.

Parameters
-------------
sparse_event: larcv.EventSparseTensor3D
    Sparse tensor to get the semantic labels

Returns
-------
np_voxels : np.ndarray
    (N, 3) array of [x, y, z] coordinates
np_features : np.ndarray
    (N, 1) array of ghost labels (1 for ghosts, 0 otherwise)
meta : Meta
    Metadata of the parsed image

---
### FunctionDef: `process_gnn_config`

Process the GNN backbone structure and the output layers.

Parameters
----------
node_pred : Union[int, dict], optional
    Number of node predictions. If there are multiple node predictions,
    provide a (key, value) pair for each type of prediction
edge_pred : Union[int, dict], optional
    Number of edge predictions. If there are multiple edge predictions,
    provide a (key, value) pair for each type of prediction
global_pred : Union[int, dict], optional
    Number of edge predictions. If there are multiple edge predictions,
    provide a (key, value) pair for each type of prediction
**gnn_model, dict
    Paramters to initialize the GNN backbone

---
### FunctionDef: `process_loss_config`

Initialize the loss function

Parameters
----------
loss : str, default 'ce'
    Name of the loss function to apply
balance_loss : bool, default False
    Whether to weight the loss to account for class imbalance
weights : list, optional
    (C) One weight value per class

---
### FunctionDef: `process_loss_config`

Process the loss configuration

Parameters
----------
evaluate_clustering_metrics : bool, default False
    If `True`, evaluates the clustering accuracy directly, rather than
    simply reporting an edge assignment acurracy
**loss : dict
    Loss configurationd dictionary

---
### FunctionDef: `process_loss_config`

Process the loss configuration.

Parameters
----------
node_loss : Union[dict, Dict[dict]], optional
    Node loss configuration
edge_loss : Union[dict, Dict[dict]], optional
    Edge loss configuration
global_loss : Union[dict, Dict[dict]], optional
    Global loss configuration

---
### FunctionDef: `process_loss_config`

Process the loss function parameters.

Parameters
----------
loss : str, default 'ce'
    Loss function used for semantic segmentation
ghost_label : int, default -1
    ID of ghost points. If specified (> -1), classify ghosts only
alpha : float, default 1.0
    Classification loss prefactor
beta : float, default 1.0
    Ghost mask loss prefactor
balance_loss : bool, default False
    Whether to weight the loss to account for class imbalance
upweight_points : bool, default False
    Whether to weight the loss higher near specific points (to be
    provided as `point_label` as a loss input)
upweight_radius: bool, default False
    Radius around the points of interest for which to upweight the loss

---
### FunctionDef: `process_loss_config`

Process the loss function parameters.

Parameters
----------
resolution : float, default 5.
    Distance from a label point in pixels within which a voxel is
    considered positive (pixel of interest)
mask_loss : str, default 'CE'
    Name of the loss function to use
point_classes : Union[int, list], optional
    If provided, restricts the loss to points of (a) certain shape(s)
balance_mask_loss : bool, default True
    Apply class-weights to the mask loss
mask_weighting_mode : str, default 'const'
    Method for class-weighting the mask loss
balance_type_loss : bool, default True
    Apply class-weights to the type loss
type_weighting_method : str, default 'const'
    Method class-weighting the type loss
reg_loss_weight : float, default 1.
    Relative weight to apply to the regression loss
type_loss_weight : float, default 1.
    Relative weight to apply to the point type loss
mask_loss_weight : float, default 1.
    Relative weight to apply to the mask loss
endpoint_loss_weight : float, default 1.
    Relative weight to apply to the endpoint classification
return_mask_labels : bool, default False
    If `True`, returns the masks used to compute the mask loss
restrict_to_clusters : bool, default False
    If `True`, when computing the positive labels for PPN, it will only
    look for points that are close to a given PPN label point with the
    same particle id.

---
### FunctionDef: `process_model_config`

Initialize the underlying UResNet model.

Parameters
----------
num_classes : int
    Number of classes to classify the voxels as
ghost : bool, default False
    Whether to add a deghosting step in the classification model
**backbone : dict
    UResNet backbone configuration

---
### FunctionDef: `process_model_config`

Initialize the underlying encoder and the final layer.

Parameters
----------
num_classes : int
    Number of classes that each image can be sorted as
**encoder : dict
    Encoder configuration

---
### FunctionDef: `process_model_config`

Initialize the underlying encoder and the final layer.

Parameters
----------
num_classes : int
    Number of classes that each image can be sorted as
**encoder : dict
    Encoder configuration

---
### FunctionDef: `process_model_config`

Initialize the underlying modules.

Parameters
----------
embedder : dict
    Pixel embedding configuration
kernel : dict
    Edge kernel configuration
constructor : dict
    Edge index construction configuration
shapes : List[str]
    List of shape names to construct clusters for
use_raw_features : bool, default True
    Use the list of embedder features as is, without the output layers
invert : bool, default True
    Invert the edge scores so that 0 is on an 1 is off
make_clusters : bool, default False
    If `True`, builds a list of cluster indexes

---
### FunctionDef: `process_model_config`

Process the PPN-specific parameters.

Parameters
----------
mask_score_threshold : float, default 0.5
    Predicted score above which a pixel is considered positive
classify_endpoints : bool, default False
    Whether or not to predict which point is the start/end for a track
propagate_all : bool, default False
    If `True`, the mask will not be applied at every PPN layer
use_binary_mask : bool, default False
    If `True`, converts the features to a binary mask based on score
ghost : bool, default False
    Whether or not the input contains ghosts
use_true_ghost_mask : bool, default False
    If `True`, ghost labels to deghost the tensor

---
### FunctionDef: `process_model_config`

Process the embedding parameters.

Parameters
----------
predict_semantics : bool, default False
    If `True`, the embedder will output semantic predictions
num_classes : int, optional
    Number of classes to classify the voxels as
coord_conv : bool, default True
    If `True`, include the normalized pixel coordinates as a set of
    input features to the backbone UResNet
covariance_mode : str, default 'softplus'
    Activation used to predict cluster covariance (spatial extent)
occupancy_mode : str, default 'softplus'
    Activation used to predict cluster occupancy (pixel count)
feature_embedding_dim : int, default 16
    Number of features per pixel in embedding space
spatial_embedding_space : int, default 3
    Number of spatial features per pixel in embedding space

---
### FunctionDef: `process_model_config`

Process the model configuration

Parameters
----------
constructor : dict, optional
    Edge index construction configuration
shapes : List[int], default [0, 1, 2, 3]
    List of semantic shapes to run DBSCAN on
invert : bool, default True
    Invert the edge scores so that 0 is on an 1 is off

---
### FunctionDef: `process_model_config`

Process the parameters of the upstream model needed for in the loss.

Parameters
----------
num_classes : int
    Number of classes to classify the voxels as
ghost : bool, default False
    Whether to add a deghosting step in the classification model
**kwargs : dict, optional
    Leftover model configuration (no need in the loss)

---
### FunctionDef: `process_model_config`

Process the top-level configuration block.

This dispatches each block to its own configuration processor.

Parameters
----------
nodes : dict
    Input node configuration
graph : dict
    Input graph configuration
gnn_model : dict
    Underlying graph neural network configuration
node_encoder : dict
    Node encoder configuration
edge_encoder : dict
    Edge encoder configuration
global_encoder : dict, optional
    Global encoder configuration
dbscan : dict, optional
    DBSCAN fragmentation configuration

---
### FunctionDef: `process_node_config`

Process the node parameters of the model.

Parameters
----------
source : str, default 'cluster'
    Column name in the label tensor which contains the input cluster IDs
shapes : int, optional
    Type of nodes to include in the input. If not specified, include
    all types
min_size : int, default -1
    Minimum number of voxels in a cluster to be included in the input
make_groups : bool, default False
    Use edge predictions to build node groups
grouping_method : str, default 'score'
    Algorithm used to build a node partition
grouping_through_track : bool, default False
    If `True`, shower objects can only be connected to one track object

---
### FunctionDef: `process_overlay_config`

Process the image overlay configuration

Parameters
----------
mode : str, default 'const'
    Method used to from overlay indexes ('const' or 'poisson')
size : int, default 2
    Number of images to merge to produce each new image

---
### FunctionDef: `process_particle_event`

Corrects/fetches attributes for a larcv.EventParticle object.

Does the following:
- Builds the interaction ID information if it is not provided
- Gets the true neutrino ID this particle came from
- Gets a simplified enumerated particle species ID
- Gets a flag as to whether a particle is a primary within its interaction
- Gets a flag as to whether a particle is a primary within its group

Parameters
----------
particle_event : larcv.EventParticle
    (P) List of true particle instances
particle_mpv_event : larcv.EventParticle, optional
    (M) List of true MPV particle instances
neutrino_event : larcv.EventNeutrino, optional
    (N) List of true neutrino instances

Returns
-------
interaction_ids : np.ndarray
    (P) List of interaction IDs, one per true particle instance
nu_ids : np.ndarray
    (P) List of neutrino IDs, one per true particle instance
group_primary_ids : np.ndarray
    (P) List of particle group primary IDs, one per true particle instance
inter_primary_ids : np.ndarray
    (P) List of particle primary IDs, one per true particle instance
pids : np.ndarray
    (P) List of particle IDs, one per true particle instance

---
### FunctionDef: `process_particles`

Process Particle object list to add/correct attributes in place.

Does the following:
- Adds interaction ID information if it is not provided
- Adds the true neutrino ID this particle came from
- Adds a simplified enumerated particle species ID
- Adds a flag as to whether a particle is a primary within its interaction
- Adds a flag as to whether a particle is a primary within its group

Parameters
----------
particles : List[Particle]
    (P) List of true particle instances
particle_event : larcv.EventParticle
    (P) List of true particle instances
particle_mpv_event : larcv.EventParticle, optional
    (M) List of true MPV particle instances
neutrino_event : larcv.EventNeutrino, optional
    (N) List of true neutrino instances

---
### FunctionDef: `process_rescale`

Fetches one or a list of tensors, concatenate their feature vectors.

Parameters
-------------
sparse_event_list: List[larcv.EventSparseTensor3D]
    (7) List of sparse tensors used to compute the rescaled charge
    - Charge value of each of the contributing planes (3)
    - Index of the plane hit contributing to the space point (3)
    - Semantic labels (1)

Returns
-------
np_voxels : np.ndarray
    (N, 3) array of [x, y, z] coordinates
np_features : np.ndarray
    (N, 1) array of rescaled charge values
meta : Meta
    Metadata of the parsed image

---
### FunctionDef: `process_rescale`

Parse a list of 3D clusters into a single tensor and reset
the value column by rescaling the charge coming from 3 wire planes.

Parameters
----------
sparse_value_event_list : List[larcv.EventSparseTensor3D]
    (7) List of sparse tensors used to compute the rescaled charge
    - Charge value of each of the contributing planes (3)
    - Index of the plane hit contributing to the space point (3)
    - Semantic labels (1)
**kwargs : dict, optional
    Extra data products to pass to the parent Cluster3DParser

Returns
-------
np_voxels : np.ndarray
    (N, 3) array of [x, y, z] coordinates
np_features : np.ndarray
    (N, 2/14) array of features, minimally [voxel value, cluster ID].
    If `add_particle_info` is `True`, the additonal columns are
    [group ID, interaction ID, neutrino ID, particle type,
    group primary bool, interaction primary bool, vertex x, vertex y,
    vertex z, momentum, semantic type, particle ID]
meta : Meta
    Metadata of the parsed image

---
### FunctionDef: `process_run_info`

Process the run information.

Check the run information for duplicates and initialize a dictionary
which map (run, subrun, event) triplets onto entry index.

---
### FunctionDef: `process_single`

Converts the PPN output from a single entry into points of interests
for that entry.

Notes
-----
This function works both `torch.Tensor` and `np.ndarray` objects.

Parameters
----------
ppn_raw : Union[torch.Tensor, np.ndarray]
     Raw output of PPN
ppn_coords : Union[torch.Tensor, np.ndarray]
     Coordinates of the image at each PPN layer
ppn_masks : Union[torch.Tensor, np.ndarray]
     Predicted masks of at each PPN layer
ppn_ends : Union[torch.Tensor, np.ndarray], optional
     Raw logits from the end point classification layer of PPN
segmentation : Union[torch.Tensor, np.ndarray], optional
     Raw logits from the semantic segmentation network output
ghost : Union[torch.Tensor, np.ndarray], optional
     Raw logits from the ghost segmentation network output
selection : Union[torch.Tensor, np.ndarray], optional
     List of indexes to consider exclusively (e.g. to get PPN
     predictions within a list of clusters)

Returns
-------
Union[TensorBatch, List[np.ndarray]]
    (N, P) Tensor of predicted points with P divided between
    [batch_id, x, y, z, validity scores (2), occupancy, type scores (5),
     predicted type, endpoint type]

---
### FunctionDef: `process_single`

Match all the requested objects in a single category.

Parameters
----------
reco_objs : List[object]
    List of reconstructed objects
truth_objs : List[object]
    List of truth objects
matcher : MatchProcessor.Matcher
    Matching method and function
name : str
    Object type name
meta : Meta, optional
    Metadata information to convert position to index

---
### FunctionDef: `process_single_loss_config`

Process a loss configuration.

Parameters
----------
prefix : dict
    Name of the output type to apply the loss to
loss : Union[int, dict]
    Loss configuration
constructor : object
    Loss constructor function

---
### FunctionDef: `process_world`

Check on the number of available GPUs and what has been requested.

Parameters
----------
base : dict
    Base driver configuration dictionary
**kwargs : dict
    Other elements of the driver configuration
    Analysis script configurationdictionary

Returns
-------
distributed : bool
    If `True`, distribute the training process
world_size : int
    Number of devices to use in the distributed training process

---
### FunctionDef: `pur`

Assignment purity.

Parameters
----------
truth : np.ndarray
    (N) Set of true labels
pred : np.ndarray
    (N) Set of predicted labels
batch_ids : np.ndarray, optional
    (N) Batch IDs
per_cluster : bool, default True
    If `True`, computes the purity per predicted cluster, than averages it

Returns
-------
float
    Assignment purity

---
### FunctionDef: `pur_eff`

Assignment purity and efficiency.

Parameters
----------
truth : np.ndarray
    (N) Set of true labels
pred : np.ndarray
    (N) Set of predicted labels
batch_ids : np.ndarray, optional
    (N) Batch IDs
per_cluster : bool, default True
    If `True`, computes the metrics per predicted cluster, than averages them

Returns
-------
float
    Assignment purity
float
    Assignment efficiency

---
### FunctionDef: `pytest_addoption`

Defines testing command line arguments that can be passed to any
test scripts inside the general test directory.

---
### FunctionDef: `pytest_generate_tests`

Appends general parameters to all tests.

---
### FunctionDef: `query`

Gets the database information for a given run. If the run does not
exist in the list, pick the one closest but earlier than it.

Parameters
----------
run_id : int
    ID of the run to get the values for

Returns
-------
np.ndarray
    List of values per channel

---
### FunctionDef: `query`

Queries the LUT to get the calibration values for a set of points.

Parameters
----------
points: np.ndarry
    (N, 3) Coordinates of the points to query a calibration for

Returns
-------
np.ndarray
    Calibration constants

---
### ClassDef: `RandomSequenceBatchSampler`

Samples sequential batches randomly within the dataset.

---
### FunctionDef: `reader_factory`

Instantiates reader based on type specified in configuration under
`io.reader.name`. The name must match the name of a class under
`spine.io.readers`.

Parameters
----------
reader_cfg : dict
    Writer configuration dictionary

Returns
-------
object
    Writer object

Note
----
Currently the choice is limited to `HDF5Writer` only.

---
### ClassDef: `ReaderBase`

Parent reader class which provides common functions between all readers.

This class provides these basic functions:
1. Method to parse the requested file list or file list file into a list of
   paths to existing files (throws if nothing is found)
2. Method to produce a list of entries in the file(s) as selected by the
   provided parameters, checks that they exist (throws if they do not)
3. Essential `__len__` and `__getitem__` methods. Must define the
   `get` function in the inheriting class for both of them to work.

Attributes
----------
name : str
    Name of the reader, as requested in the configuration
num_entries : int
    Total number of entries in the files provided
entry_index : List[int]
    List of global indexes to cycle through
file_paths : List[str]
    List of files to read data from
file_offsets : List[int]
    Offsets between the global index and each individual file start index
file_index : List[int]
    Index of the file each entry in entry_index lives in
run_info : np.ndarray
    (run, subrun, event) triplets associated with each entry in the file list
run_map : Dict[Tuple[int], int]
    Maps each available (run, subrun, event) triplet onto an entry_index index

---
### FunctionDef: `rebuild_matrix`

Builds a confusion matrix from an entry-wise storage file.

Parameters
----------
data : pd.Dataframe
    Dataframe which contains the flattened matrix
num_classes : int, optional
    Number of classes to represent
mapping : dict, optional
    Mapping between the stored class and a redefined set of classes

---
### FunctionDef: `reco_end_dir`

Alias for `end_dir`, to match nomenclature in truth.

---
### FunctionDef: `reco_ke`

Alias for `ke`, to match nomenclature in truth.

---
### FunctionDef: `reco_ke`

Best-guess reconstructed kinetic energy in MeV.

Uses calorimetry for EM activity and this order for track:
- CSDA-based estimate if it is available
- MCS-based estimate if it is available
- Calorimetry if all else fails

Returns
-------
float
    Best-guess kinetic energy

---
### FunctionDef: `reco_length`

Alias for `length`, to match nomenclature in truth.

---
### FunctionDef: `reco_momentum`

Alias for `momentum`, to match nomenclature in truth.

---
### FunctionDef: `reco_momentum`

Best-guess reconstructed momentum in MeV/c.

Returns
-------
np.ndarray
    (3) Momentum vector

---
### FunctionDef: `reco_start_dir`

Alias for `start_dir`, to match nomenclature in truth.

---
### ClassDef: `RecoBase`

Base data structure shared among all reconstructed output classes.

---
### ClassDef: `RecoFragment`

Reconstructed fragment information.

Attributes
----------
primary_scores : np.ndarray
    (2) Array of softmax scores associated with secondary and primary

---
### ClassDef: `RecoInteraction`

Reconstructed interaction information.

---
### FunctionDef: `recombination_factor`

Calls the predefined recombination models to evaluate the
appropriate quenching factors.

Parameters
----------
dedx : Union[float, np.ndarray]
    Value or array of values of dEdx in MeV/cm
cosphi : Union[float, np.ndarray]
    Value or array of values of the cosine of the angle w.r.t. the
    drift direction (in [0,1]).

Returns
-------
Union[float, np.ndarray]
    Quenching factors in electrons/MeV

---
### ClassDef: `RecombinationCalibrator`

Applies a recombination correction factor to account for some of the
ionization electrons recombining with the Argon ions, which is an effect
that depends on the local rate of energy deposition and the angle of
the deposition trail (track) w.r.t. to the drift field.

Notes
-----
Must call the gain calibrator upstream, which converts the number of ADCs
to a number of observed ionization electrons.

---
### FunctionDef: `reconstruct_vertex_single`

Post-processor which reconstructs one vertex for each interaction
in the provided list.

Parameters
----------
inter : List[RecoInteraction, TruthInteraction]
    Reconstructed/truth interaction object

---
### ClassDef: `RecoParticle`

Reconstructed particle information.

Attributes
----------
pid_scores : np.ndarray
    (P) Array of softmax scores associated with each particle class
primary_scores : np.ndarray
    (2) Array of softmax scores associated with secondary and primary
ppn_ids : np.ndarray
    (M) List of indexes of PPN points associated with this particle
ppn_points : np.ndarray
    (M, 3) List of PPN points tagged to this particle
vertex_distance: float
    Set-to-point distance between all particle points and the parent
    interaction vertex. (untis of cm)
shower_split_angle: float
    Estimate of the opening angle of the shower. If particle is not a
    shower, then this is set to -1. (units of degrees)

---
### FunctionDef: `register_key`

Identify the dtype and shape objects to be dealt with.

Parameters
----------
data : dict
    Dictionary containing the information to be stored
key : string
    Dictionary key name

---
### FunctionDef: `regularization`

Implementation of regularization loss in Discriminative Loss
Inputs:
    cluster_means (torch.Tensor): output from find_cluster_means
Returns:
    reg_loss (float): computed regularization loss (see paper).

---
### FunctionDef: `regularization`

Implementation of regularization loss in Discriminative Loss
Inputs:
    cluster_means (torch.Tensor): output from find_cluster_means
Returns:
    reg_loss (float): computed regularization loss (see paper).

---
### FunctionDef: `regularization`

Implementation of regularization loss in Discriminative Loss
Inputs:
    cluster_means (torch.Tensor): output from find_cluster_means
Returns:
    reg_loss (float): computed regularization loss (see paper).

---
### ClassDef: `ResNetBlock`

ResNet Block.

---
### ClassDef: `ResNeXtBlock`

ResNeXt-type block with atrous convolutions.

Notes
-----
For vanilla resnext blocks, set `dilation=1` and others to default.

---
### FunctionDef: `restrict`

Function that restricts an incidence matrix of a graph
to the edges below a certain length.

If `classes` are specified, the maximum edge length must be provided
for each possible combination of node classes.

Parameters
----------
edge_index : np.ndarray
    (2, E) Tensor of edges
edge_counts : np.ndarray
    (B) : Number of edges in each entry of the batch
dist_mat : np.ndarray
    (C, C) Tensor of pair-wise cluster distances
classes : TensorBatch, optional
    (C) List of class for each cluster in the graph

Returns
-------
np.ndarray
    (2,E) Restricted tensor of edges

---
### FunctionDef: `restrict_clusts`

Restricts a cluster list against a list of shapes.

Parameters
----------
clusts : IndexBatch
    List of clusters to aggregate using GrapPA
clust_shapes : TensorBatch
    Semantic type of each of the clusters
shapes : List[int]
    List of semantic shapes to restrict to

Returns
-------
clusts : IndexBatch
    Restricted list of clusters
clust_shapes : TensorBatch
    Restricted list of semantic types
shape_index : np.ndarray
    List of indexes used to restrict the original cluster list

---
### FunctionDef: `run`

Execute a model in one or more processes.

Parameters
----------
cfg : dict
    Full driver/trainer configuration

---
### FunctionDef: `run`

Loop over the requested number of iterations, process them.

---
### FunctionDef: `run_calibration`

Run the calibration algorithm.

This converts the raw charge values in ADC to energy depositions
expressed in MeV. It applies gain, recombination, transparency
and electron lifetime corrections.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
sources : TensorBatch, optional
    (N, 2) tensor of module/tpc pair for each voxel
energy_label : TensorBatch, optional
    (N, 1 + D + 1) Tensor of true energy deposition values
    - 1 is the energy deposition value in each voxel
meta : Meta, optional
    Image metadata information
run_info : List[RunInfo], optional
    Object containing information about the run, subrun and event

Returns
-------
TensorBatch
    (N, 1 + D + N_f) tensor of calibrated voxel/value pairs

---
### FunctionDef: `run_crt_tpc_matching`

Call matcha's match-making function

Parameters
----------
tracks: list of matcha.Track instances
crthits: list of matcha.CRTHit instances

Returns
-------
list of matcha.MatchCandidate instances containing matched Track and
CRTHit objects

---
### FunctionDef: `run_deghosting`

Run the deghosting algorithm.

This removes points that are artifacts of the tomographic
reconstruction. This is only relevant for detectors producing 2D
projections of an event. If requested, charge is rescaled according
to the deghosting mask.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
sources : TensorBatch, optional
    (N, 2) tensor of module/tpc pair for each voxel
seg_label : TensorBatch, optional
    (N, 1 + D + 1) Tensor of segmentation labels
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels

Returns
-------
TensorBatch
    (N, 1 + D + N_f) tensor of deghosted voxel/value pairs

---
### FunctionDef: `run_flash_matching`

Drive the OpT0Finder flash matching.

Returns
-------
List[flashmatch::FlashMatch_t]
    List of matches

---
### FunctionDef: `run_fragmentation`

Run the fragmentation algorithm, i.e. the dense clustering step.

This breaks down each topological class individually into a set of
fragments, each composed of contiguous voxels which belong to a single
particle instance, but do not necessarily make up the whole instance.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels

---
### FunctionDef: `run_grappa`

Run the GNN-based particle aggregator.

Parameters
----------
prefix : str
    Name of the aggregation step
model : GraPA
    GraPA model to execute for this aggregation step
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
clusts : IndexBatch
    List of clusters to aggregate using GrapPA
clust_shapes : TensorBatch
    Semantic type of each of the clusters
clust_primaries : IndexBatch
    List of primary fragments associated with each input cluster
coord_label : TensorBatch, optional
    (N, 1 + D + 6) Array of label particle end points
aggregate_shapes : bool, default False
    Combine shapes to give a shape to the aggregated object
shape_use_primary : bool, default False
    Use primary shape as the group shape
point_use_primary : bool, default False
    Use the primary fragment to get the points
retain_primaries : bool, default False
    Retain the primary cluster in the aggregated group

Returns
-------
groups : IndexBatch
    List of cluster groups aggregated using GrapPA
group_shapes : TensorBatch
    Semantic type of each of the cluster groups
group_primaries : IndexBatch
    List of primary clusters for each group
shape_index : np.ndarray
    List of indexes used to restrict the original cluster list

---
### FunctionDef: `run_inter_aggregation`

Run the interaction aggreation step.

This step gathers particles into complete interaction instances.

In the process of interaction aggregation, other tasks may be performed:
- Particle identification
- Primary tagging (particle coming from the interaction vertex)
- Orientation tagging (order start/end points of particles)
- Vertex reconstruction

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels
coord_label : TensorBatch, optional
    (N, 1 + D + 6) Array of label particle end points

---
### FunctionDef: `run_part_aggregation`

Run the particle aggreation step.

This step gathers particle fragments into complete particle instances.
It either aggregates shower and track fragments independently or
jointly into a single step.

In the process of shower aggregation, shower primaries can
be identified.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels
coord_label : TensorBatch, optional
    (N, 1 + D + 6) Array of label particle end points

---
### FunctionDef: `run_segmentation_ppn`

Run the semantic segmentation and the point proposal algorithms.

This classifies each individual voxel in the image into different
particle topological categories and identifies poins of interest,
namely track end points and shower fragment start points.

Parameters
----------
data : TensorBatch
    (N, 1 + D + N_f) tensor of voxel/value pairs
seg_label : TensorBatch, optional
    (N, 1 + D + 1) Tensor of segmentation labels
clust_label : TensorBatch, optional
    (N, 1 + D + N_c) Tensor of cluster labels

---
### FunctionDef: `run_single`

Execute a model on a single process.

Parameters
----------
cfg : dict
    Full driver/trainer configuration

---
### ClassDef: `RunInfo`

Run information related to a specific event.

Attributes
----------
run : int
    Run ID
subrun : int
    Sub-run ID
event : int
    Event ID

---
### ClassDef: `RunInfoParser`

Parse run information (run, subrun, event number).

.. code-block. yaml

    schema:
      run_info:
        parser: run_info
        sparse_event: sparse3d_pcluster

---
### FunctionDef: `sample_edges`

Subsample a set number of edges from each edge label class.

Parameters
----------
edge_scores : torch.Tensor
    Edge score predictions
edge_label : torch.Tensor
    Edge labels

Returns
-------
edge_scores : torch.Tensor
    Subsampled edge predictions
edge_label : torch.Tensor
    Subsampled edge labels

---
### FunctionDef: `sampler_factory`

Instantiates sampler based on type specified in configuration under
`io.sampler.name`. The name must match the name of a class under
`spine.io.sample`.

Parameters
----------
sampler_cfg : dict
    Sampler configuration dictionary
dataset : torch.utils.data.Dataset
    Dataset to sample from
minibatch_size : int
    Number of data samples to load per iteration, per process
distributed: bool, default False
    If True, initialize as a DistributedSampler
num_replicas : int, default 1
    Total number of processes running the sampler
rank : int, default 0
    Unique identifier of the process sampling data

Returns
-------
Union[torch.utils.data.Sampler, torch.utils.data.DistributedSampler]
    Initialized sampler

---
### FunctionDef: `save_state`

Save the model state.

Save three things from the model:
- global_step (iteration)
- state_dict (model parameter values)
- optimizer (optimizer parameter values)

Parameters
----------
iteration : int
    Iteration step index

---
### ClassDef: `SaveAna`

Class which simply saves reconstructed objects (and their matches).

---
### FunctionDef: `sbd`

Compute the Symmetric Best Dice (SBD) score between two sets of labels.

Parameters
----------
truth : np.ndarray
    (N) Set of true labels
pred : np.ndarray
    (N) Set of predicted labels
batch_ids : np.ndarray, optional
    (N) Batch IDs

Returns
-------
float
    Symmetric best dice value

---
### FunctionDef: `scalar_dict`

Returns the data class attributes as a dictionary of scalars.

This is useful when storing data classes in CSV files, which expect
a single scalar per column in the table.

Parameters
----------
attrs : List[str], optional
    List of attribute names to include in the dictionary. If not
    specified, all the keys are included.
lengths : Dict[str, int], optional
    Specifies the length of variable-length attributes
lite : bool, default False
    If `True`, the `_lite_skip_attrs` are dropped

---
### FunctionDef: `scatter_boxes`

Function which produces a list of plotly traces of boxes given a list of
coordinates and a box dimension.

This function assumes that the coordinates represent the lower bounds of
the voxels they point at. This follows the `MinkowskiEngine` convention,
which is the package used for space convolutions. This can be used to
represent the PPN regions of interest in a space compressed by a factor
(b_x, b_y, b_z) from the original image resolution.

Parameters
----------
coords : np.ndarray
    (N, 3) Coordinates of in multiples of box lengths in each dimension
dimension : Union[float, np.ndarray]
    Dimensions of the boxes. Specify it as either a single number (for
    cubes) or an array of values in each dimension, i.e. (b_x, b_y, b_z)
draw_faces : bool, default True
    Weather or not to draw the box faces, or only the edges
color : Union[str, np.ndarray], default 'orange'
    Color of boxes or list of color of boxes
hovertext : Union[int, str, np.ndarray], optional
    Text associated with every box or each box
linewidth : int, default 2
    Width of the box edge lines
shared_legend : bool, default True
    If True, the plotly legend of all boxes is shared as one
**kwargs : dict, optional
    List of additional arguments to pass to
    :class:`plotly.graph_objs.Scatter3D` or
    :class:`plotly.graph_objs.Mesh3D`, depending on what the `draw_faces`
    parameter is set to.

Returns
-------
Union[List[plotly.graph_objs.Scatter3D], List[plotly.graph_objs.Mesh3D]]
    Box traces

---
### FunctionDef: `scatter_clusters`

Arranges points in clusters and scatters them and their cluster labels.

Produces :class:`plotly.graph_objs.Scatter3d` trace object to be drawn
in plotly. The object is nested to be fed directly to a
:class:`plotly.graph_objs.Figure` or :func:`plotly.offline.iplot`.
All of the regular plotly parameters are available.

Parameters
----------
points : np.ndarray
    (N, 3) array of N points of (..., x, y, z,...) coordinate information
clusts : List[np.ndarray]
    (C) List of cluster indexes
color : Union[str, np.ndarray], optional
    Color of markers or (N/C) list of color of markers or clusters
hovertext : Union[List[str], List[int]], optional
    (N/C) List of labels associated with each marker or cluster
single_trace : bool, default False
    If `True`, combine all clusters into a single plotly trace
name : Union[str, List[str]], optional
    Name of the clusters or of each cluster
mode : str, default 'scatter'
    Drawing mode; one of 'circle', 'scatter', 'ellipsoid', 'cone' or 'hull'
cmin : float, optional
    Minimum value along the color scale
cmax : float, optional
    Maximum value along the color scale
shared_legend : bool, default True
    If `True` put all cluster traces under a single shared legend
**kwargs : dict, optional
    List of additional arguments to pass to plotly.graph_objs.Scatter3D

Returns
-------
List[go.Scatter3d]
    (1/C) List with one combined trace or one trace per cluster

---
### FunctionDef: `scatter_particles`

Builds a graph of true particles in the image.

Function which returns a graph object per true particle in the
particle list, provided that the particle deposited energy in the
detector which appears in the cluster_label tensor.

Parameters
----------
cluster_label : np.ndarray
    (N, M) Tensor of pixel coordinates and their associated cluster ID
particles : List[Particle]
    (P) List of true particle objects
part_col : int
    Index of the column in the label tensor that contains the particle ID
**kwargs : dict, optional
    List of additional arguments to pass to plotly.graph_objs.Scatter3D that
    make up the output list

Returns
-------
List[plotly.graph_objs.Scatter3D]
    List of particle traces

---
### FunctionDef: `scatter_points`

Scatters points and their labels.

Produces :class:`plotly.graph_objs.Scatter3d` or
:class:`plotly.graph_objs.Scatter` trace object to be drawn in plotly. The
object is nested to be fed directly to a :class:`plotly.graph_objs.Figure`
or :func:`plotly.offline.iplot`. All of the regular plotly parameters are
available.

It can scatter points individually (default `mode`) or it can draw lines
between the provided points (`mode='lines'` option).

Parameters
----------
points : np.ndarray
    (N, 2+) array of N points of (..., x, y, [z],...) coordinate information
color : Union[str, np.ndarray], optional
    Color of markers/lines or (N) list of color of markers/lines
markersize : float, default 2
    Marker size
linewidth : float, default 2
    Line width
colorscale : Union[str, List[str], List[List[float, str]], optional
    Plotly colorscale specifier for the markers
cmin : Union[int, float], optional
    Minimum of the color range
cmax : Union[int, float], optional
    Maximum of the color range
opacity : float
    Marker opacity
hovertext : Union[List[str], List[int]], optional
    (N) List of labels associated with each marker
hovertemplate : str, optional
    Hover information formatting
dim : int, default 3
    Dimension (can either be 2 or 3)
mode : str, default 'markers'
    Drawing mode
marker : dict, optional
    Marker style configuration dictionary
line : dict, optional
   Line style configuration dictionary
**kwargs : dict, optional
    List of additional arguments to pass to plotly.graph_objs.Scatter3D

Returns
-------
List[go.Scatter3d]
    (1) List with one graph of the input points

---
### FunctionDef: `search_and_replace`

Recursively parse config for all instances of (key : val) pairs
and replace it with new value.

---
### ClassDef: `SEBlock`

Squeeze and Excitation block.

---
### FunctionDef: `seed`

Sets the numpy random seed for all Numba jitted functions.

Note that setting the seed using `np.random.seed` outside a Numba jitted
function does *not* set the seed of Numba functions.

Parameters
----------
seed : int
    Random number generator seed

---
### ClassDef: `SegmentAna`

Class which computes and stores the necessary data to build a
semantic segmentation confusion matrix.

---
### ClassDef: `SegmentationLoss`

Loss definition for semantic segmentation.

For a regular flavor UResNet, it is a cross-entropy loss.
For deghosting, it depends on a configuration parameter `ghost`:

- If `ghost=True`, we first compute the cross-entropy loss on the ghost
  point classification (weighted on the fly with sample statistics). Then we
  compute a mask = all non-ghost points (based on true information in label)
  and within this mask, compute a cross-entropy loss for the rest of classes.

- If `ghost=False`, we compute a N+1-classes cross-entropy loss, where N is
  the number of classes, not counting the ghost point class.

See Also
--------
:class:`UResNetSegmentation`

---
### FunctionDef: `select_particle_pairs`

Select particle pairs for logging (only for mpv/nu interactions)

---
### ClassDef: `SENet`

UNet Type encoder-decoder network, with atrous convolutions and
resnext-type blocks.

---
### FunctionDef: `sequential_cluster_distances`

Order clusters in order of distance from a starting point, compute
the distances between successive clusters. 

Parameters
----------
points : np.ndarray
    (N, 3) List of track cluster point coordinates
labels : np.ndarray
    (N) Track chunk labels
start_point : np.ndarray
    (3) Start point of the track cluster

---
### ClassDef: `SequentialBatchSampler`

Samples batches sequentially within the dataset.

---
### ClassDef: `SEResNetBlock`

Squeeze and Excitation ResNet block.

---
### FunctionDef: `set_latex_size`

Returns optimal figure dimension for a latex plot, depending on
the requested width.

Parameters
----------
width : int
    Width of the page in points (pixels)
fraction : float, default 1
    Fraction of the page width used by the figure

Returns
-------
width : float
    Width of the figure in inches
height : float
    Height of the figure in inches

---
### FunctionDef: `set_log_dir`

Simply reset the base log directory to another one.

Parameters
----------
log_dir, str
    Path to the parent directory of all the log files

---
### FunctionDef: `set_precision`

Casts all the vector attributes to a different precision.

Parameters
----------
int : default 4
    Precision in number of bytes (half=2, single=4, double=8)

---
### FunctionDef: `setup_cnn_configuration`

Base function for global network parameters (CNN-based models).

This avoids repeating the same base configuration parsing everywhere.
For example, typical usage would be:

.. code-block:: python

    class UResNetEncoder(torch.nn.Module):
        def __init__(self, cfg):
            super().__init__()
            setup_cnn_configuration(self, **cfg)

Parameters
----------
reps : int
    Number of time convolutions are repeated at each depth
depth : int
    Depth of the CNN (number of downsampling)
filters : int
    Number of input filters
input_kernel : int, default 3
    Input kernel size
data_dim : int, default 3
    Dimension of the input image data
num_input : int, default 1
    Number of features in the input image
allow_bias : bool, default False
    Whether to allow biases in the convolution and linear layers
activation : union[str, dict], default 'relu'
    Activation function configuration
normalization : union[str, dict], default 'batch_norm'
    Normalization function configuration
spatial_size : int, optional
    Size of the input image in number of voxels per data_dim. This is only
    necessary when passing the normalized coordinates as features.

---
### FunctionDef: `setup_ddp`

Sets up the DistributedDataParallel environment.

---
### FunctionDef: `shape`

Shape of the underlying data.

Returns
-------
tuple
    Tuple of sizes in each dimension

---
### ClassDef: `ShapeEnum`

Enumerates all possible shape values.

---
### ClassDef: `ShowerMultiArmCheck`

Check whether given primary electron candidate is likely
to be a merged multi-particle shower.

This processor computes direction vectors of the shower points
from the shower start and performs DBSCAN clustering on the unit sphere
using the cosine distance metric. If there are more than one cluster that
has a mean direction vector outside a certain angular threshold, the
shower is considered to be a multi-arm shower and is rejected as 
a valid primary electron candidate.

NOTE: This processor can only change reco electron shower pid to
photon pid depending on the angle threshold. 

---
### ClassDef: `ShowerStartDEdxAna`

This analysis script computes the dE/dx value within some distance
from the start point of an EM shower object.

This is a useful diagnostic tool to evaluate the calorimetric separability
of different EM shower types (electron vs photon), which are expected to
have different dE/dx patterns near their start point.

---
### ClassDef: `ShowerStartpointCorrectionProcessor`

Correct the startpoint of the primary EM shower by 
finding the closest point to the vertex.

---
### FunctionDef: `sigmoid_ce_loss`

Args:
    inputs: A float tensor of arbitrary shape.
            The predictions for each example.
    targets: A float tensor with the same shape as inputs. Stores the binary
             classification label for each element in inputs
            (0 for the negative class and 1 for the positive class).
Returns:
    Loss tensor

---
### ClassDef: `SingleParticleEnergyParser`

Get the first true particle's kinetic energy.

.. code-block. yaml

    schema:
      image_energy:
        parser: single_particle_energy
        particle_event: particle_pcluster

---
### ClassDef: `SingleParticlePIDParser`

Get the first true particle's species.

.. code-block. yaml

    schema:
      image_pid:
        parser: single_particle_pid
        particle_event: particle_pcluster

---
### FunctionDef: `size`

Total number of voxels that make up the object.

Returns
-------
int
    Total number of voxels in the object

---
### FunctionDef: `size_adapt`

Total number of voxels that make up the object in the adapted tensor.

Returns
-------
int
    Total number of voxels in the object

---
### FunctionDef: `size_g4`

Total number of voxels that make up the object in the Geant4 tensor.

Returns
-------
int
    Total number of voxels in the object

---
### FunctionDef: `skip_attrs`

Fetches the list of attributes to not store to file.

Returns
-------
List[str]
    List of attributes to exclude from the storage process

---
### FunctionDef: `softmax`

Numba implementation of `scipy.special.softmax(x, axis)`.

Parameters
----------
x : np.ndarray
    (N,M) array of values
axis : int
    Array axis ID

Returns
-------
np.ndarray
    (N,M) Array of softmax scores

---
### FunctionDef: `source_modes`

Dictionary which makes the correspondance between the name of a true
object source attribute with the underlying source tensor it points to.

Returns
-------
Dict[str, str]
    Dictionary of (attribute, key) mapping for point sources

---
### ClassDef: `Sparse2DParser`

Class that retrieves and parses a 2D sparse tensor.

.. code-block. yaml

    schema:
      input_data:
        parser: sparse2d
        sparse_event_list:
          - sparse2d_pcluster_0
          - sparse2d_pcluster_1
          - ...
        projection_id: 0

---
### ClassDef: `Sparse3DAggregateParser`

Class that aggregates features from multiple sparse tensors

.. code-block. yaml

    schema:
      charge_label:
        parser: sparse3d_aggr
        aggr: sum
        sparse_event_list:
          - sparse3d_reco_cryoE_rescaled
          - sparse3d_reco_cryoW_rescaled

---
### ClassDef: `Sparse3DChargeRescaledParser`

Class that convert a tensor containing semantics to binary ghost labels.

.. code-block. yaml

    schema:
      input_rescaled:
        parser: sparse3d_charge_rescaled
        sparse_event_semantics: sparse3d_semantics

---
### ClassDef: `Sparse3DGhostParser`

Class that convert a tensor containing semantics to binary ghost labels.

.. code-block. yaml

    schema:
      ghost_label:
        parser: sparse3d_ghost
        sparse_event_semantics: sparse3d_semantics

---
### ClassDef: `Sparse3DParser`

Class that retrieves and parses a 3D sparse tensor.

.. code-block. yaml

    schema:
      input_data:
        parser: sparse3d
        sparse_event_list:
          - sparse3d_pcluster_0
          - sparse3d_pcluster_1
          - ...

---
### ClassDef: `SparseResidualEncoder`

Encoder for sparse tensor feature extraction.

---
### FunctionDef: `spatial_embedding_loss`

Compute spatial centroid regression loss.

INPUTS:
    - sp_emb (N x D)
    - groups (N)
    - ft_centroids (N_c X F)

---
### ClassDef: `SPICEFragmentManager`

Full chain model fragment mananger for SPICE Clustering

---
### ClassDef: `SPICELoss`

Loss function for Proposal-Free Mask Generators.

---
### ClassDef: `SPICELoss`

Loss function for Sparse Spatial Embeddings Model, with fixed
centroids and symmetric gaussian kernels.

---
### FunctionDef: `split`

Breaks up the index batch into its constituents.

Returns
-------
List[List[Union[np.ndarray, torch.Tensor]]]
    List of list of indexes per entry in the batch

---
### FunctionDef: `split`

Breaks up the index batch into its constituents.

Returns
-------
List[Union[np.ndarray, torch.Tensor]]
    List of one index per entry in the batch

---
### FunctionDef: `split`

Breaks up the tensor batch into its constituents.

Returns
-------
List[Union[np.ndarray, torch.Tensor]]
    List of one tensor per entry in the batch

---
### FunctionDef: `split`

Migrate all points to a target module, organize them by module ID.

Parameters
----------
points : np.ndarray
    (N, 3) Set of point coordinates
target_id : int
    Module ID to which to move the point cloud
sources : np.ndarray, optional
    (N, 2) Array of [module ID, tpc ID] pairs, one per voxel
meta : Meta, optional
    Meta information about the voxelized image. If provided, the
    points are assumed to be provided in voxel coordinates.

Returns
-------
np.ndarray
    (N, 3) Shifted set of points
List[np.ndarray]
    List of index of points that belong to each module

---
### FunctionDef: `split_angles`

Split 3D angles between vectors to two 2D projected angles

Parameters
----------
theta : np.ndarray
    Array of 3D angles in [0, np.pi]

Returns
-------
float
    Frist array of 2D angle in [-np.pi, np.pi]
float
    Second array of 2D angle in [-np.pi, np.pi]

---
### FunctionDef: `splits`

Boundaries needed to split the data into its constituents.

Returns
-------
Union[np.ndarray, torch.Tensor]
    (B-1) One split per batch boundary

---
### ClassDef: `SPP`

Spatial Pyramid Pooling.

PSPNet (Pyramid Scene Parsing Network) uses vanilla SPPs, while
DeeplabV3 and DeeplabV3+ uses ASPP (atrous versions).

Default parameters will construct a global average pooling + unpooling
layer which is done in ParseNet.

---
### FunctionDef: `standard_forward`

Forwarding operation for standard dropout segmentation network.

---
### FunctionDef: `start`

Starts a stopwatch for a unique key.

Parameters
----------
key : Union[str, List[str]]
    Key or list of keys for which to start the clock

---
### FunctionDef: `start`

Time when the stopwatch was last started.

---
### FunctionDef: `start_dir`

Converts the initial momentum to a direction vector.

Returns
-------
np.ndarray
    (3) Start direction vector

---
### FunctionDef: `start_dir`

Converts the initial momentum to a direction vector.

Returns
-------
np.ndarray
    (3) Start direction vector

---
### FunctionDef: `step`

Performs a single optimization step.

Parameters
----------
closure : callable, optional
    A closure that reevaluates the model and returns the loss

---
### FunctionDef: `step`

Performs a single optimization step.
Arguments:
    closure (callable, optional): A closure that reevaluates the model
        and returns the loss.

---
### FunctionDef: `step_energy_loss_lar`

Steps the initial energy of a particle down by pushing it through
steps of dx of liquid argon. If `num_steps` is not specified, it will
iterate until the particle kinetic energy reaches 0.

Parameters
----------
T0 : float
    Initial kinetic energy in MeV
M : float
    Particle mass in MeV/c^2
dx : float
    Step size in cm
z : int, default 1
    Impinging partile charge in multiples of electron charge
num_steps : int, optional
    If specified, only step a maximum of `num_steps` times

Returns
-------
np.array
    Array of kinetic energies at each step

---
### FunctionDef: `stop`

Stops a stopwatch for a unique key.

Parameters
----------
key : str
    Key for which to stop the clock

---
### FunctionDef: `stop`

Time when the stopwatch was last stopped.

---
### ClassDef: `Stopwatch`

Simple class to hold timing information for a specific process.

---
### ClassDef: `StopwatchManager`

Simple class to organize various time measurements.

---
### FunctionDef: `store`

Stores an `ndarray` in the file and stores its mapping in the event
dataset.

Parameters
----------
out_file : h5py.File
    HDF5 file instance
event : dict
    Dictionary of objects that make up one event
key: str
    Name of the dataset in the file
array : np.ndarray
    Array to be stored

---
### FunctionDef: `store_flat`

Stores a concatenated list of arrays in the file and stores its
index mapping in the event dataset to break them.

Parameters
----------
out_file : h5py.File
    HDF5 file instance
event : dict
    Dictionary of objects that make up one event
key: str
    Name of the dataset in the file
array_list : list(np.ndarray)
    List of arrays to be stored

---
### FunctionDef: `store_jagged`

Stores a jagged list of arrays in the file and stores an index
mapping for each array element in the event dataset.

Parameters
----------
out_file : h5py.File
    HDF5 file instance
event : dict
    Dictionary of objects that make up one event
key: str
    Name of the dataset in the file
array_list : list(np.ndarray)
    List of arrays to be stored

---
### FunctionDef: `store_objects`

Stores a list of objects with understandable attributes in the file
and stores its mapping in the event dataset.

Parameters
----------
out_file : h5py.File
    HDF5 file instance
event : dict
    Dictionary of objects that make up one event
key: str
    Name of the dataset in the file
array : np.ndarray
    Array of objects or dictionaries to be stored
obj_dtype : list
    List of (key, dtype) pairs which specify what's to store
lite : bool
    If `True`, store the lite version of objects

---
### FunctionDef: `submatrix`

Numba implementation of matrix subsampling.

Parameters
----------
x : np.ndarray
    (N,M) array of values
index1 : np.ndarray
    (N') array of indices along axis 0 in the input matrix
index2 : np.ndarray
    (M') array of indices along axis 1 in the input matrix

Returns
-------
np.ndarray
    (N',M') array of values from the original matrix

---
### FunctionDef: `sumsq_evd_loss`

Negative log loss for Dirichlet prior evidential learning.

INPUTS:
    - alpha (FloatTensor): N x C concentration parameters, 
    where C is the number of class labels.
    - y (FloatTensor): N x C one-hot encoded class labels

RETURNS:
    - loss (FloatTensor): N x 1 non-reduced loss for each example. 

---
### ClassDef: `TemplateAna`

Description of what the analysis script is supposed to be doing.

---
### ClassDef: `TemplateParticleIdentifier`

Class which uses dE/dx templates to do particle identification.

The basics of template-based PID are as follows:
- Chunk a track into chunks
- Identify the dE/dx of the tracks in each chunk
- Try to match the dE/dx profile to a known particle template

---
### ClassDef: `TemplateProcessor`

Description of what the post-processor is supposed to be doing.

---
### FunctionDef: `tensor`

Alias for the underlying data stored.

Returns
-------
Union[np.ndarray, torch.Tensor, ME.SparseTensor]
    Underlying tensor of data

---
### ClassDef: `TensorBatch`

Batched tensor with the necessary methods to slice it.

---
### FunctionDef: `test_bootstrap_sampler`

Tests the bootstrap batch sampler.

---
### FunctionDef: `test_collate_edge_index`

Tests the collation of edge indexes.

---
### FunctionDef: `test_collate_list`

Tests the collation of simple lists.

---
### FunctionDef: `test_collate_scalar`

Tests the collation of scalar values.

---
### FunctionDef: `test_collate_sparse`

Tests the collation of sparse tensors.

---
### FunctionDef: `test_hdf5_reader`

Tests the loading of a LArCV file.

---
### FunctionDef: `test_hdf5_writer`

Tests the HDF5 writer.

---
### FunctionDef: `test_larcv_dataset`

Tests a torch dataset based on LArCV data.

Most of the functions of this dataset are shared with the underlying
:class:`LArCVReader` class which is tested elsewhere.

---
### FunctionDef: `test_larcv_reader`

Tests the loading of a LArCV file.

---
### FunctionDef: `test_loader`

Tests the loading of data using a full IO configuration.

---
### FunctionDef: `test_model_construction`

Tests whether a model and its loss can be constructed.

---
### FunctionDef: `test_model_forward`

Test whether a model can be trained.
Using only numpy input arrays, should also test with parsers running.

Parameters
----------
config: dict
    Generated by a fixture above, dummy config to allow networks to run.
    It is mostly empty, we rely on networks default config.
N: int
    Spatial size
num_voxels_low: int, optional
    Lower boundary for generating (random) number of voxels.
num_voxels_high: int, optional
    Upper boundary for generating (random) number of voxels.

---
### FunctionDef: `test_model_full`

Tests whether a model can be trained.
Including parsers and trainval in the execution.

Parameters
----------
config: dict
    Generated by a fixture above, dummy config to allow networks to run.
    It is mostly empty, we rely on networks default config.

---
### FunctionDef: `test_parse_cluster2d`

Tests the parsing of LArCV 2D sparse data organized in a group.

---
### FunctionDef: `test_parse_cluster3d`

Tests the parsing of LArCV 3D sparse data organized in a group.

---
### FunctionDef: `test_parse_cluster3d_multi`

Tests the parsing of LArCV 3D sparse data organized in a group.

---
### FunctionDef: `test_parse_cluster3d_rescale`

Tests the parsing of LArCV 3D sparse data organized in a group.

---
### FunctionDef: `test_parse_crthits`

Tests the parsing of a list of CRT hits.

---
### FunctionDef: `test_parse_crthits`

Tests the parsing of a list of CRT hits.

---
### FunctionDef: `test_parse_flashes`

Tests the parsing of a list of list of optical flashes.

---
### FunctionDef: `test_parse_flashes`

Tests the parsing of a list of optical flashes.

---
### FunctionDef: `test_parse_meta2d`

Tests the parsing of metadata for 2D sparse events.

---
### FunctionDef: `test_parse_meta3d`

Tests the parsing of metadata for 3D sparse events.

---
### FunctionDef: `test_parse_neutrinos`

Tests the parsing of LArCV neutrino information.

---
### FunctionDef: `test_parse_particle_coordinates`

Tests the parsing of LArCV particle coordinates (GrapPA
end cluster end points label for standalone training).

---
### FunctionDef: `test_parse_particle_energy`

Tests the parsing of LArCV single particle energy parser.

---
### FunctionDef: `test_parse_particle_graph`

Tests the parsing of LArCV particle information into a set of
parentage relations.

---
### FunctionDef: `test_parse_particle_pid`

Tests the parsing of LArCV single particle PID parser.

---
### FunctionDef: `test_parse_particle_points`

Tests the parsing of LArCV particle points (PPN labels).

---
### FunctionDef: `test_parse_particles`

Tests the parsing of LArCV particle information.

---
### FunctionDef: `test_parse_run_info`

Tests the parsing of the run info of 3D sparse events.

---
### FunctionDef: `test_parse_spars3d_rescale`

Tests the parsing of 3D LArCV sparse data into a set of rescaled charges.

This parser takes 6 values (3 charges, 3 indexes) and combines this
with segementation labels to produce a single rescaled charge feature.

---
### FunctionDef: `test_parse_sparse2d`

Tests the parsing of LArCV 2D sparse data.

---
### FunctionDef: `test_parse_sparse2d_list`

Tests the parsing of a LArCV 2D sparse data list (multi-features).

---
### FunctionDef: `test_parse_sparse3d`

Tests the parsing of LArCV 3D sparse data.

---
### FunctionDef: `test_parse_sparse3d_ghost`

Tests the parsing of LArCV 3D sparse semantic labels to ghost labels.

---
### FunctionDef: `test_parse_sparse3d_list`

Tests the parsing of a LArCV 3D sparse data list (multi-features).

---
### FunctionDef: `test_parse_trigger`

Tests the parsing of trigger information.

---
### FunctionDef: `test_random_sequence_sampler`

Tests the random sequence batch sampler.

---
### FunctionDef: `test_sequential_sampler`

Tests the sequential batch sampler.

---
### ClassDef: `Time`

Simple dataclass to hold time information.

Attributes
----------
wall : float, optional
     Wall time
cpu : float, optional
     CPU time

---
### FunctionDef: `time`

Returns the time recorded since the last start.

Parameters
----------
key : str
    Key for which to return the time

Returns
-------
Time
    Execution time of one iteration of a process

---
### FunctionDef: `time`

Time between the last start and the last stop.

---
### FunctionDef: `time_sum`

Returns the sum of times recorded between each start/stop pairs.

Parameters
----------
key : str
    Key for which to return the time

Returns
-------
Time
    Execution time of all iterations of a process so far

---
### FunctionDef: `time_sum`

Sum of times between all watch starts en stops.

---
### FunctionDef: `times`

Returns the times for each of the stopwatches as a dictionary.

Returns
-------
Dict[str, Time]
    Execution time of one iteration of each process

---
### FunctionDef: `times_sum`

Returns the times for each of the stopwatches as a dictionary.

Returns
-------
Dict[str, Time]
    Execution time of all iterations of each process so far

---
### FunctionDef: `timing`

Function which wraps any function and times it.

Parameters
----------
fn : callable
    Function to time

Returns
-------
callable
    Timed function

---
### FunctionDef: `to_cm`

Converts pixel coordinates to detector coordinates in cm.

Parameters
----------
coords : np.ndarray
    (N, 2/3) Input pixel coordinates
center : bool, default False
    If `True`, offset the input coordinates by half a pixel size. This
    makes sense to provide unbiased coordinates when converting indexes.

Returns
-------
np.ndarray
    Detector coordinates in cm

---
### FunctionDef: `to_cm`

Converts the coordinates of the positional attributes to cm.

Parameters
----------
meta : Meta
    Metadata information about the rasterized image

---
### FunctionDef: `to_cm`

Converts the pixel coordinates of the tensor to cm.

Parameters
----------
meta : Meta
    Metadata information about the rasterized image

---
### FunctionDef: `to_numpy`

Cast underlying index to a `np.ndarray` and return a new instance.

Returns
-------
TensorBatch
    New `TensorBatch` object with an underlying np.ndarray tensor.

---
### FunctionDef: `to_numpy`

Cast underlying index to a `np.ndarray` and return a new instance.

Returns
-------
TensorBatch
    New `TensorBatch` object with an underlying np.ndarray tensor.

---
### FunctionDef: `to_numpy`

Cast underlying tensor to a `np.ndarray` and return a new instance.

Returns
-------
TensorBatch
    New `TensorBatch` object with an underlying np.ndarray tensor.

---
### FunctionDef: `to_px`

Converts detector coordinates in cm to pixel coordinates.

Parameters
----------
coords : np.ndarray
    (N, 2/3) Input detector coordinates
floor : bool, default False
    If `True`, converts pixel coordinates to indexes (floor function)

Returns
-------
np.ndarray
    Pixel coordinates

---
### FunctionDef: `to_px`

Converts the coordinates of the positional attributes to pixel.

Parameters
----------
meta : Meta
    Metadata information about the rasterized image

---
### FunctionDef: `to_px`

Converts the coordinates of the tensor to pixel indexes.

Parameters
----------
meta : Meta
    Metadata information about the rasterized image

---
### FunctionDef: `to_tensor`

Cast underlying index to a `torch.tensor` and return a new instance.

Parameters
----------
dtype : torch.dtype, optional
    Data type of the tensor to create
device : torch.device, optional
    Device on which to put the tensor

Returns
-------
TensorBatch
    New `TensorBatch` object with an underlying np.ndarray tensor.

---
### FunctionDef: `to_tensor`

Cast underlying index to a `torch.tensor` and return a new instance.

Parameters
----------
dtype : torch.dtype, optional
    Data type of the tensor to create
device : torch.device, optional
    Device on which to put the tensor

Returns
-------
TensorBatch
    New `TensorBatch` object with an underlying np.ndarray tensor.

---
### FunctionDef: `to_tensor`

Cast underlying tensor to a `torch.tensor` and return a new instance.

Parameters
----------
dtype : torch.dtype, optional
    Data type of the tensor to create
device : torch.device, optional
    Device on which to put the tensor

Returns
-------
TensorBatch
    New `TensorBatch` object with an underlying np.ndarray tensor.

---
### FunctionDef: `topology`

String representing the interaction topology.

Returns
-------
str
    String listing the number of primary particles in this interaction

---
### FunctionDef: `tpc_traces`

Function which produces a list of traces which represent the TPCs in
a 3D event display.

Parameters
----------
meta : Meta, optional
    Metadata information (only needed if pixel_coordinates is True)
draw_faces : bool, default False
    Weather or not to draw the box faces, or only the edges
shared_legend : bool, default True
    If True, the legend entry in plotly is shared between all the
    detector volumes
name : Union[str, List[str]], default 'Detector'
    Name(s) of the detector volumes
color : Union[int, str, np.ndarray]
    Color of boxes or list of color of boxes
linewidth : int, default 2
    Width of the box edge lines
**kwargs : dict, optional
    List of additional arguments to pass to
    spine.viusalization.boxes.box_traces

Returns
-------
List[Union[plotly.graph_objs.Scatter3D, plotly.graph_objs.Mesh3D]]
    List of detector traces (one per TPC)

---
### ClassDef: `TPCDetector`

Handles all geometry queries for a set of time-projection chambers.

Attributes
----------
modules : List[Module]
    (N_m) List of TPC modules associated with this detector
chambers : List[Chamber]
    (N_t) List of individual TPC associated with this detector
det_ids : np.ndarray, optional
    (N_c) Map between logical and physical TPC index

---
### ClassDef: `TrackCompletenessAna`

This analysis script identifies gaps in tracks and measures the
cumulative length of these gaps relative to the track length.

This is a useful diagnostic tool to evaluate the space-point efficiency
on tracks (good standard candal as track should have exactly no gap in
a perfectly efficient detector).

---
### ClassDef: `TrackExtremaProcessor`

Assigns track start point and end point.

---
### ClassDef: `TrackShowerMergerProcessor`

Merge tracks into showers based on a set of selection criteria.
    

---
### ClassDef: `TrackValidityProcessor`

Check if track is valid based on the proximity to reconstructed vertex.
Can also reject small tracks that are close to the vertex (optional).

---
### FunctionDef: `train_single`

Train a model in a single process.

Parameters
----------
rank : int
    Process rank
cfg : dict
    Full driver/trainer configuration
distributed : bool, default False
    If `True`, distribute the training process
world_size : int, optional
    Number of devices to use in the distributed training process

---
### ClassDef: `TrainDrawer`

Class which centralizes function used to monitor a training process.

---
### ClassDef: `TransformerEncoderLayer`

Transformer module (attention mechanism) that takes (N, F_in) feature
tensors to (N, F_out) feature tensor. 

---
### ClassDef: `TransformerSPICE`

Transformer based model for particle clustering, using Mask3D
as a backbone.

Mask3D backbone implementation: https://github.com/JonasSchult/Mask3D

Mask3D: https://arxiv.org/abs/2210.03105

---
### FunctionDef: `translate`

Moves a point cloud from one module to another one

Parameters
----------
points : np.ndarray
    (N, 3) Set of point coordinates
source_id: int
    Module ID from which to move the point cloud
target_id : int
    Module ID to which to move the point cloud
factor : Union[float, np.ndarray], optional
    Multiplicative factor to apply to the offset. This is necessary if
    the points are not expressed in detector coordinates

Returns
-------
np.ndarray
    (N, 3) Set of translated point coordinates

---
### ClassDef: `Translater`

Generic class to handle moving images around.

---
### ClassDef: `TransparencyCalibrator`

Applies a correction on the amount of charge observed in a space point
based on its position in the plane of the sensitive wires/pixels (yz).

---
### ClassDef: `Trigger`

Trigger information.

Attributes
----------
id : int
    Trigger ID
time_s : int
    Integer seconds component of the UNIX trigger time
time_ns : int
    Integer nanoseconds component of the UNIX trigger time
beam_time_s : int
    Integer seconds component of the UNIX beam pulse time
beam_time_ns : int
    Integer seconds component of the UNIX beam pulse time
type : int
    DAQ-specific trigger type

---
### ClassDef: `TriggerParser`

Copy construct Trigger and return a `Trigger`.

.. code-block. yaml
    schema:
      trigger:
        parser: trigger
        trigger_event: trigger_base

---
### ClassDef: `TriggerProcessor`

Parses trigger information from a CSV file and adds a new trigger_info
data product to the data dictionary.

---
### ClassDef: `TruthBase`

Base data structure shared among all truth output classes.

Attributes
----------
orig_id : int
    If matched to an MC truth instance, ID of the original instance
depositions_q : np.ndarray
    (N) Array of values for each voxel in the same units as the input image
depositions_q_sum : float
    Total amount of depositions in the same units as the input image
index_adapt: np.ndarray
    (N') Voxel indexes corresponding to this object in the adapted cluster
    label tensor
size_adapt : int
    Number of points, N', that make up this object in the adapted cluster
    label tensor
points_adapt : np.ndarray
    (N', 3) Set of voxel coordinates using adapted cluster labels
sources_adapt : np.ndarray
    (N', 2) Set of voxel sources as (Module ID, TPC ID) pairs, adapted
depositions_adapt : np.ndarray
    (N') Array of values for each voxel in the adapted cluster label tensor
depositions_adapt_sum : float
    Total amount of depositions in adapted cluster label tensor
depositions_adapt_q : np.ndarray
    (N) Array of values for each voxel in the same units as the input image
depositions_adapt_q_sum : float
    Total amount of depositions in adapted cluster label tensor in the same
    units as the input image
sources_adapt : np.ndarray
    (N, 2) Set of voxel sources as (Module ID, TPC ID) pairs, adapted
index_g4: np.ndarray
    (N'') Fragment voxel indexes in the true Geant4 energy deposition tensor
size_g4 : int
    Number of points, N'', that make up this object in the true Geant4
    energy deposition tensor
points_g4 : np.ndarray
    (N'', 3) Set of voxel coordinates of true Geant4 energy depositions
depositions_g4 : np.ndarray
    (N'') Array of true Geant4 energy depositions per voxel
depositions_g4_sum : float
    Total amount of true Geant4 depositions

---
### ClassDef: `TruthFragment`

Truth fragment information.

This inherits all of the attributes of :class:`Particle`, which contains
the G4 truth information for the fragment.

Attributes
----------
orig_interaction_id : int
    Unaltered index of the interaction in the original MC particle list
orig_parent_id : int
    Unaltered index of the particle parent in the original MC particle list
orig_group_id : int
    Unaltered index of the particle group in the original MC particle list
orig_children_id : np.ndarray
    Unaltered list of the particle children in the original MC particle list
children_counts : np.ndarray
    (P) Number of truth child fragment of each shape
reco_length : float
    Reconstructed length of the fragment (only assigned to track objects)
reco_start_dir : np.ndarray
    (3) Particle direction estimate w.r.t. the start point
reco_end_dir : np.ndarray
    (3) Particle direction estimate w.r.t. the end point (only assigned
    to track objects)

---
### ClassDef: `TruthInteraction`

Truth interaction information.

This inherits all of the attributes of :class:`Interaction`, which contains
the G4 truth information for the interaction.

Attributes
----------
nu_id : int
    Index of the neutrino matched to this interaction
reco_vertex : np.ndarray
    (3) Coordinates of the reconstructed interaction vertex

---
### ClassDef: `TruthParticle`

Truth particle information.

This inherits all of the attributes of :class:`Particle`, which contains
the G4 truth information for the particle.

Attributes
----------
orig_interaction_id : int
    Unaltered index of the interaction in the original MC particle list
orig_parent_id : int
    Unaltered index of the particle parent in the original MC particle list
orig_group_id : int
    Unaltered index of the particle group in the original MC particle list
orig_children_id : np.ndarray
    Unaltered list of the particle children in the original MC particle list
children_counts : np.ndarray
    (P) Number of truth child particle of each shape
reco_length : float
    Reconstructed length of the particle (only assigned to track objects)
reco_start_dir : np.ndarray
    (3) Particle direction estimate w.r.t. the start point
reco_end_dir : np.ndarray
    (3) Particle direction estimate w.r.t. the end point (only assigned
    to track objects)
reco_ke : float
    Best-guess reconstructed KE of the particle
reco_momentum : np.ndarray
    Best-guess reconstructed momentum of the particle

---
### FunctionDef: `umbrella_curv`

Computes the umbrella curvature as in equation 9 of "Umbrella Curvature:
A New Curvature Estimation Method for Point Clouds" by A.Foorginejad and
K.Khalili
(https://www.sciencedirect.com/science/article/pii/S2212017313006828)

Parameters
----------
voxels : np.ndarray
    (N, 3) Voxel coordinates
vox_id : int
    Index of the voxel w.r.t. which to compute the curvature

Returns
-------
float
    Value of the umbrella curvature at `vox_id`

---
### ClassDef: `UncertaintyFormatter`

Use a new-style format string (as used by `str.format`) to format the tick.

The field used for the tick value must be labeled *x* and the field used
for the tick position must be labeled *pos*.

---
### FunctionDef: `union_find`

Implementation of the Union-Find algorithm.

This algorithm forms group based on the connectivity of its consistuents.
If two entities are connected, they belong to the same group.

Parameters
----------
edge_index : np.ndarray
    (E, 2) Sparse incidence matrix
num_nodes : int
    Number of nodes in the graph, C

Returns
-------
np.ndarray
    (C) Node group IDs
Dict[int, np.ndarray]
    Dictionary which maps group IDs onto constituent cluster IDs

---
### FunctionDef: `union_find`

Numba implementation of the Union-Find algorithm.

This function assigns a group to each node in a graph, provided
a set of edges connecting the nodes together.

Parameters
----------
edge_index : np.ndarray
    (E, 2) List of edges (sparse adjacency matrix)
count : int
    Number of nodes in the graph, C
return_inverse : bool, default True
    Make sure the group IDs range from 0 to N_groups-1

Returns
-------
np.ndarray
    (C) Group assignments for each of the nodes in the graph

---
### FunctionDef: `unique`

Numba implementation of `np.unique(x, return_counts=True)`.

Parameters
----------
x : np.ndarray
    (N) array of values

Returns
-------
np.ndarray
    (U) array of unique values
np.ndarray
    (U) array of counts of each unique value in the original array

---
### FunctionDef: `unique_index`

Returns the list of unique indexes in the tensor and their first index.

This is a temporary implementation until PyTorch adds support for the
`return_index` argument in their `torch.unique` function.

Parameters
----------
x : torch.Tensor
    (N) Tensor of values

Returns
-------
unique : torch.Tensor
    (U) List of unique values in the input tensor
index : torch.Tensor
    (U) List of the first index of each unique values

---
### FunctionDef: `unique_labels`

Transforms labels to range from 0 to C-1 labels (with C the number of
unique values in the label array.

If batch IDs are provided, ensures that the labels are unique at the batch
level as well.

Parameters
----------
labels : np.ndarray
    (N) Labels
batch_ids : np.ndarray, optional
    (N) Batch IDs

Returns
-------
inverse : np.ndarray
    (N) Unique labels across all entries in the batch
unique : np.ndarray
    (C) Unique set of labels
counts : np.ndarray
    (C) Number of labels which belong to each unique category

---
### ClassDef: `Unwrapper`

Unwraps batched data to its constituent entries.

Class used to break down the batched input and output dictionaries into
individual events. When passed through the model, the input is concatenated
into single tensors/arrays for faster processing; this class breaks the
output down event-wise to be human-readable.

---
### FunctionDef: `update`

Updates this manager with values from another stopwatch manager.

Parameters
----------
other : StopwatchManager
     Dictionary of execution times from another process
prefix : str, optional
     String to prefix the timer key with

Returns
-------
Dict[str, Time]
    Combined execution time of all iterations of each process so far

---
### FunctionDef: `update_counts`

Updates the number of elements per entry in the batch, provided
a mask which restricts the number of valid elements in the batch.

Parameters
----------
counts : np.ndarray
    (B) : Number of elements in each entry of the batch
mask : np.ndarray
    Mask to apply to the list of elements

Returns
-------
np.ndarray
    (B) Updated number of elements in each entry of the batch

---
### FunctionDef: `update_keys`

Update the underlying set of keys and their necessity in place.

Parameters
----------
update_dict : Dict[str, bool]
    Dictionary of (key, necessity) pairs to update the keys with

---
### FunctionDef: `update_keys`

Update the underlying set of keys and their necessity in place.

Parameters
----------
update_dict : Dict[str, bool]
    Dictionary of (key, necessity) pairs to update the keys with

---
### FunctionDef: `update_progress`

Pure Python Progress Bar
Author: Brian Khuu, rayryeng
Reference: https://stackoverflow.com/questions/3160699/python-progress-bar

---
### FunctionDef: `update_result`

Update loss and accuracy using the output of one of the module.

Parameters
----------
result : dict
    Dictionary output of the module
prefix : str, optional
    Prefix to preface the loss output keys with

---
### FunctionDef: `upper`

Upper bounds of the box.

Returns
-------
np.ndarray
    Upper bounds of the box

---
### ClassDef: `UResNet`

Vanilla UResNet with access to intermediate feature planes.

See :func:`setup_cnn_configuration` for available parameters.

---
### ClassDef: `UResNetDecoder`

Vanilla UResNet Decoder.

See :func:`setup_cnn_configuration` for available parameters.

---
### ClassDef: `UResNetEncoder`

Vanilla UResNet encoder.

See :func:`setup_cnn_configuration` for available parameters.

---
### ClassDef: `UResNetPPN`

A model made of a UResNet backbone and PPN layers.

Typical configuration:

.. code-block:: yaml

    model:
      name: uresnet_ppn_chain
      modules:
        uresnet:
          # Your backbone uresnet config here
        ppn:
          # Your ppn config here

See Also
--------
:class:`UResNetSegmentation`, :class:`PPN`

---
### ClassDef: `UResNetPPNLoss`

Loss for amodel made of a UResNet backbone and PPN layers.

It includes a segmentation loss and a PPN loss.

Typical configuration:

.. code-block:: yaml

    model:
      name: uresnet_ppn_chain
      modules:
        uresnet:
          # Your backbone uresnet config goes here
        ppn:
          # Your ppn config goes here
        ppn_loss:
          # Your ppn loss config goes here

See Also
--------
:class:`spine.model.uresnet.SegmentationLoss`,
:class:`spine.model.layer.cnn.ppn.PPNLoss`

---
### ClassDef: `UResNetSegmentation`

UResNet for semantic segmentation.

Typical configuration should look like:

.. code-block:: yaml

    model:
      name: uresnet
      modules:
        uresnet:
          # Your config goes here

See :func:`setup_cnn_configuration` for available parameters for the
backbone UResNet architecture.

See configuration file(s) prefixed with `uresnet_` under the `config`
directory for detailed examples of working configurations.

---
### ClassDef: `UResNetVertexLoss`

See Also
--------
spine.model.uresnet.SegmentationLoss, spine.model.layer.common.ppn.PPNLonelyLoss

---
### ClassDef: `UResNeXt`

UNet Type encoder-decoder network, with atrous convolutions and
resnext-type blocks.

---
### FunctionDef: `values`

Get the list of all initialized stopwatches.

Returns
-------
List[Stopwatch]
    List of stopwatch objects

---
### FunctionDef: `var_length_attrs`

Fetches the list of variable-length array attributes as a dictionary.

Returns
-------
Dict[str, type]
    Dictionary which maps variable-length attributes onto their type

---
### ClassDef: `VertexPointParser`

Class that retrieves the vertices.

It provides the coordinates of points where multiple particles originate:
- If the `neutrino_event` is provided, it simply uses the coordinates of
  the neutrino interaction points.
- If the `particle_event` is provided instead, it looks for ancestor point
  positions shared by at least two particles.

.. code-block. yaml

    schema:
      vertices:
        parser: vertex_points
        particle_event: particle_pcluster
        #neutrino_event: neutrino_mpv
        sparse_event: sparse3d_pcluster
        include_point_tagging: True

---
### ClassDef: `VertexPPNChain`

Experimental model for PPN-like vertex prediction

---
### ClassDef: `VertexPPNLoss`

Loss function for PPN.

Output
------
vertex_reg_loss : float
    Distance loss
vertex_mask_loss : float
    Binary voxel-wise prediction (is there an object of interest or not)
vertex_loss : float
    Combined loss
vertex_accuracy : float
    Combined accuracy

See Also
--------
PPN, spine.model.uresnet_ppn_chain

---
### ClassDef: `VertexProcessor`

Reconstruct one vertex for each interaction in the provided list.

---
### FunctionDef: `visualize_subgraph`

Visualizes the subgraph given an edge mask
:attr:`edge_mask`.
Args:
    node_idx (int): The node id to explain.
        Set to :obj:`-1` to explain graph.
    edge_index (LongTensor): The edge indices.
    edge_mask (Tensor): The edge mask.
    y (Tensor, optional): The ground-truth node-prediction labels used
        as node colorings. All nodes will have the same color
        if :attr:`node_idx` is :obj:`-1`.(default: :obj:`None`).
    threshold (float, optional): Sets a threshold for visualizing
        important edges. If set to :obj:`None`, will visualize all
        edges with transparancy indicating the importance of edges.
        (default: :obj:`None`)
    edge_y (Tensor, optional): The edge labels used as edge colorings.
    node_alpha (Tensor, optional): Tensor of floats (0 - 1) indicating
        transparency of each node.
    seed (int, optional): Random seed of the :obj:`networkx` node
        placement algorithm. (default: :obj:`10`)
    **kwargs (optional): Additional arguments passed to
        :func:`nx.draw`.
:rtype: :class:`matplotlib.axes.Axes`, :class:`networkx.DiGraph`

---
### FunctionDef: `volume_index`

Returns an index which corresponds to detectors in a certain volume.

Parameters
----------
volume_id : int
    ID of the volume to return the index for

Returns
-------
np.ndarray
    Index of the detectors which belong to the requested volume ID

---
### FunctionDef: `voxel_efficiency_bipartite`

Computes the fraction of secondary voxels that are associated to the
correct primary.

Parameters
----------
clusts : List[np.ndarray]
    (C) List of cluster indexes
node_assn : np.ndarray
    (C) True node groups labels
node_pred : np.ndarray
    (C) Predicted node group labels
node_pred : np.ndarray
    (P) List of primary IDs

Returns
-------
float
    Fraction of correctly assigned secondary voxels

---
### FunctionDef: `W_max`

Maximum energy transfer in a single colision.

Parameters
----------
beta : float
    Lorentz beta (v/c)
gamma : float
    Lorentz gamma (1/sqrt(1-beta**2))
M : float
    Mass of the impinging particle in MeV/c^2

Returns
-------
float
    Maximum energy transferred in a single colision

---
### FunctionDef: `weight`

Weight parameter of the AdaIN layer.

Note that in AdaptIS, the parameters to the AdaIN layer
are trainable outputs from the controller network.

---
### FunctionDef: `writer_factory`

Instantiates writer based on type specified in configuration under
`io.writer.name`. The name must match the name of a class under
`spine.io.writers`.

Parameters
----------
writer_cfg : dict
    Writer configuration dictionary
prefix : str, optional
    Input file prefix to use as an output name
split : bool, default False
    Split the output into one file per input file

Returns
-------
object
    Writer object

Note
----
Currently the choice is limited to `HDF5Writer` only.

---
### FunctionDef: `xloss`

Cross entropy loss

---
