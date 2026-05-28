# repo2rlenv-crabbox-demo

Live demo for [`huggingface/Repo2RLEnv#53`](https://github.com/huggingface/Repo2RLEnv/pull/53) —
runs Repo2RLEnv `pr_diff` tasks on islo.dev sandboxes via [crabbox](https://github.com/openclaw/crabbox).

▶ **https://zozo123.github.io/repo2rlenv-crabbox-demo/**

The site shows three verified runs on a live islo.dev sandbox:

- single task, oracle diff → `final_reward = 1.0`
- single task, empty diff → `final_reward = 0.0`
- 3-task batch (j=3) → all 1.0 in ~57 s wall

Source of the wrapper lives in the PR:
[`examples/crabbox-islo/runner.py`](https://github.com/huggingface/Repo2RLEnv/blob/feat/crabbox-islo-example/examples/crabbox-islo/runner.py).
