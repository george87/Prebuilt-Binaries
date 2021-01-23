*Numba 0.52.0* binaries
-----------------------

- Sources downloaded from [[PyPI]: numba - numba-0.52.0.tar.gz](https://files.pythonhosted.org/packages/46/e1/cbbc7c7967d9b10e54c852bf5bece0222a63bfb809d3354014c957ef1bda/numba-0.52.0.tar.gz)
- Modified them in order to compile, as *Python 3.9* *API* is a bit changed
- Built with:
    - *NumPy 1.19.4* (**modified** version on *pc064* to bypass temporary fix for [[GitHub]: numpy/numpy - polyfit and eig regression tests fail after Windows 10 update to 2004](https://github.com/numpy/numpy/issues/16744))
    - *TBB 2020.3* (compatible *tbb.dll* (and maybe other dependencies) required at runtime, if this feature is to be used)

- **Tests fail**:
    - I don't know how relevant that is, because **same thing happens** with official *.whls* for *Python 3.8* (something is definitely wrong here)
    - Not a strong argument, but *code00.py* from [[SO]: Executing the assembly generated by Numba (@CristiFati's answer)](https://stackoverflow.com/questions/61678226/executing-the-assembly-generated-by-numba/61859833#61859833) produces same results for *Python*: *v3.8* and *v3.9*

**Platforms**:
- *Windows*
