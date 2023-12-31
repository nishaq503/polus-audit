# Status of Polus Plugins

This is a summary of the plugins on the master branch.
The following table shows a quick overview, while subsequent sections provide more details.

## Summary Table

The columns are as follows:

* `Family`: The group of plugins that the plugin belongs to. This refers to the (potentially nested) folder that the plugin is in.
* `Plugin`: The name of the plugin.
  * I have stripped the `polus-` prefix from the plugin name.
  * Some plugins did not have the `-plugin` postfix.
* `Version`: The version of the plugin.
  * If there is an open PR for the plugin, this number will reflect the version in the PR.
* `Language`: The language(s) that the plugin is written in.
* `Status`: The status of the plugin.
  * `Updated`: The plugin has been updated to the new standard for python plugins.
  * `Peer Review`: The plugin has been updated to the new standard for python plugins and is currently in peer review.
  * `Old`: The plugin has not been updated to the new standard for python plugins.
  * `Unknown`: The plugin is not a python plugin.
* `PR`: The PR number for the plugin.
  * If there is no PR, this will be `None`.
* `bfio`: The version of bfio that the plugin uses.
  * If the plugin does not use bfio, this will be `None`.
  * 1.x refers to an undetermined version of bfio before the 2.0 release.
  * 2.x refers to an undetermined version of bfio before the 2.1.9 release.
* `filepattern`: The version of filepattern that the plugin uses.
  * If the plugin does not use filepattern, this will be `None`.
  * 1.x refers to an undetermined version of filepattern before the 2.0.0 release.
  * test-2.2.7 refers to the version of filepattern on test-pypi.
* `preadator`: The version of preadator that the plugin uses.
  * If the plugin does not use preadator, this will be `None`.
* `nyxus`: The version of nyxus that the plugin uses.
  * If the plugin does not use nyxus, this will be `None`.

### Clustering

| Family | Plugin | Version | Language | Status | PR | bfio | filepattern | preadator | nyxus |
| ------ | ------ | ------- | -------- | ------ | -- | ---- | ----------- | --------- | ----- |
| clustering | k-means-clustering-plugin | 0.3.2-dev | Python | Updated | None | None | 2.0.0 | None | 0.5.0 |
| clustering/K-NN | Distributed-Memory | None | C++ | Unknown | None | None | None | None | None |
| clustering/K-NN | Shared-Memory-GPU | 0.1.0 | Cuda | Unknown | None | None | None | None | None |
| clustering/K-NN | Shared-Memory-OpenMP | 0.1.0 | C++ | Unknown | None | None | None | None | None |
| clustering/K-NN | Shared-Memory-Serial | 0.1.0 | C++ | Unknown | None | None | None | None | None |
| clustering | feature-subsetting-plugin | 0.1.11 | Python | Old | None | None | 1.4.5 | None | None |
| clustering | hdbscan-clustering-plugin | 0.4.7 | Python | Old | None | None | None | None | None |
| clustering | outlier-removal-plugin | 0.2.5 | Python | Old | None | None | None | None | None |

### Dimension Reduction

| Family | Plugin | Version | Language | Status | PR | bfio | filepattern | preadator | nyxus |
| ------ | ------ | ------- | -------- | ------ | -- | ---- | ----------- | --------- | ----- |
| dimension_reduction/PCA | Distributed-Memory | Unknown | Python | Old | None | None | None | None | None |
| dimension_reduction/PCA | Shared-Memory | 0.1.3 | Python | Old | None | None | None | None | None |
| dimension_reduction/UMAP | Shared-Memory-GPU | 0.1.0 | C++/Cuda | Unknown | None | None | None | None | None |
| dimension_reduction/UMAP | Shared-Memory-OpenMP | 0.1.6 | C++ | Unknown | None | None | None | None | None |

### Features

| Family | Plugin | Version | Language | Status | PR | bfio | filepattern | preadator | nyxus |
| ------ | ------ | ------- | -------- | ------ | -- | ---- | ----------- | --------- | ----- |
| features | feature-segmentation-eval | 0.2.3 | Python | Updated | None | None | 2.0.1 | None | None |
| features | nyxus-plugin | 0.1.3 | Python | Old | None | None | 1.4.7 | 0.2.0 | 0.4.0 |
| features | pixel-segmentation-eval | 0.1.10 | Python | Updated | None | 2.1.9 | 2.0.1 | None | None |
| features | csv-statistics-plugin | 0.2.1 | Python | Old | None | None | 1.4.7 | None | None |
| features | feature-extraction-plugin | 0.12.2 | Python | Old | None | Unknown | 1.4.4 | None | None |
| features | imagenet-model-featurization-plugin | 0.1.3 | Python | Old | None | 2.1.9 | None | None | None |
| features | object-spectral-featurization-plugin | 0.1.2 | Python | Old | None | 2.1.9 | None | None | None |
| features | region-segmentation-eval | 0.2.3 | Python | Updated | None | 2.1.9 | 2.0.1 | None | None |

### Formats

| Family | Plugin | Version | Language | Status | PR | bfio | filepattern | preadator | nyxus |
| ------ | ------ | ------- | -------- | ------ | -- | ---- | ----------- | --------- | ----- |
| formats | file-renaming-plugin | 0.2.0 | Python | Updated | None | None | None | None | None |
| formats | label-to-vector-plugin | 0.7.0-dev30 | Python | Peer Review | [#450](https://github.com/PolusAI/polus-plugins/pull/450) | 2.1.9 | 2.0.1 | None | None |
| formats | ome-converter-plugin | 0.3.0 | Python | Peer Review | [#486](https://github.com/PolusAI/polus-plugins/pull/486) | 2.1.9 | test-2.2.7 | None | None |
| formats | czi-extract-plugin | 1.1.1 | Python | Old | None | 2.x | None | 0.2.0 | None |
| formats | fcs-to-csv-converter-plugin | 0.2.5 | Python | Old | None | None | None | None | None |
| formats | feather-to-tabular-plugin | 0.1.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| formats | imaris-parser-plugin | 0.3.3 | Python | Old | None | None | None | None | None |
| formats | multichannel-tiff-plugin | 0.2.3 | Python | Old | None | 1.x | 1.2.4 | None | None |
| formats | tabular-to-feather-plugin | 0.1.4 | Python | Old | None | None | 1.4.7 | None | None |
| formats | tiledtiff-converter-plugin | 1.1.2 | Java | Unknown | None | None | None | None | None |
| formats | vector-to-label-plugin | 0.7.0-dev34 | Python | Peer Review | [#450](https://github.com/PolusAI/polus-plugins/pull/450) | 2.1.9 | 2.0.1 | None | None |

### Regression

| Family | Plugin | Version | Language | Status | PR | bfio | filepattern | preadator | nyxus |
| ------ | ------ | ------- | -------- | ------ | -- | ---- | ----------- | --------- | ----- |
| regression | basic-flatfield-estimation-plugin | 2.0.0 | Python | Updated | None | 2.1.9 | 2.0.0 | None | None |
| regression | theia-bleedthrough-estimation-plugin | 0.5.0-dev0 | Python | Peer Review | [#451](https://github.com/PolusAI/polus-plugins/pull/451) | 2.3.1-dev0 | 2.0.1 | None | None |

### Segmentation

| Family | Plugin | Version | Language | Status | PR | bfio | filepattern | preadator | nyxus |
| ------ | ------ | ------- | -------- | ------ | -- | ---- | ----------- | --------- | ----- |
| segmentation | aics-classic-seg-plugin | 0.1.11 | Python | Old | None | None | None | None | None |
| segmentation | cell-nuclei-segmentation | 0.1.4 | Python | Old | None | None | None | None | None |
| segmentation | imagej-threshold-apply-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-huang-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-ij1-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-intermodes-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-isodata-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-li-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-maxentropy-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-maxlikelyhood-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-mean-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-minerror-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-minimum-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-moments-plugin | 0.4.2 | Python | Old | None | Unknown | 1.4.4 | None | None |
| segmentation | imagej-threshold-otsu-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-percentile-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | imagej-threshold-renyientropy-plugin | 0.4.2 | Python | Old | None | Unknown | 1.4.4 | None | None |
| segmentation | imagej-threshold-rosin-plugin | 0.4.2 | Python | Old | None | Unknown | 1.4.4 | None | None |
| segmentation | imagej-threshold-shanbhag-plugin | 0.4.2 | Python | Old | None | Unknown | 1.4.4 | None | None |
| segmentation | imagej-threshold-triangle-plugin | 0.4.2 | Python | Old | None | Unknown | 1.4.4 | None | None |
| segmentation | imagej-threshold-yen-plugin | 0.4.2 | Python | Old | None | Unknown | 1.4.4 | None | None |
| segmentation | smp-training-plugin | 0.5.11 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| segmentation | z01-segmentation-plugin | 0.2.0 | Python | Old | None | 2.x | None | None | None |

### Transforms

| Family | Plugin | Version | Language | Status | PR | bfio | filepattern | preadator | nyxus |
| ------ | ------ | ------- | -------- | ------ | -- | ---- | ----------- | --------- | ----- |
| transforms | recycle-vector-plugin | 1.5.0 | Python | Old | None | None | 1.4.7 | None | None |
| transforms/images | apply-flatfield-plugin | 2.0.0-dev8 | Python | Peer Review | [#443](https://github.com/PolusAI/polus-plugins/pull/443) | 2.1.9 | 2.0.0 | None | None |
| transforms/images | image-assembler-plugin | 1.4.0-dev0 | Python | Peer Review | [#479](https://github.com/PolusAI/polus-plugins/pull/479), [#481](https://github.com/PolusAI/polus-plugins/pull/481) | 2.1.9 | 2.0.4 | 0.4.0.dev2 | None |
| transforms/images | image-calculator-plugin | 0.2.0 | Python | Updated | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | lumos-bleedthrough-correction-plugin | 0.1.0 | Python | Updated | None | 2.1.9 | 2.0.0 | None | None |
| transforms/images | montage-plugin | 0.5.0 | Python | Updated | None | 2.1.9 | 2.0.0 | None | None |
| transforms/images | autocropping-plugin | 1.0.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | binary-operations-plugin | 0.4.2 | Python | Old | None | 1.x | 1.4.7 | None | None |
| transforms/images | ftl-label-plugin | 0.3.10 | Python/CPython/Rust | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | image-registration-plugin | 0.3.5 | Python | Old | None | 1.x | 1.2.4 | None | None |
| transforms/images | imagej-deconvolve-richardsonlucy-plugin | 0.4.3 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-deconvolve-richardsonlucytv-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-filter-addpoissonnoise-plugin | 0.4.4 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-filter-convolve-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-filter-correlate-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-filter-derivativegauss-plugin | 0.4.4 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-filter-dog-plugin | 0.3.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-filter-frangivesselness-plugin | 0.4.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-filter-gauss-plugin | 0.3.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-filter-partialderivative-plugin | 0.3.5 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-filter-sobel-plugin | 0.3.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-filter-tubeness-plugin | 0.3.8 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-image-integral-plugin | 0.3.2 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | imagej-image-invert-plugin | 0.4.0 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| transforms/images | intensity-projection-plugin | 1.0.0 | Python | Old | None | 2.0.5 | None | 0.2.0 | None |
| transforms/images | rolling-ball-plugin | 1.1.0-dev0 | Python | Peer Review | [#429](https://github.com/PolusAI/polus-plugins/pull/429) | 2.1.9 | None | None | None |
| transforms/images | stack-z-slice-plugin | 1.2.4 | Python | Old | None | 2.x | 1.4.7 | 0.2.0 | None |
| transforms/images | roi-relabel-plugin | 0.2.2 | Python | Updated | None | 2.1.9 | 2.0.0 | None | None |
| transforms/tabular | csv-merger-plugin | 0.4.0 | Python | Old | None | None | 1.4.7 | None | None |
| transforms/tabular | generalized-linear-model-plugin | 0.2.5 | R | Unknown | None | None | None | None | None |
| transforms/tabular | tabular-thresholding-plugin | 0.1.3 | Python | Updated | None | None | test-2.2.7 | None | None |

### Utils

| Family | Plugin | Version | Language | Status | PR | bfio | filepattern | preadator | nyxus |
| ------ | ------ | ------- | -------- | ------ | -- | ---- | ----------- | --------- | ----- |
| utils | filepattern-generator-plugin | 0.2.1 | Python | Old | None | None | 1.4.7 | None | None |
| utils | csv-collection-merger | 0.1.1 | sh | Old | None | None | None | None | None |
| utils | generic-to-image-collection-plugin | 0.1.1 | Python | Old | None | 2.x | 1.4.7 | None | None |
| utils | imagej-macro-plugin | 0.1.3 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| utils | notebook-plugin | 0.4.0 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| utils | stitching-vector-merger-plugin | 0.1.8 | Python | Old | None | None | None | None | None |
| utils | subset-data-plugin | 0.1.8 | Python | Old | None | None | 1.4.7 | None | None |

### Visualization

| Family | Plugin | Version | Language | Status | PR | bfio | filepattern | preadator | nyxus |
| ------ | ------ | ------- | -------- | ------ | -- | ---- | ----------- | --------- | ----- |
| visualization | color-pyramid-builder-plugin | 0.3.3 | Python | Updated | None | 1.x | 1.2.4 | None | None |
| visualization | feature-heatmap-pyramid-plugin | 0.2.0 | Python | Updated | None | 1.x | 1.2.4 | None | None |
| visualization | graph-pyramid-builder-plugin | 1.3.8 | Python | Updated | None | 1.x | 1.2.4 | None | None |
| visualization | image-cluster-annotation-plugin | 0.2.4 | Python | Updated | None | 2.x | 1.2.4 | None | None |
| visualization | precompute-slide-plugin | 1.7.0-dev0 | Python | Peer Review | [#484](https://github.com/PolusAI/polus-plugins/pull/484) | 2.1.9 | 2.0.4 | 0.4.0-dev2 | None |
| visualization | precompute-volume-plugin | 1.7.0-dev0 | Python | Old | None | 2.1.9 | 1.4.7 | None | None |
| visualization | tabular-to-microjson-plugin | 0.1.0 | Python | Updated | None | None | 2.0.1 | None | None |

## Details

### Clustering

<details>
<summary>k-means-clsutering-plugin</summary>

* Version: 0.3.2-dev
* Language: Python
* Status: Updated
* bfio: None
* filepattern: 2.0.0
* preadator: None
* nyxus: 0.5.0

</details>  <!-- end k-means-clustering-plugin -->

<details>
<summary>K-NN</summary>

<details>
<summary>Distributed-Memory</summary>

* Version: None
* Language: C++
* Status: Unknown
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end Distributed-Memory -->

<details>
<summary>Shared-Memory-GPU</summary>

* Version: 0.1.0
* Language: Cuda
* Status: Unknown
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end Shared-Memory-GPU -->

<details>
<summary>Shared-Memory-OpenMP</summary>

* Version: 0.1.0
* Language: C++
* Status: Unknown
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end Shared-Memory-OpenMP -->

<details>
<summary>Shared-Memory-Serial</summary>

* Version: 0.1.0
* Language: C++
* Status: Unknown
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end Shared-Memory-Serial -->

</details>  <!-- end K-NN -->

<details>
<summary>feature-subsetting-plugin</summary>

* Version: 0.1.11
* Language: Python
* Status: Old
* bfio: None
* filepattern: 1.4.5
* preadator: None
* nyxus: None

</details>  <!-- end feature-subsetting-plugin -->

<details>
<summary>hdbscan-clustering-plugin</summary>

* Version: 0.4.7
* Language: Python
* Status: Old
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end hdbscan-clustering-plugin -->

<details>
<summary>outlier-removal-plugin</summary>

* Version: 0.2.5
* Language: Python
* Status: Old
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>   <!-- end outlier-removal-plugin -->

### Dimension Reduction

<details>
<summary>PCA</summary>

<details>
<summary>Distributed-Memory</summary>

* Version: Unknown
* Language: Python
* Status: Old
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end Distributed-Memory -->

<details>
<summary>Shared-Memory</summary>

* Version: 0.1.3
* Language: Python
* Status: Old
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end Shared-Memory -->

</details>  <!-- end PCA -->

<details>
<summary>UMAP</summary>

<details>
<summary>Shared-Memory-GPU</summary>

* Version: 0.1.0
* Language: C++/Cuda
* Status: Unknown
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end Shared-Memory-GPU -->

<details>
<summary>Shared-Memory-OpenMP</summary>

* Version: 0.1.6
* Language: C++
* Status: Unknown
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end Shared-Memory-OpenMP -->

</details>  <!-- end UMAP -->

### Features

<details>
<summary>feature-segmentation-eval</summary>

* Version: 0.2.3
* Language: Python
* Status: Updated
* bfio: None
* filepattern: 2.0.1
* preadator: None
* nyxus: None

</details>  <!-- end feature-segmentation-eval -->

<details>
<summary>nyxus-plugin</summary>

* Version: 0.1.3
* Language: Python
* Status: Old
* bfio: None
* filepattern: 1.4.7
* preadator: 0.2.0
* nyxus: 0.4.0

</details>  <!-- end nyxus-plugin -->

<details>
<summary>pixel-segmentation-eval</summary>

* Version: 0.1.10
* Language: Python
* Status: Updated
* bfio: 2.1.9
* filepattern: 2.0.1
* preadator: None
* nyxus: None

</details>  <!-- end pixel-segmentation-eval -->

<details>
<summary>csv-statistics-plugin</summary>

* Version: 0.2.1
* Language: Python
* Status: Old
* bfio: None
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end csv-statistics-plugin -->

<details>
<summary>feature-extraction-plugin</summary>

* Version: 0.12.2
* Language: Python
* Status: Old
* bfio: Unknown
* filepattern: 1.4.4
* preadator: None
* nyxus: None

</details>  <!-- end feature-extraction-plugin -->

<details>
<summary>imagenet-model-featurization-plugin</summary>

* Version: 0.1.3
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end imagenet-model-featurization-plugin -->

<details>
<summary>object-spectral-featurization-plugin</summary>

* Version: 0.1.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end object-spectral-featurization-plugin -->

<details>
<summary>region-segmentation-eval</summary>

* Version: 0.2.3
* Language: Python
* Status: Updated
* bfio: 2.1.9
* filepattern: 2.0.1
* preadator: None
* nyxus: None

</details>  <!-- end region-segmentation-eval -->

### Formats

<details>
<summary>file-renaming-plugin</summary>

* Version: 0.2.0
* Language: Python
* Status: Updated
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end file-renaming-plugin -->

<details>
<summary>label-to-vector-plugin</summary>

* Version: 0.7.0-dev30
* Language: Python
* Status: Peer Review
* PR: [#450](https://github.com/PolusAI/polus-plugins/pull/450)
* bfio: 2.1.9
* filepattern: 2.0.1
* preadator: None
* nyxus: None

</details>  <!-- end label-to-vector-plugin -->

<details>
<summary>ome-converter-plugin</summary>

* Version: 0.3.0
* Language: Python
* Status: Peer Review
* PR: [#486](https://github.com/PolusAI/polus-plugins/pull/486)
* bfio: 2.1.9
* filepattern: test-2.2.7
* preadator: None
* nyxus: None

</details>  <!-- end ome-converter-plugin -->

<details>
<summary>czi-extract-plugin</summary>

* Version: 1.1.1
* Language: Python
* Status: Old
* bfio: 2.x
* filepattern: None
* preadator: 0.2.0
* nyxus: None

</details>  <!-- end czi-extract-plugin -->

<details>
<summary>fcs-to-csv-converter-plugin</summary>

* Version: 0.2.5
* Language: Python
* Status: Old
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end fcs-to-csv-converter-plugin -->

<details>
<summary>feather-to-tabular-plugin</summary>

* Version: 0.1.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end feather-to-tabular-plugin -->

<details>
<summary>imaris-parser-plugin</summary>

* Version: 0.3.3
* Language: Python
* Status: Old
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>   <!-- end imaris-parser-plugin -->

<details>
<summary>multichannel-tiff-plugin</summary>

* Version: 0.2.3
* Language: Python
* Status: Old
* bfio: 1.x
* filepattern: 1.2.4
* preadator: None
* nyxus: None

</details>  <!-- end multichannel-tiff-plugin -->

<details>
<summary>tabular-to-feather-plugin</summary>

* Version: 0.1.4
* Language: Python
* Status: Old
* bfio: None
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end tabular-to-feather-plugin -->

<details>
<summary>tiledtiff-converter-plugin</summary>

* Version: 1.1.2
* Language: Java
* Status: Unknown
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end tiledtiff-converter-plugin -->

<details>
<summary>vector-to-label-plugin</summary>

* Version: 0.7.0-dev34
* Language: Python
* Status: Peer Review
* PR: [#450](https://github.com/PolusAI/polus-plugins/pull/450)
* bfio: 2.1.9
* filepattern: 2.0.1
* preadator: None
* nyxus: None

</details>  <!-- end vector-to-label-plugin -->

### Regression

<details>
<summary>basic-flatfield-estimation-plugin</summary>

* Version: 2.0.0
* Language: Python
* Status: Updated
* bfio: 2.1.9
* filepattern: 2.0.0
* preadator: None
* nyxus: None

</details>  <!-- end basic-flatfield-estimation-plugin -->

<details>
<summary>theia-bleedthrough-estimation-plugin</summary>

* Version: 0.5.0-dev0
* Language: Python
* Status: Peer Review
* PR: [#451](https://github.com/PolusAI/polus-plugins/pull/451)
* bfio: 2.3.1-dev0
* filepattern: 2.0.1
* preadator: None
* nyxus: None

</details>  <!-- end theia-bleedthrough-estimation-plugin -->

### Segmentation

<details>
<summary>aics-classic-seg-plugin</summary>

* Version: 0.1.11
* Language: Python
* Status: Old
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end aics-classic-seg-plugin -->

<details>
<summary>cell-nuclei-segmentation</summary>

* Version: 0.1.4
* Language: Python
* Status: Old
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end cell-nuclei-segmentation -->

<details>
<summary>imagej-threshold-apply-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-apply-plugin -->

<details>
<summary>imagej-threshold-huang-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-huang-plugin -->

<details>
<summary>imagej-threshold-ij1-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None  <!-- end imagej-threshold-ij1-plugin -->

</details>

<details>
<summary>imagej-threshold-intermodes-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-intermodes-plugin -->

<details>
<summary>imagej-threshold-isodata-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-isodata-plugin -->

<details>
<summary>imagej-threshold-li-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-li-plugin -->

<details>
<summary>imagej-threshold-maxentropy-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-maxentropy-plugin -->

<details>
<summary>imagej-threshold-maxlikelyhood-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-maxlikelyhood-plugin -->

<details>
<summary>imagej-threshold-mean-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-mean-plugin -->

<details>
<summary>imagej-threshold-minerror-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-minerror-plugin -->

<details>
<summary>imagej-threshold-minimum-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-minimum-plugin -->

<details>
<summary>imagej-threshold-moments-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-moments-plugin -->

<details>
<summary>imagej-threshold-otsu-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-otsu-plugin -->

<details>
<summary>imagej-threshold-percentile-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-percentile-plugin -->

<details>
<summary>imagej-threshold-renyientropy-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-renyientropy-plugin -->

<details>
<summary>imagej-threshold-rosin-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-rosin-plugin -->

<details>
<summary>imagej-threshold-shanbhag-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-shanbhag-plugin -->

<details>
<summary>imagej-threshold-triangle-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-triangle-plugin -->

<details>
<summary>imagej-threshold-yen-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-threshold-yen-plugin -->

<details>
<summary>smp-training-plugin</summary>

* Version: 0.5.11
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end smp-training-plugin -->

<details>
<summary>z01-segmentation-plugin</summary>

* Version: 0.2.0
* Language: Python
* Status: Old
* bfio: 2.x
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end z01-segmentation-plugin -->

### Transforms

<details>
<summary>recycle-vector-plugin</summary>

* Version: 1.5.0
* Language: Python
* Status: Old
* bfio: None
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end recycle-vector-plugin -->

#### Images

<details>
<summary>apply-flatfield-plugin</summary>

* Version: 2.0.0-dev8
* Language: Python
* Status: Peer Review
* PR: [#443](https://github.com/PolusAI/polus-plugins/pull/443)
* bfio: 2.1.9
* filepattern: 2.0.0
* preadator: None
* nyxus: None

</details>  <!-- end apply-flatfield-plugin -->

<details>
<summary>image-assembler-plugin</summary>

* Version: 1.4.0-dev0
* Language: Python
* Status: Peer Review
* PR: [#479](https://github.com/PolusAI/polus-plugins/pull/479), [#481](https://github.com/PolusAI/polus-plugins/pull/481)
* bfio: 2.1.9
* filepattern: 2.0.4
* preadator: 0.4.0.dev2
* nyxus: None

</details>  <!-- end apply-flatfield-plugin -->

<details>
<summary>image-calculator-plugin</summary>

* Version: 0.2.0
* Language: Python
* Status: Updated
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end image-calculator-plugin -->

<details>
<summary>lumos-bleedthrough-correction-plugin</summary>

* Version: 0.1.0
* Language: Python
* Status: Updated
* bfio: 2.1.9
* filepattern: 2.0.0
* preadator: None
* nyxus: None

</details>  <!-- end lumos-bleedthrough-correction-plugin -->

<details>
<summary>montage-plugin</summary>

* Version: 0.5.0
* Language: Python
* Status: Updated
* bfio: 2.1.9
* filepattern: 2.0.0
* preadator: None
* nyxus: None

</details>  <!-- end montage-plugin -->

<details>
<summary>autocropping-plugin</summary>

* Version: 1.0.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end autocropping-plugin -->

<details>
<summary>binary-operations-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 1.x
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end binary-operations-plugin -->

<details>
<summary>ftl-label-plugin</summary>

* Version: 0.3.10
* Language: Python/CPython/Rust
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end ftl-label-plugin -->

<details>
<summary>image-registration-plugin</summary>

* Version: 0.3.5
* Language: Python
* Status: Old
* bfio: 1.x
* filepattern: 1.2.4
* preadator: None
* nyxus: None

</details>  <!-- end image-registration-plugin -->

<details>
<summary>imagej-deconvolve-richardsonlucy-plugin</summary>

* Version: 0.4.3
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-deconvolve-richardsonlucy-plugin -->

<details>
<summary>imagej-deconvolve-richardsonlucytv-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-deconvolve-richardsonlucytv-plugin -->

<details>
<summary>imagej-filter-addpoissonnoise-plugin</summary>

* Version: 0.4.4
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-filter-addpoissonnoise-plugin -->

<details>
<summary>imagej-filter-convolve-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-filter-convolve-plugin -->

<details>
<summary>imagej-filter-correlate-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-filter-correlate-plugin -->

<details>
<summary>imagej-filter-derivativegauss-plugin</summary>

* Version: 0.4.4
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-filter-derivativegauss-plugin -->

<details>
<summary>imagej-filter-dog-plugin</summary>

* Version: 0.3.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-filter-dog-plugin -->

<details>
<summary>imagej-filter-frangivesselness-plugin</summary>

* Version: 0.4.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-filter-frangivesselness-plugin -->

<details>
<summary>imagej-filter-gauss-plugin</summary>

* Version: 0.3.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-filter-gauss-plugin -->

<details>
<summary>imagej-filter-partialderivative-plugin</summary>

* Version: 0.3.5
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-filter-partialderivative-plugin -->

<details>
<summary>imagej-filter-sobel-plugin</summary>

* Version: 0.3.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-filter-sobel-plugin -->

<details>
<summary>imagej-filter-tubeness-plugin</summary>

* Version: 0.3.8
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-filter-tubeness-plugin -->

<details>
<summary>imagej-image-integral-plugin</summary>

* Version: 0.3.2
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-image-integral-plugin -->

<details>
<summary>imagej-image-invert-plugin</summary>

* Version: 0.4.0
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-image-invert-plugin -->

<details>
<summary>intensity-projection-plugin</summary>

* Version: 0.1.9
* Language: Python
* Status: Old
* bfio: 2.0.5
* filepattern: None
* preadator: 0.2.0
* nyxus: None

</details>  <!-- end intensity-projection-plugin -->

<details>
<summary>rolling-ball-plugin</summary>

* Version: 1.1.0-dev0
* Language: Python
* Status: Peer Review
* PR: [#429](https://github.com/PolusAI/polus-plugins/pull/429)
* bfio: 2.1.9
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end rolling-ball-plugin -->

<details>
<summary>stack-z-slice-plugin</summary>

* Version: 1.2.4
* Language: Python
* Status: Old
* bfio: 2.x
* filepattern: 1.4.7
* preadator: 0.2.0
* nyxus: None

</details>  <!-- end stack-z-slice-plugin -->

<details>
<summary>roi-relabel-plugin</summary>

* Version: 0.2.2
* Language: Python
* Status: Updated
* bfio: 2.1.9
* filepattern: 2.0.0
* preadator: None
* nyxus: None

</details>  <!-- end roi-relabel-plugin -->

#### Tabular

<details>
<summary>csv-merger-plugin</summary>

* Version: 0.4.0
* Language: Python
* Status: Old
* bfio: None
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end csv-merger-plugin -->

<details>
<summary>generalized-linear-model-plugin</summary>

* Version: 0.2.5
* Language: R
* Status: Unknown
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end generalized-linear-model-plugin -->

<details>
<summary>tabular-thresholding-plugin</summary>

* Version: 0.1.3
* Language: Python
* Status: Updated
* bfio: None
* filepattern: test-2.2.7
* preadator: None
* nyxus: None

</details>  <!-- end tabular-thresholding-plugin -->

### Utils

<details>
<summary>filepattern-generator-plugin</summary>

* Version: 0.2.1
* Language: Python
* Status: Old
* bfio: None
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end filepattern-generator-plugin -->

<details>
<summary>csv-collection-merger</summary>

* Version: 0.1.1
* Language: sh
* Status: Old
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end csv-collection-merger -->

<details>
<summary>generic-to-image-collection-plugin</summary>

* Version: 0.1.1
* Language: Python
* Status: Old
* bfio: 2.x
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end generic-to-image-collection-plugin -->

<details>
<summary>imagej-macro-plugin</summary>

* Version: 0.1.3
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end imagej-macro-plugin -->

<details>
<summary>notebook-plugin</summary>

* Version: 0.4.0
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end notebook-plugin -->

<details>
<summary>stitching-vector-merger-plugin</summary>

* Version: 0.1.8
* Language: Python
* Status: Old
* bfio: None
* filepattern: None
* preadator: None
* nyxus: None

</details>  <!-- end stitching-vector-merger-plugin -->

<details>
<summary>subset-data-plugin</summary>

* Version: 0.1.8
* Language: Python
* Status: Old
* bfio: None
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end subset-data-plugin -->

### Visualization

<details>
<summary>color-pyramid-builder-plugin</summary>

* Version: 0.3.3
* Language: Python
* Status: Updated
* bfio: 1.x
* filepattern: 1.2.4
* preadator: None
* nyxus: None

</details>  <!-- end color-pyramid-builder-plugin -->

<details>
<summary>feature-heatmap-pyramid-plugin</summary>

* Version: 0.2.0
* Language: Python
* Status: Updated
* bfio: 1.x
* filepattern: 1.2.4
* preadator: None
* nyxus: None

</details>  <!-- end feature-heatmap-pyramid-plugin -->

<details>
<summary>graph-pyramid-builder-plugin</summary>

* Version: 1.3.8
* Language: Python
* Status: Updated
* bfio: 1.x
* filepattern: 1.2.4
* preadator: None
* nyxus: None

</details>  <!-- end graph-pyramid-builder-plugin -->

<details>
<summary>image-cluster-annotation-plugin</summary>

* Version: 0.2.4
* Language: Python
* Status: Updated
* bfio: 2.x
* filepattern: 1.2.4
* preadator: None
* nyxus: None

</details>  <!-- end image-cluster-annotation-plugin -->

<details>
<summary>precompute-slide-plugin</summary>

* Version: 1.7.0-dev0
* Language: Python
* Status: Peer Review
* PR: [#484](https://github.com/PolusAI/polus-plugins/pull/484)
* bfio: 2.1.9
* filepattern: 2.0.4
* preadator: 0.4.0-dev2
* nyxus: None

</details>  <!-- end precompute-slide-plugin -->

<details>
<summary>precompute-volume-plugin</summary>

* Version: 1.7.0-dev0
* Language: Python
* Status: Old
* bfio: 2.1.9
* filepattern: 1.4.7
* preadator: None
* nyxus: None

</details>  <!-- end precompute-volume-plugin -->

<details>
<summary>tabular-to-microjson-plugin</summary>

* Version: 0.1.0
* Language: Python
* Status: Updated
* bfio: None
* filepattern: 2.0.1
* preadator: None
* nyxus: None

</details>  <!-- end tabular-to-microjson-plugin -->
