> [!NOTE]
> **9base status: Historical** · **Lifecycle: archived.**
>
> This repository is retained as historical material and is not actively maintained by 9base.
> The provenance and scope below distinguish local work from inherited projects and dependencies.

# NVIDIA Stuff — historical container launcher collection

This is Suleyman Poyraz's (Zaryob's) small collection of Jetson Nano/NVIDIA
installation notes and Docker launcher commands from **2022**. Its two recorded
local commits add the script collection in January and the short README in
August 2022. It is now retained as historical engineering material and archived
after documentation; it is not actively maintained.

## Material index

| Directory | Retained material and recorded image references |
| --- | --- |
| [caffe2](caffe2) | Launcher and short note; `nvcr.io/nvidia/caffe2:18.08-py3` |
| [julia](julia) | Julia launcher; `nvcr.io/hpc/julia:v2.4.1` |
| [l4](l4) | L4T base, CUDA, ML and framework launcher variants; includes `l4t-base:r32.6.1`, `l4t-cuda:10.2.460-runtime`, `l4t-ml:r32.6.1-py3`, `l4t-pytorch:r32.6.1-pth1.9-py3` and `tensorflow:21.12-tf1-py3` under `nvcr.io/nvidia` |
| [matlab](matlab) | MATLAB launcher and short note; `nvcr.io/partners/matlab:r2021b` |
| [nvdli-data](nvdli-data) | NVIDIA DLI Nano AI launcher; `nvcr.io/nvidia/dli/dli-nano-ai:v2.0.2-r32.6.1kr` |
| [pytorch](pytorch) | PyTorch launcher; `nvcr.io/nvidia/pytorch:21.12-py3` |
| [tensorflow](tensorflow) | TensorFlow launcher; `nvcr.io/nvidia/tensorflow:21.12-tf1-py3` |

These are references recorded in the scripts, not newly built 9base images or
verified currently available downloads. Some commands reference L4T/Jetson
images while others select general NVIDIA GPU or partner images; the collection
does not establish that all of them ran on Jetson Nano or one common architecture.

The scripts record GPU runtime options, host networking and workstation-specific
mounts such as `~/images/...`, TensorRT/Python 3.6 directories and `/usr/src`.
The DLI example also references the Argus socket and `/dev/video0`. Those paths
describe the original command assumptions, not a portable installation recipe.

## Scope and attribution

9base's contribution is the local command/note collection. NVIDIA, partner
images, Julia, MATLAB, Caffe2, PyTorch, TensorFlow and their dependencies remain
their respective projects' work. This is not a complete ML framework source
tree, a downstream container distribution or a tested current image matrix.
No current build, image pull, hardware execution or licensing change was made.
There is no evidenced relationship to the Tinker Board 2 family.

## Archival reconstruction note

This explanation was reconstructed on **8 October 2026** from the public
repository tree, metadata and commit history. It is new documentation of
historical material, not evidence that this explanation existed during the
original development period. Original source authorship, technical history
and license files have not been rewritten.

---

## Legacy README (preserved unchanged)

# NVIDIA Stuff

NVIDIA Jetson nano installation guides
