# GIL

In the default CPython build, the global interpreter lock (GIL) lets only one thread execute Python bytecode at a time, limiting parallelism for CPU-bound Python code. CPython 3.13 introduced an optional free-threaded build that can run with the GIL disabled, allowing Python threads to execute in parallel. Free threading is officially supported as of 3.14, but the free-threaded build is not the default.

Visit the following resources to learn more:

- [@official@Python Support for Free Threading](https://docs.python.org/3/howto/free-threading-python.html)
- [@article@What is GIL?](https://realpython.com/python-gil/)
- [@article@Python Multithreading: The Most Practical Intro](https://roadmap.sh/python/multithreading)
