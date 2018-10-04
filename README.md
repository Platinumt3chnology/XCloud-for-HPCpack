## Python for HPC: ECP Community Materials

This site provides a combination of original resources and recommended links for Python users in
the ECP and broader scientific community. It is part of the [IDEAS-ECP](https://ideas-productivity.org/ideas-ecp) project.

### Quick-start Guides
 - [Python for HPC](tutorials/python.whatis.md)
 - [Creating a PYPI package](tutorials/python.pypi-packaging.md)
 - [Using Conda / Anaconda](tutorials/python.conda.md)
 - [Documenting with Sphinx](tutorials/python.doc-sphinx.md)

### Presentations
 - [Python for High Performance Computing](https://github.com/wscullin/ecp_python_tutorial/blob/master/slides/ECP_Python_Tutorial_2018.pdf) ECP Annual Meeting 2018. William Scullin (ALCF), Matt Belhorn (OLCF) and Rollin Thomas (NERSC)
 - [HPC Python Testing and Debugging Tutorial 2018](https://github.com/wscullin/ecp_python_tutorial/blob/master/slides/debugging_slides.pdf) ECP Annual Meeting 2018. Matt Belhorn (OLCF), William Scullin (ALCF), Rollin Thomas (NERSC) 
 - [Analyzing Python Performance with Intel VTune](https://www.alcf.anl.gov/files/Tullos-Analyzing_Python_Performance.pdf) 2017 Intel presentation.
 - [Using and Scaling Python](https://www.alcf.anl.gov/files/Scullin-Pavlyk%20_SDL2018_Python.pdf) ALCF Simulation, Data, and Learning Workshop 2018. William Scullin (ALCF) and Oleksandr Pavlyk (Intel)

### Webinars
 - [Python in HPC Webinar 2017 (See Webinar No. 8)](https://ideas-productivity.org/events/hpc-best-practices-webinars) 
 - [Jupyter and HPC: Current State and Future Roadmap 2018 (Webinar No.15)](https://ideas-productivity.org/events/hpc-best-practices-webinars) 

### Tips on Python for Scientific Computing
 - [Interrogating NumPy Configuration/Compiler Options](tutorials/interrogating_numpy.md)
 - [Links for moving from Matlab to NumPy](tutorials/matlab-numpy-conversion.md)
 
### Python resources for computational scientists
 - [XSD Python Training Home: Python lecture/video series for Scientists](https://confluence.aps.anl.gov/display/XSDPT/XSD+Python+Training+Home) (From Argonne APS) Recommended as an introductory course for scientists.
 - [SciPy Lectures](http://www.scipy-lectures.org/) A community-based series of tutorials.
 - [On-demand learning for Python - using a Transmedia Learning Framework](https://bssw.io/resources/transmedia-learning-frameworks-tlf)

 
### Scientific Libraries

#### Scientific computing packages in Python (running C extensions):
 - [NumPy](http://www.numpy.org/) NumPy is the fundamental package for scientific computing with Python.
 - [SciPy](https://www.scipy.org/) A Python-based ecosystem of open-source software for mathematics, science, and engineering. Now incorporates: Numpy, the SciPy library, Matplotlib, IPython, SymPy and Pandas.
 
#### Parallel and Distributed Programming Options:
 
 Note: Python provides an in-built [threading](https://docs.python.org/3/library/threading.html) module. However, this is not really suitable for parallel computation due to the [GIL](https://wiki.python.org/moin/GlobalInterpreterLock) (Global Interpreter Lock)
 
 - [mpi4py](https://mpi4py.readthedocs.io/en/stable/) Python wrapper for MPI
 - [Multiprocessing module](https://docs.python.org/3/library/multiprocessing.html) Basic multiple process parallelism through forked interpreters (with threading like interface). Be aware of issues mixing with OpenMP, MPI, or shared memory tools.


#### Python bindings to scientific libraries in HPC:
 - [petsc4py](https://bitbucket.org/petsc/petsc4py) Python bindings for PETSc
 - [slepc4py](https://bitbucket.org/slepc/slepc4py) Python bindings for SLEPc, the Scalable Library for Eigenvalue Problem Computations
 - [PyTrilinos](https://trilinos.org/packages/pytrilinos/) A set of python wrappers for selected Trilinos packages

#### I/O:
 - [h5py](https://www.h5py.org/) The h5py package is a Pythonic interface to the HDF5 binary data format.

 
### Python on Accelerators

 - [Numba](https://numba.pydata.org/) Numba is an open source JIT compiler that translates a subset of Python and NumPy code into fast machine code (Mark hotspot functions with decorators and they are compiled.). Numba supports Intel and AMD x86, POWER8/9, and ARM CPUs, NVIDIA and AMD GPUs. Relies on decorators to identify code sections to accelerate. Requires LLVM. Works with the standard CPython.  [Accelerating Python with the Numba (Video)](https://www.youtube.com/watch?v=eYIPEDnp5C4)
 - [PyCUDA](https://documen.tician.de/pycuda/tutorial.html)
   PyCUDA lets you access Nvidia's CUDA parallel computation API from Python.
 - [PyOpenCL](https://documen.tician.de/pyopencl/index.html)
   PyOpenCL lets you access the OpenCL parallel computation API from Python


### Ensemble and Workflow tools
 
 - [Parsl](http://parsl-project.org) Use Parsl with Jupyter notebooks to scale interactive analyses from laptops to supercomputers. [video](https://www.youtube.com/watch?v=tHTt0Pyb4_M)
 - [Balsam](https://www.alcf.anl.gov/balsam) Workflow system for managing large campaigns of interdependent jobs (unlimited queue depth). Balsam manages a database of jobs, with specified dependences. Jobs can be added to the database from anywhere on the system, for dynamic workflows.
 - [libEnsemble](https://libensemble.readthedocs.io) Library for dynamic ensembles using generator and simulator functions (e.g. using numerical optimization).


### Conferences and Events
 - [SciPy 2018 Videos](https://www.youtube.com/playlist?list=PLYx7XA2nY5Gd-tNhm79CNMe_qvi35PgUR)
 - [ALCF Simulation, Data and Learning Workshop 2018](https://www.alcf.anl.gov/workshops/sdl-workshop-oct2018) Includes slides for many relevant presentations.
 - PyHPC Workshop 2018 (In conjunction with SC18) [Announcements](https://twitter.com/pythonhpc?lang=en) [Register](https://www.dlr.de/sc/desktopdefault.aspx/tabid-12954/22625_read-52397/)
 
Find more software engineering materials for computational scientists at the [Better Scientific Software](https://bssw.io/) website.


### Feedback

Any feedback, corrections and suggested additions are welcome: shudson@anl.gov

<iframe src="https://ghbtns.com/github-btn.html?user=betterscientificsoftware&repo=python-for-hpc&type=star&count=false&size=large" frameborder="0" scrolling="0" width="160px" height="30px"></iframe>
