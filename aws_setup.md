Setup keys in `$aws configure` and use `us-west-2`.

Create instance using `$bash ~/git/PracticalDeepLearningforCoders/courses/setup/setup_t2_micro.sh`.

If see error "A client error (InvalidKeyPair.NotFound) occurred when calling the RunInstances operation: The key pair 'aws-key-fast-ai' does not exist " Do
`$ rm ~/.ssh/aws-key-fast-ai.pem`
Inside the instance:
```
$ nvidia-smi
$ sudo rm .bash_history`
$ jupyter notebook
```
Password for notebook: `dl_course`.
In `.bash_profile`, add
```
alias ssh_fastai_t2='ssh -i [YOUR_HOME].ssh/aws-key-fast-ai.pem ubuntu@ec2-[IP].us-west-2.compute.amazonaws.com'
```

Notebook is on `[IP]:8888`.
