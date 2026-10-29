<p align="center">
  <a href="https://gpuzero.dev">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="gpuzero-lockup-dark.svg">
      <img src="gpuzero-lockup.svg" alt="GPU Zero" height="48">
    </picture>
  </a>
</p>

<p align="center">
  <b>Training on your own cloud.</b><br>
  GPUs that start when there is a job, checkpoint every step, and stop when the work or the budget is done.
</p>

<p align="center">
  <a href="https://gpuzero.dev">gpuzero.dev</a>
</p>

---

The open-source pieces under GPU Zero. Each one is useful on its own, without the others and without an account.

| | |
|---|---|
| **[Ravex](https://github.com/gpuzero-dev/ravex)** | Checkpoint and resume for PyTorch, from one decorator on the function that trains. Kill the process, run the same command, and it picks up where it stopped. Pure Python. `pip install ravex` |
| **[Moonclip](https://github.com/gpuzero-dev/moonclip)** | The checkpoint engine underneath: Rust with Python bindings, saves only what changed as compressed deltas, writes in the background, to a local path or any S3 bucket. `pip install moonclip` |
| **[Smith](https://github.com/gpuzero-dev/smith)** | The agent on a training node. Takes jobs from a queue and runs the scripts it was configured with, never commands it was sent. |

Ravex and Moonclip are Apache-2.0.
