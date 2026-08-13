---
icon: fontawesome/brands/python
---

# Python

## :material-file-cog: **pys3fuse**

`pys3fuse` is a FUSE filesystem written in Python that brings S3-compatible
object storage into the POSIX filesystem world. Instead of interacting with
an S3 bucket exclusively through an object-storage API, the project lets
you expose a bucket through a mounted directory and work with it using
familiar filesystem operations. 

The project can be installed as a Python package and run directly as a
module. After installing the required FUSE libraries and creating a mount
directory, `pys3fuse` can be launched with `python -m pys3fuse --help`,
providing a small but interesting intersection between Python, filesystems,
FUSE, and S3-compatible storage.

:octicons-mark-github-24: [View repository](https://github.com/mahdihaghverdi/pys3fuse){:target="_blank"}

!!! success

    This project was my bachelor's final project.
    
!!! info

    :lucide-corner-down-right: [Proposal](https://github.com/mahdihaghverdi/BCProject/blob/main/Proposal/proposal.pdf){:target="_blank"}
    :lucide-corner-down-right: [Project Report](https://github.com/mahdihaghverdi/pys3fuse/blob/main/Docs/main.pdf){:target="_blank"}
---

## :material-language-python: **listappend**

`listappend` is a small research-oriented project created to accompany a
deep dive into how Python's `list.append()` is implemented inside the
CPython interpreter. Rather than being a conventional library, it contains
the code and experiments used to investigate the behavior of
`PyListObject` and its `append` method at the C layer. 

The repository separates Python-level implementations from experiments
that collect statistics from the actual CPython interpreter. The `imple`
directory contains Python implementations of the relevant code, while
`nativeimpl` is used for gathering measurements from CPython itself,
making the project a practical companion to understanding Python's runtime
internals. 

:octicons-mark-github-24: [View repository](https://github.com/mahdihaghverdi/listappend){:target="_blank"}

---

## :material-code-braces: **PLCompiler**

`PLCompiler` is a compiler-design project developed for a university
Compiler Design course. The project is structured around the classical
compiler pipeline and is planned in multiple phases, starting with
tokenization and continuing through syntactic and semantic parsing. 

The repository includes a dedicated `PLTokenizer` component as well as
documentation for the project, and it can be executed directly through
Python with `python -m PLCompiler --help`. The project provides a practical
way to explore the transition from source code to tokens and, eventually,
to syntactic and semantic understanding of a programming language.

:octicons-mark-github-24: [View repository](https://github.com/mahdihaghverdi/plcompiler){:target="_blank"}

---

## :material-api: **SimpleRESTBlog**

`SimpleRESTBlog` is a fully asynchronous RESTful blog API built with
Python and FastAPI, backed by PostgreSQL. Its architecture is deliberately
layered and decoupled, separating the data, service, and API layers while
using dependency injection to keep higher layers independent from lower
level implementation details.

The project goes beyond a basic CRUD API: it includes JWT-based
authentication, TOTP two-factor authentication, ACL-based authorization,
PostgreSQL's `LTree` for hierarchical comments, Redis integration,
pagination, migrations with Alembic, and automated linting and formatting.
The resulting architecture provides a practical example of structuring a
non-trivial asynchronous Python backend as a collection of independent
layers and services. 

:octicons-mark-github-24: [View repository](https://github.com/mahdihaghverdi/simplerestblog){:target="_blank"}
