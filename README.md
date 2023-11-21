# qsub

```
# interactive mode
qsub -I -q gpuvolta -l ncpus=12,ngpus=1,mem=64gb,walltime=04:00:00
```

```
# check if job not running
qstat -u $USER -Esw
```



```
# Device info
# CPU
cat /proc/cpuinfo
# GPU
nvidia-smi
# OS
lsb_release -a

# other
sudo lshw -C display
