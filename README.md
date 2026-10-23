# repo2rlenv-crabbox-demo

Demo record (May 2026) for [`huggingface/Repo2RLEnv#53`](https://github.com/huggingface/Repo2RLEnv/pull/53), closed unmerged —
an adapter that runs Repo2RLEnv `pr_diff` tasks on islo.dev sandboxes via [openclaw/crabbox](https://github.com/openclaw/crabbox).

▶ **https://zozo123.github.io/repo2rlenv-crabbox-demo/**

The page records three runs on an islo.dev sandbox (May 2026):

- single task, oracle diff → `final_reward = 1.0`
- single task, empty diff → `final_reward = 0.0`
- 3-task batch (j=3) → all 1.0 in ~57 s wall

Wrapper source (on the fork; the PR was closed unmerged):
[`examples/crabbox/runner.py`](https://github.com/zozo123/Repo2RLEnv/blob/727d33f9416936b14d14a5e3fd1e351d61fb9bee/examples/crabbox/runner.py).

By [Yossi Eliaz](https://zozo123.github.io/).
