# check-quota

Show SLURM GPU partition usage: total / allocated / idle nodes, and how many nodes each active user is running or has queued.

## Requirements

- Python 3.9+
- [click](https://pypi.org/project/click/)
- SLURM commands (`sinfo`, `squeue`) on `PATH`

## Install

```bash
pip install click
cp check_quota ~/.local/bin/
chmod +x ~/.local/bin/check_quota
```

## Usage

```bash
check_quota              # default partition: gpu
check_quota -p cpu       # another partition
```
